# API priority & Fairness watch experiments


## Cluster sizing

The experiment was performed in a AWS based cluster with:

3x m5.xlarge (4 vCPU + 16 GiB)
3x m5.large worker nodes: (2 vCPU + 8 GiB)


## Metrics

- Count watches per kube-apiserver instance: `sum(apiserver_registered_watchers{apiserver="kube-apiserver"}) by (instance,apiserver)`
