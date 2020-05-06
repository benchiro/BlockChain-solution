# ParityTechnologiesDevOpsTask
automation of the provisioning and deployment process of the substate blockchain

Starting  Node

# Purge chain cleans up any old data from running a `dev` node in the past
# You will be prompted to type `y`
./target/release/node-template purge-chain --dev

# Run your actual node in "development" mode
./target/release/node-template --dev
#software
So we should make sure that docker engine is now running for containerisation and then we install kubernetes as well for our containerisation
ochestration management and then we start to role out all the scripts that l shared for creating pods.

### Execute our deployment using YAML

To create these, we can run the command `kubectl create -f substrate-master.yml` ' kubectl create -f  substrate-telemetry-exporter-master' to create our deployment 
and it will run service as well
```
kubectl create -f helloworld-deployment.yml

Notice the `---` that marks the end of one section and starts another.

We can run the command `kubectl get all` to see all our resources running, as shown in the output below.
kubectl apply commands in order how l will deploy in the cluster

kubectl get commands

kubectl get pod
kubectl get pod --watch
kubectl get pod -o wide
kubectl get all | grep substrate-master
kubectl get all | grep substrate-telemetry-exporter-master

kubectl debugging commands

kubectl describe pod substrate-master-xxxxxx
kubectl describe service substrate-master-service
kubectl logs substrate-master-xxxxxx
kubectl describe pod substrate-telemetry-exporter-master-xxxxxx
kubectl describe service substrate-telemetry-exporter-master-service
kubectl logs substrate-telemetry-exporter-master-xxxxx



