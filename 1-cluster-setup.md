

# Prerequisites

An OpenShift (OCP) 4.12 (or later) Cluster with access to to Nvidia A10G GPUs (i’m using ROSA based out of eu-central-1) which makes those GPUs available with the g5.8xlarge instance types.

**Warning - these GPU instance types are expensive - so be sure to take care in how long you have them running.**


# Setup

Either on the OCP Machinesets screen or in your [https://console.redhat.com/openshift](https://console.redhat.com/openshift) account, add two g5.8xlarge nodes to your cluster as shown


## Console.redhat.com

If you have a ROSA cluster, open it and add a Machine Pool as shown
![alt_text](images/image1-a-10-g-machine-pool.png "image_tooltip")



## Directly add a Machineset

If your cluster is not contriolled from console.redhat.com, you directly add a machineset of this type and scale it to 2 - [as described here](https://docs.openshift.com/container-platform/4.14/machine_management/creating-infrastructure-machinesets.html). i.e. on this screen



![alt_text](images/image2-a-10-g-machine-sets.png "image_tooltip")



# Steps
