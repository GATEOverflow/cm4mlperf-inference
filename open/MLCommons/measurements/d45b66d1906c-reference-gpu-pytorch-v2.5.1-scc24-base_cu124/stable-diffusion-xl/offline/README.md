This experiment is generated using the [MLCommons Collective Mind automation framework (CM)](https://github.com/mlcommons/cm4mlops).

*Check [CM MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.2.0-39-generic-x86_64-with-glibc2.35
* CPU version: x86_64
* Python version: 3.10.12 (main, Sep 11 2024, 15:47:36) [GCC 11.4.0]
* MLCommons CM version: 3.3.4

## CM Run Command

See [CM installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U cmind

cm rm cache -f

cm pull repo gateoverflow@cm4mlops --checkout=c4e45d45a3bda44e57d86a3aa5cfbdca4ff34541

cm run script \
	--tags=run-mlperf,inference,_r4.1-dev,_short,_scc24-base \
	--model=sdxl \
	--implementation=reference \
	--backend=pytorch \
	--category=datacenter \
	--scenario=Offline \
	--execution_mode=test \
	--device=cuda \
	--precision=float16 \
	--docker_it=no \
	--docker_cm_repo=gateoverflow@cm4mlops \
	--docker_dt=yes \
	--quiet \
	--results_dir=/home/cmuser/scc_gh_action_results \
	--submission_dir=/home/cmuser/scc_gh_action_submissions \
	--precision=float16 \
	--env.CM_MLPERF_MODEL_SDXL_DOWNLOAD_TO_HOST=yes \
	--clean
```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf (CM scripts),
 you should simply reload gateoverflow@cm4mlops without checkout and clean CM cache as follows:*

```bash
cm rm repo gateoverflow@cm4mlops
cm pull repo gateoverflow@cm4mlops
cm rm cache -f

```

## Results

Platform: d45b66d1906c-reference-gpu-pytorch-v2.5.1-scc24-base_cu124

Model Precision: fp32

### Accuracy Results 
`CLIP_SCORE`: `16.3689`, Required accuracy for closed division `>= 31.68632` and `<= 31.81332`
`FID_SCORE`: `237.82579`, Required accuracy for closed division `>= 23.01086` and `<= 23.95008`

### Performance Results 
`Samples per second`: `0.382853`
