# linux-scheduling-lab
This repo contains my hands-on experiments with **Linux scheduling**.
I’m exploring CFS, Real-Time (FIFO/RR), and Deadline scheduling policies, using both stock and PREEMPT_RT kernels.

## 📂 Structure
- **programs/** → C test programs (periodic tasks, CPU hogs, etc.)
- **scripts/** → automation scripts for running experiments
- **results/** → raw logs (cyclictest, ftrace, perf)
- **plots/** → latency histograms, runqueue graphs
- **docs/** → experiment write-ups and reports

## 🚀 Experiments
1. **Week 1: Baseline**
   - Run `cyclictest` under CFS vs FIFO
   - Collect ftrace logs (`sched_switch`, `sched_wakeup`)
   - Compare latencies

2. **Week 2: CPU Isolation**
   - Use `isolcpus` and `taskset` to shield RT tasks
   - Measure improvements in tail latency

(… more weeks will follow …)

---

### Goal
To build a strong portfolio in **Linux scheduling and real-time systems** by:
- Running reproducible experiments
- Sharing code, logs, and analysis
- Contributing small improvements back to open sourceHands-on experiments with Linux scheduling
