# Braintrust

## Welcome

### Concepts

Building blocks

`Trace` is fundamental object in Braintrust. A single trace is a single execution of an instrumented set of code. Traces appear in `Experiments` and `Logs`


```
Sounds just like Mlflow; traces, experiments
```

`Span` is an atomic unit of computation. Spans form the building blocks of a trace and can include

- Input
- Output
- Expected output
- Metadata
- Scores

`Objects and organizing constructs`

- Organization
    - Project
        - Experiment
            - Experiment Trace
        - Trace
            - Log Trace
        - Dataset
        - Prompt
        - Playground

`Systems` 

- Your code. Use `Eval()` to defince evaluations, `traced()` to trace code, and `.log()` to log data.
- The data plane, stores and serves data for experiments, logs, dataset, pomrpts, and playgrounds. By defailt, we host data plane for you, but you can self host
- The control plane, which hosts the Braintrust UI and metadata. Same thing we host but you can also self host



```
This is literally MLflow. Kind of like a Databricks without the compute provisioning, just the eval, tracing, logging.  
```

```
I think the last piece to the puzzle is monitoring. 
```
