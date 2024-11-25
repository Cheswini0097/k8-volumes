
#EFS volume kuberenetes configuration Static

 Create  the efc the vpc network
 Install the CSI deivers,
 latest release is 

```
kubectl kustomize \
    "github.com/kubernetes-sigs/aws-efs-csi-driver/deploy/kubernetes/overlays/stable/?ref=release-2.1" > public-ecr-driver.yaml
``` 
 file will be created under the name " public-ecr-driver.yaml"

 ```
 kubectl apply -f public-ecr-driver.yaml
 ```
#Install drivers and allow traffic  2049 from worker node
 # give permission for the Eks nodes from iam role;



#Kuberenetes-volume

command to check the pv (persistant volume)

```
Kubectl  get pv
```
command to describe the pv

```
kuctl describe pv
```
command to check the pvc

```
Kubectl get pvc
```

command to list the pvc
```

Kubectl get pvc


