# UWM_ECE757_project_26sp
project proposal: https://docs.google.com/document/d/1MOxm9JDT42SOu8l0D4pbyJysy6ABp9lJLKtDCHpbAY4/edit?tab=t.0

# Workload Design
## option1
a logic-simulation workload 

pros:
- a more real-life problem 
- based on whatever TA provided; possibly can be extended to be more complex

cons: not sure if we should extend or if it is easy to extend

## option2
Design 3–4 workload/graph families. Each workload/graph describe a typical scenarios. For example,
- workload1: a few long low-priority jobs come first, and many short high-priority jobs arrives over time
- workload2:

cons: don't know how a typical graph is defined, i.e., how to design the proportion of different types of kernels (nodes) in one graph


# Scheduling
The simplest approach might assign each node to a single GPU and execute tasks one at a time. 
As an extension, you could also explore more advanced strategies, such as allowing multiple GPUs to collaborate on a larger task. Of course, this introduces additional considerations (e.g., memory transfers between GPUs and coordination overhead), so it would be reasonable to start with a simpler design and then extend it if time permits. 
You could then implement and compare several scheduling policies (e.g., FIFO, priority-based, or dependency-aware policies) 

# Evaluation 
metrics such as total execution time, waiting time, fairness, or GPU utilization.

# Results

# Reference
[1] Algorithmic Techniques for GPU Scheduling: A Comprehensive Survey https://www.mdpi.com/1999-4893/18/7/385 

[2] TimeGraph: GPU scheduling for real-time multi-tasking environments
*Note*: Designed a real-time scheduler that allows GPUs to execute tasks based on their priorities. It also gives each task a maximum usage time to prevent low priority tasks taking too many resources.
*Can be used in "scheduling design"*

