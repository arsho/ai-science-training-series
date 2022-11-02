## Log
```
arsho@thetagpu06:~/ai-science-training-series/07_largeScaleTraining/src/ai4sci$ ./main.sh batch_size=512 > main-bs-512.log 2>&1 &
[1] 2926636
arsho@thetagpu06:~/ai-science-training-series/07_largeScaleTraining/src/ai4sci$ ls
10112556.cobaltlog  10112558.cobaltlog	10112558.output  ilsvrc_dataset.py  __init__.py  main-bs-512.log  main.sh     __pycache__
10112557.cobaltlog  10112558.error	conf		 ilsvrc.json	    logs	 main.py	  network.py  trainer.py
arsho@thetagpu06:~/ai-science-training-series/07_largeScaleTraining/src/ai4sci$ tail -f "main-bs-512.log" $(tail -1 logs/latest)
==> main-bs-512.log <==
┃  Job started at: 2022-11-02-145619 on thetagpu06           ┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛

The following have been reloaded with a version change:
  1) openmpi/openmpi-4.0.5 => openmpi/openmpi-4.1.4_ucx-1.12.1_gcc-9.4.0

Found venv at: /home/arsho/ai-science-training-series/07_largeScaleTraining/venv/, using that
./main.sh: line 132: /home/arsho/ai-science-training-series/07_largeScaleTraining/venvs/thetaGPU/2022-07-01/bin/activate: No such file or directory
Defaulting to user installation because normal site-packages is not writeable
Requirement already satisfied: pip in /lus/theta-fs0/software/thetagpu/conda/2022-07-01/mconda3/lib/python3.8/site-packages (22.3)

==> /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/logs/2022-11-02-194738-thetagpusn1_ngpu_ncpu128.log <==

==> main-bs-512.log <==
Defaulting to user installation because normal site-packages is not writeable
Obtaining file:///home/arsho/ai-science-training-series/07_largeScaleTraining
  Installing build dependencies: started
  Installing build dependencies: finished with status 'done'
  Checking if build backend supports build_editable: started
  Checking if build backend supports build_editable: finished with status 'done'
  Getting requirements to build editable: started
  Getting requirements to build editable: finished with status 'done'
  Preparing editable metadata (pyproject.toml): started
  Preparing editable metadata (pyproject.toml): finished with status 'done'
Building wheels for collected packages: ai4sci
  Building editable for ai4sci (pyproject.toml): started
  Building editable for ai4sci (pyproject.toml): finished with status 'done'
  Created wheel for ai4sci: filename=ai4sci-0.0.0-0.editable-py3-none-any.whl size=1166 sha256=086bff868af72f502be4091d7c7d4cdb2d20f5f1877994085f9db3af80cfa1de
  Stored in directory: /tmp/pip-ephem-wheel-cache-0v7v3h3t/wheels/67/b6/39/96fa820e234b3e0ea1ae80b7bed8d14c53de05072671ba8eeb
Successfully built ai4sci
Installing collected packages: ai4sci
  Attempting uninstall: ai4sci
    Found existing installation: ai4sci 0.0.0
    Uninstalling ai4sci-0.0.0:
      Successfully uninstalled ai4sci-0.0.0
Successfully installed ai4sci-0.0.0
WIDTH: 
DIR=/home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci
MAIN=/home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/main.py
PARENT=/home/arsho/ai-science-training-series/07_largeScaleTraining/src
ROOT=/home/arsho/ai-science-training-series/07_largeScaleTraining
LOGDIR=/home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/logs
LOGFILE=/home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/logs/2022-11-02-145619-thetagpu06_ngpu1_ncpu256.log
IBV_FORK_SAFE=
─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃  STARTING A NEW RUN ON 1 GPUs 256  ┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛


─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────┃  - DATE: 2022-11-02-145619
┃  - NCPUS: 256
┃  - NRANKS: 1
┃  - NGPUS PER RANK: 1
┃  - NGPUS TOTAL: 1
┃  - MAIN: /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/main.py
┃  - Writing logs to /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/logs/2022-11-02-145619-thetagpu06_ngpu1_ncpu256.log
┃  - python3: /lus/theta-fs0/software/thetagpu/conda/2022-07-01/mconda3/bin/python3
┃  - mpirun: /lus/theta-fs0/software/thetagpu/openmpi/openmpi-4.1.4_ucx-1.12.1_gcc-9.4.0/bin/mpirun
┃  - ai4sci: /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/__init__.py
┃  - exec: /lus/theta-fs0/software/thetagpu/openmpi/openmpi-4.1.4_ucx-1.12.1_gcc-9.4.0/bin/mpirun --verbose     -n 1     --hostfile /var/tmp/cobalt.10112558     -npernode 1     -x PYTHONUSERBASE     -x PYTHONSTARTUP     -x http_proxy     -x https_proxy     -x PATH     -x LD_LIBRARY_PATH /lus/theta-fs0/software/thetagpu/conda/2022-07-01/mconda3/bin/python3 /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/main.py batch_size=512
─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────

2022-11-02 14:58:11.693859: W tensorflow/core/grappler/costs/op_level_cost_estimator.cc:690] Error in PredictCost() for the op: op: "CropAndResize" attr { key: "T" value { type: DT_UINT8 } } attr { key: "extrapolation_value" value { f: 0 } } attr { key: "method" value { s: "bilinear" } } inputs { dtype: DT_UINT8 shape { dim { size: 1 } dim { size: -5 } dim { size: -6 } dim { size: 3 } } } inputs { dtype: DT_FLOAT shape { dim { size: -2 } dim { size: 4 } } } inputs { dtype: DT_INT32 shape { dim { size: -2 } } } inputs { dtype: DT_INT32 shape { dim { size: 2 } } } device { type: "CPU" vendor: "AuthenticAMD" model: "241" frequency: 2245 num_cores: 2 environment { key: "cpu_instruction_set" value: "SSE, SSE2, SSE3" } environment { key: "eigen" value: "3.4.90" } l1_cache_size: 32768 l2_cache_size: 524288 l3_cache_size: 268435456 memory_size: 268435456 } outputs { dtype: DT_FLOAT shape { dim { size: -2 } dim { size: -10 } dim { size: -11 } dim { size: 3 } } }
^C      
arsho@thetagpu06:~/ai-science-training-series/07_largeScaleTraining/src/ai4sci$ tail -f "main-bs-512.log" $(tail -1 logs/latest)
==> main-bs-512.log <==
┃  - NGPUS TOTAL: 1
┃  - MAIN: /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/main.py
┃  - Writing logs to /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/logs/2022-11-02-145619-thetagpu06_ngpu1_ncpu256.log
┃  - python3: /lus/theta-fs0/software/thetagpu/conda/2022-07-01/mconda3/bin/python3
┃  - mpirun: /lus/theta-fs0/software/thetagpu/openmpi/openmpi-4.1.4_ucx-1.12.1_gcc-9.4.0/bin/mpirun
┃  - ai4sci: /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/__init__.py
┃  - exec: /lus/theta-fs0/software/thetagpu/openmpi/openmpi-4.1.4_ucx-1.12.1_gcc-9.4.0/bin/mpirun --verbose     -n 1     --hostfile /var/tmp/cobalt.10112558     -npernode 1     -x PYTHONUSERBASE     -x PYTHONSTARTUP     -x http_proxy     -x https_proxy     -x PATH     -x LD_LIBRARY_PATH /lus/theta-fs0/software/thetagpu/conda/2022-07-01/mconda3/bin/python3 /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/main.py batch_size=512
─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────

2022-11-02 14:58:11.693859: W tensorflow/core/grappler/costs/op_level_cost_estimator.cc:690] Error in PredictCost() for the op: op: "CropAndResize" attr { key: "T" value { type: DT_UINT8 } } attr { key: "extrapolation_value" value { f: 0 } } attr { key: "method" value { s: "bilinear" } } inputs { dtype: DT_UINT8 shape { dim { size: 1 } dim { size: -5 } dim { size: -6 } dim { size: 3 } } } inputs { dtype: DT_FLOAT shape { dim { size: -2 } dim { size: 4 } } } inputs { dtype: DT_INT32 shape { dim { size: -2 } } } inputs { dtype: DT_INT32 shape { dim { size: 2 } } } device { type: "CPU" vendor: "AuthenticAMD" model: "241" frequency: 2245 num_cores: 2 environment { key: "cpu_instruction_set" value: "SSE, SSE2, SSE3" } environment { key: "eigen" value: "3.4.90" } l1_cache_size: 32768 l2_cache_size: 524288 l3_cache_size: 268435456 memory_size: 268435456 } outputs { dtype: DT_FLOAT shape { dim { size: -2 } dim { size: -10 } dim { size: -11 } dim { size: 3 } } }

==> /home/arsho/ai-science-training-series/07_largeScaleTraining/src/ai4sci/logs/2022-11-02-145619-thetagpu06_ngpu1_ncpu256.log <==
[2022-11-02 15:16:56,975][ai4sci.trainer][INFO] - [0] [0/1: 189440 / 1281167 (15%)] epoch=0.0000 dt=0.9026 running_loss=0.0013 batch_loss=0.0077 acc=0.0156 batch_acc=0.1777
[2022-11-02 15:17:25,393][ai4sci.trainer][INFO] - [0] [0/1: 194560 / 1281167 (15%)] epoch=0.0000 dt=0.8323 running_loss=0.0013 batch_loss=0.0084 acc=0.0162 batch_acc=0.1426
[2022-11-02 15:17:59,236][ai4sci.trainer][INFO] - [0] [0/1: 199680 / 1281167 (16%)] epoch=0.0000 dt=0.9253 running_loss=0.0013 batch_loss=0.0081 acc=0.0169 batch_acc=0.1348
[2022-11-02 15:18:23,689][ai4sci.trainer][INFO] - [0] [0/1: 204800 / 1281167 (16%)] epoch=0.0000 dt=0.8565 running_loss=0.0014 batch_loss=0.0077 acc=0.0175 batch_acc=0.1855
[2022-11-02 15:18:47,429][ai4sci.trainer][INFO] - [0] [0/1: 209920 / 1281167 (16%)] epoch=0.0000 dt=0.7583 running_loss=0.0014 batch_loss=0.0079 acc=0.0182 batch_acc=0.1465
[2022-11-02 15:19:18,967][ai4sci.trainer][INFO] - [0] [0/1: 215040 / 1281167 (17%)] epoch=0.0000 dt=0.7246 running_loss=0.0014 batch_loss=0.0078 acc=0.0188 batch_acc=0.1484
[2022-11-02 15:19:58,682][ai4sci.trainer][INFO] - [0] [0/1: 220160 / 1281167 (17%)] epoch=0.0000 dt=0.7677 running_loss=0.0015 batch_loss=0.0076 acc=0.0195 batch_acc=0.1641
[2022-11-02 15:20:23,814][ai4sci.trainer][INFO] - [0] [0/1: 225280 / 1281167 (18%)] epoch=0.0000 dt=0.7721 running_loss=0.0015 batch_loss=0.0081 acc=0.0201 batch_acc=0.1582
[2022-11-02 15:20:47,378][ai4sci.trainer][INFO] - [0] [0/1: 230400 / 1281167 (18%)] epoch=0.0000 dt=0.6071 running_loss=0.0015 batch_loss=0.0078 acc=0.0208 batch_acc=0.1855
[2022-11-02 15:21:24,133][ai4sci.trainer][INFO] - [0] [0/1: 235520 / 1281167 (18%)] epoch=0.0000 dt=0.6744 running_loss=0.0016 batch_loss=0.0076 acc=0.0215 batch_acc=0.1816
[2022-11-02 15:21:49,035][ai4sci.trainer][INFO] - [0] [0/1: 240640 / 1281167 (19%)] epoch=0.0000 dt=0.9607 running_loss=0.0016 batch_loss=0.0079 acc=0.0222 batch_acc=0.1465
[2022-11-02 15:22:12,838][ai4sci.trainer][INFO] - [0] [0/1: 245760 / 1281167 (19%)] epoch=0.0000 dt=0.8493 running_loss=0.0016 batch_loss=0.0079 acc=0.0229 batch_acc=0.1719
[2022-11-02 15:22:36,606][ai4sci.trainer][INFO] - [0] [0/1: 250880 / 1281167 (20%)] epoch=0.0000 dt=0.6921 running_loss=0.0017 batch_loss=0.0077 acc=0.0237 batch_acc=0.1934
[2022-11-02 15:23:00,861][ai4sci.trainer][INFO] - [0] [0/1: 256000 / 1281167 (20%)] epoch=0.0000 dt=0.7564 running_loss=0.0017 batch_loss=0.0078 acc=0.0244 batch_acc=0.1699
[2022-11-02 15:23:27,205][ai4sci.trainer][INFO] - [0] [0/1: 261120 / 1281167 (20%)] epoch=0.0000 dt=0.7827 running_loss=0.0017 batch_loss=0.0075 acc=0.0252 batch_acc=0.1836
[2022-11-02 15:23:51,023][ai4sci.trainer][INFO] - [0] [0/1: 266240 / 1281167 (21%)] epoch=0.0000 dt=0.7820 running_loss=0.0017 batch_loss=0.0075 acc=0.0260 batch_acc=0.2148
[2022-11-02 15:24:15,332][ai4sci.trainer][INFO] - [0] [0/1: 271360 / 1281167 (21%)] epoch=0.0000 dt=0.6922 running_loss=0.0018 batch_loss=0.0075 acc=0.0268 batch_acc=0.2207
[2022-11-02 15:24:50,030][ai4sci.trainer][INFO] - [0] [0/1: 276480 / 1281167 (22%)] epoch=0.0000 dt=0.6231 running_loss=0.0018 batch_loss=0.0076 acc=0.0275 batch_acc=0.2285
[2022-11-02 15:25:19,922][ai4sci.trainer][INFO] - [0] [0/1: 281600 / 1281167 (22%)] epoch=0.0000 dt=0.6182 running_loss=0.0018 batch_loss=0.0074 acc=0.0283 batch_acc=0.1973
[2022-11-02 15:25:43,636][ai4sci.trainer][INFO] - [0] [0/1: 286720 / 1281167 (22%)] epoch=0.0000 dt=0.7581 running_loss=0.0019 batch_loss=0.0075 acc=0.0291 batch_acc=0.2148
[2022-11-02 15:26:07,273][ai4sci.trainer][INFO] - [0] [0/1: 291840 / 1281167 (23%)] epoch=0.0000 dt=0.6097 running_loss=0.0019 batch_loss=0.0078 acc=0.0299 batch_acc=0.1914
[2022-11-02 15:26:31,653][ai4sci.trainer][INFO] - [0] [0/1: 296960 / 1281167 (23%)] epoch=0.0000 dt=0.7307 running_loss=0.0019 batch_loss=0.0076 acc=0.0307 batch_acc=0.2227
[2022-11-02 15:26:55,184][ai4sci.trainer][INFO] - [0] [0/1: 302080 / 1281167 (24%)] epoch=0.0000 dt=0.7259 running_loss=0.0020 batch_loss=0.0076 acc=0.0315 batch_acc=0.2188
[2022-11-02 15:27:18,429][ai4sci.trainer][INFO] - [0] [0/1: 307200 / 1281167 (24%)] epoch=0.0000 dt=0.7250 running_loss=0.0020 batch_loss=0.0073 acc=0.0323 batch_acc=0.2168
[2022-11-02 15:27:42,329][ai4sci.trainer][INFO] - [0] [0/1: 312320 / 1281167 (24%)] epoch=0.0000 dt=0.5822 running_loss=0.0020 batch_loss=0.0071 acc=0.0331 batch_acc=0.2383
[2022-11-02 15:28:17,371][ai4sci.trainer][INFO] - [0] [0/1: 317440 / 1281167 (25%)] epoch=0.0000 dt=0.6033 running_loss=0.0020 batch_loss=0.0074 acc=0.0340 batch_acc=0.2266
[2022-11-02 15:28:41,834][ai4sci.trainer][INFO] - [0] [0/1: 322560 / 1281167 (25%)] epoch=0.0000 dt=0.7861 running_loss=0.0021 batch_loss=0.0074 acc=0.0348 batch_acc=0.2227
[2022-11-02 15:29:08,485][ai4sci.trainer][INFO] - [0] [0/1: 327680 / 1281167 (26%)] epoch=0.0000 dt=0.6361 running_loss=0.0021 batch_loss=0.0072 acc=0.0357 batch_acc=0.2598
[2022-11-02 15:29:33,450][ai4sci.trainer][INFO] - [0] [0/1: 332800 / 1281167 (26%)] epoch=0.0000 dt=0.6638 running_loss=0.0021 batch_loss=0.0072 acc=0.0365 batch_acc=0.2148
[2022-11-02 15:29:58,425][ai4sci.trainer][INFO] - [0] [0/1: 337920 / 1281167 (26%)] epoch=0.0000 dt=0.7796 running_loss=0.0022 batch_loss=0.0073 acc=0.0374 batch_acc=0.2148
[2022-11-02 15:30:22,378][ai4sci.trainer][INFO] - [0] [0/1: 343040 / 1281167 (27%)] epoch=0.0000 dt=0.9550 running_loss=0.0022 batch_loss=0.0071 acc=0.0382 batch_acc=0.2344
[2022-11-02 15:30:47,693][ai4sci.trainer][INFO] - [0] [0/1: 348160 / 1281167 (27%)] epoch=0.0000 dt=0.7856 running_loss=0.0022 batch_loss=0.0075 acc=0.0392 batch_acc=0.1973

```
