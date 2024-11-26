<p align=center> <img src="FedSemHAR.png" width = 80%/> </p>


<p align="center"><em>FedSemHAR: Personalized Federated Learning for Semantic Human Activity Recognition </em></p>



## BASELINE (<a href="https://cheng-haha.github.io/papers/ProtoHAR_Prototype_Guided_Personalized_Federated_Learning_for_Human_Activity_Recognition.pdf">paper</a>)
<p align=center> <img src="visual abstract.png" width = 80%/> </p>


## Benchmark
We offer a benchmark for [USC-HAD](https://sipi.usc.edu/had/) and [HARBOX](https://github.com/xmouyang/FL-Datasets-for-HAR). 


1. git clone the repo

2. Download USC-HAD and HARBOX datasets to raw data directory.

3. Generate heterogeneous data sets



**NOTE**:`args.dataset_dir = {your dataset path}`


```
python  data/uschad/uschad_subdata.py --dataset_dir /data/har/raw/USC-HAD/
python  data/harbox/harbox_subdata.py --dataset_dir /data/har/raw/large_scale_HARBox/
```
4. Usage
````
bash runexp.sh
````

## Run details 
1. USC-HAD has 14 clients, HARBOX has 120 clients
2. the learning rate of USC is 0.001, HARBOX:0.01
