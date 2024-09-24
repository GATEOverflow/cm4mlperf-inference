Please download [summary.xlsx](summary.xlsx) to view the most recent results. 
 ```
[2024-09-24 15:19:44,825 submission_checker1.py:2911 INFO] Results=3, NoResults=0, Power Results=0
[2024-09-24 15:19:44,825 submission_checker1.py:2918 INFO] ---
[2024-09-24 15:19:44,825 submission_checker1.py:2919 INFO] Closed Results=0, Closed Power Results=0

[2024-09-24 15:19:44,825 submission_checker1.py:2924 INFO] Open Results=3, Open Power Results=0

[2024-09-24 15:19:44,825 submission_checker1.py:2929 INFO] Network Results=0, Network Power Results=0

[2024-09-24 15:19:44,825 submission_checker1.py:2934 INFO] ---
[2024-09-24 15:19:44,825 submission_checker1.py:2936 INFO] Systems=3, Power Systems=0
[2024-09-24 15:19:44,825 submission_checker1.py:2937 INFO] Closed Systems=0, Closed Power Systems=0
[2024-09-24 15:19:44,825 submission_checker1.py:2942 INFO] Open Systems=3, Open Power Systems=0
[2024-09-24 15:19:44,825 submission_checker1.py:2947 INFO] Network Systems=0, Network Power Systems=0
[2024-09-24 15:19:44,825 submission_checker1.py:2952 INFO] ---
[2024-09-24 15:19:44,825 submission_checker1.py:2957 INFO] SUMMARY: submission looks OK
INFO:root:       ! call "postprocess" from /home/runner/CM/repos/mlcommons@cm4mlops/script/run-mlperf-inference-submission-checker/customize.py

```

|    | Organization   | Availability   | Division   | SystemType   | SystemName   | Platform                                               | Model               | MlperfModel         | Scenario   |   Result | Accuracy                                                      |   number_of_nodes | host_processor_model_name   |   host_processors_per_node |   host_processor_core_count | accelerator_model_name   |   accelerators_per_node | Location                                                                                                  | framework   | operating_system                                | notes                             |   compliance |   errors | version   |   inferred | has_power   | Units     |
|---:|:---------------|:---------------|:-----------|:-------------|:-------------|:-------------------------------------------------------|:--------------------|:--------------------|:-----------|---------:|:--------------------------------------------------------------|------------------:|:----------------------------|---------------------------:|----------------------------:|:-------------------------|------------------------:|:----------------------------------------------------------------------------------------------------------|:------------|:------------------------------------------------|:----------------------------------|-------------:|---------:|:----------|-----------:|:------------|:----------|
|  0 | MLCommons      | available      | open       | datacenter   | 48ed6105bd85 | 48ed6105bd85-nvidia-gpu-TensorRT-scc24-main            | stable-diffusion-xl | stable-diffusion-xl | Offline    | 1.13292  | CLIP_SCORE: 15.586050063371658  FID_SCORE: 236.8087101317688  |                 1 | Intel(R) Xeon(R) w7-2495X   |                          1 |                          24 | NVIDIA GeForce RTX 4090  |                       1 | open/MLCommons/results/48ed6105bd85-nvidia-gpu-TensorRT-scc24-main/stable-diffusion-xl/offline            | TensorRT    | Ubuntu 20.04 (linux-6.2.0-39-generic-glibc2.31) | Automated by MLCommons CM v2.3.6. |            1 |        0 | v4.1      |          0 | False       | Samples/s |
|  1 | MLCommons      | available      | open       | datacenter   | 48ed6105bd85 | 48ed6105bd85-nvidia-gpu-TensorRT-scc24-base            | stable-diffusion-xl | stable-diffusion-xl | Offline    | 1.13598  | CLIP_SCORE: 15.586050063371658  FID_SCORE: 236.8087101317688  |                 1 | Intel(R) Xeon(R) w7-2495X   |                          1 |                          24 | NVIDIA GeForce RTX 4090  |                       1 | open/MLCommons/results/48ed6105bd85-nvidia-gpu-TensorRT-scc24-base/stable-diffusion-xl/offline            | TensorRT    | Ubuntu 20.04 (linux-6.2.0-39-generic-glibc2.31) | Automated by MLCommons CM v2.3.6. |            1 |        0 | v4.1      |          0 | False       | Samples/s |
|  2 | MLCommons      | available      | open       | datacenter   | 48ed6105bd85 | 48ed6105bd85-reference-gpu-pytorch_v2.1.0a0-scc24-base | stable-diffusion-xl | stable-diffusion-xl | Offline    | 0.373636 | CLIP_SCORE: 15.236237794160843  FID_SCORE: 238.78369342212613 |                 1 | Intel(R) Xeon(R) w7-2495X   |                          1 |                          24 | NVIDIA GeForce RTX 4090  |                       1 | open/MLCommons/results/48ed6105bd85-reference-gpu-pytorch_v2.1.0a0-scc24-base/stable-diffusion-xl/offline | TensorRT    | Ubuntu 20.04 (linux-6.2.0-39-generic-glibc2.31) | Automated by MLCommons CM v2.3.6. |            1 |        0 | v4.1      |          0 | False       | Samples/s |