This experiment is generated using the [MLCommons Collective Mind automation framework (CM)](https://github.com/mlcommons/cm4mlops).

*Check [CM MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-6.1.112-1.el9.elrepo.x86_64-x86_64-with-glibc2.35
* CPU version: x86_64
* Python version: 3.10.12 (main, Sep 11 2024, 15:47:36) [GCC 11.4.0]
* MLCommons CM version: 3.2.2

## CM Run Command

See [CM installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U cmind

cm rm cache -f

cm pull repo mlcommons@cm4mlops --checkout=bcde11676cc734f2398028a039fc1c94ae9fa81a

cm run script \
	--tags=run-mlperf,inference,_r4.1-dev \
	--model=bert-99 \
	--implementation=reference \
	--framework=pytorch \
	--category=edge \
	--scenario=Offline \
	--execution_mode=valid \
	--device=cuda \
	--quiet
```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf (CM scripts),
 you should simply reload mlcommons@cm4mlops without checkout and clean CM cache as follows:*

```bash
cm rm repo mlcommons@cm4mlops
cm pull repo mlcommons@cm4mlops
cm rm cache -f

```

## Results

Platform: 666dfb9811e4-reference-gpu-pytorch-cu124

Model Precision: fp32

### Accuracy Results 
`F1`: `90.87602`, Required accuracy for closed division `>= 89.96526`

### Performance Results 
`Samples per second`: `85.4467`
