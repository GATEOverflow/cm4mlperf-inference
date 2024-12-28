This experiment is generated using the [MLCommons Collective Mind automation framework (CM)](https://github.com/mlcommons/cm4mlops).

*Check [CM MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.8.0-49-generic-x86_64-with-glibc2.29
* CPU version: x86_64
* Python version: 3.8.10 (default, Nov  7 2024, 13:10:47) 
[GCC 9.4.0]
* MLCommons CM version: 3.5.2

## CM Run Command

See [CM installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U cmind

cm rm cache -f

cm pull repo mlcommons@mlperf-automations --checkout=467517e4a572872046058e394a0d83512cfff38b

cm run script \
	--tags=app,mlperf,inference,generic,_nvidia,_sdxl,_tensorrt,_test,_r4.1-dev_default,_float16,_offline \
	--quiet=true \
	--env.CM_MLPERF_MODEL_SDXL_DOWNLOAD_TO_HOST=yes \
	--env.CM_QUIET=yes \
	--env.CM_MLPERF_IMPLEMENTATION=nvidia \
	--env.CM_MLPERF_MODEL=sdxl \
	--env.CM_MLPERF_RUN_STYLE=test \
	--env.CM_MLPERF_SKIP_SUBMISSION_GENERATION=False \
	--env.CM_DOCKER_PRIVILEGED_MODE=True \
	--env.CM_MLPERF_BACKEND=tensorrt \
	--env.CM_MLPERF_SUBMISSION_SYSTEM_TYPE=datacenter \
	--env.CM_MLPERF_CLEAN_ALL=True \
	--env.CM_MLPERF_DEVICE= \
	--env.CM_MLPERF_USE_DOCKER=True \
	--env.CM_MLPERF_MODEL_PRECISION=float16 \
	--env.OUTPUT_BASE_DIR=/home/arjun/scc_gh_action_results \
	--env.CM_MLPERF_LOADGEN_SCENARIO=Offline \
	--env.CM_MLPERF_INFERENCE_SUBMISSION_DIR=/home/arjun/scc_gh_action_submissions \
	--env.CM_MLPERF_INFERENCE_VERSION=5.0-dev \
	--env.CM_RUN_MLPERF_INFERENCE_APP_DEFAULTS=r4.1-dev_default \
	--env.CM_MLPERF_SUBMISSION_DIVISION=open \
	--env.CM_RUN_MLPERF_SUBMISSION_PREPROCESSOR=False \
	--env.CM_MLPERF_SUBMISSION_GENERATION_STYLE=short \
	--env.CM_MLPERF_SUT_NAME_RUN_CONFIG_SUFFIX4=scc24-base \
	--env.CM_DOCKER_IMAGE_NAME=scc24-nvidia \
	--env.CM_MLPERF_INFERENCE_MIN_QUERY_COUNT=50 \
	--env.CM_MLPERF_LOADGEN_ALL_MODES=yes \
	--env.CM_MLPERF_INFERENCE_SOURCE_VERSION=5.0.4 \
	--env.CM_MLPERF_LAST_RELEASE=v5.0 \
	--env.CM_TMP_PIP_VERSION_STRING= \
	--env.CM_MODEL=sdxl \
	--env.CM_MLPERF_LOADGEN_COMPLIANCE=no \
	--env.CM_MLPERF_CLEAN_SUBMISSION_DIR=yes \
	--env.CM_RERUN=yes \
	--env.CM_MLPERF_LOADGEN_EXTRA_OPTIONS= \
	--env.CM_MLPERF_LOADGEN_MODE=performance \
	--env.CM_MLPERF_LOADGEN_SCENARIOS,=Offline \
	--env.CM_MLPERF_LOADGEN_MODES,=performance,accuracy \
	--env.CM_OUTPUT_FOLDER_NAME=test_results \
	--env.CM_DOCKER_REUSE_EXISTING_CONTAINER=no \
	--env.CM_DOCKER_DETACHED_MODE=yes \
	--add_deps_recursive.get-mlperf-inference-results-dir.tags=_version.r4_1-dev \
	--add_deps_recursive.get-mlperf-inference-submission-dir.tags=_version.r4_1-dev \
	--add_deps_recursive.mlperf-inference-nvidia-scratch-space.tags=_version.r4_1-dev \
	--add_deps_recursive.submission-checker.tags=_short-run \
	--add_deps_recursive.coco2014-preprocessed.tags=_size.50,_with-sample-ids \
	--add_deps_recursive.coco2014-dataset.tags=_size.50,_with-sample-ids \
	--add_deps_recursive.nvidia-preprocess-data.extra_cache_tags=scc24-base \
	--v=False \
	--print_env=False \
	--print_deps=False \
	--dump_version_info=True \
	--env.OUTPUT_BASE_DIR=/cm-mount/home/arjun/scc_gh_action_results \
	--env.CM_MLPERF_INFERENCE_SUBMISSION_DIR=/cm-mount/home/arjun/scc_gh_action_submissions \
	--env.SDXL_CHECKPOINT_PATH=/home/cmuser/CM/repos/local/cache/762e6805370c44eb/stable_diffusion_fp16 \
	--env.MLPERF_SCRATCH_PATH=/home/cmuser/CM/repos/local/cache/4db00c74da1e44c8
```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf (CM scripts),
 you should simply reload mlcommons@mlperf-automations without checkout and clean CM cache as follows:*

```bash
cm rm repo mlcommons@mlperf-automations
cm pull repo mlcommons@mlperf-automations
cm rm cache -f

```

## Results

Platform: a17ea85374b0-nvidia_original-gpu-tensorrt-vdefault-scc24-base

Model Precision: int8

### Accuracy Results 

### Performance Results 
`Samples per second`: `1.31542`
