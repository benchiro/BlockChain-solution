# ParityTechnologiesDevOpsTask
automation of the provisioning and deployment process of the substate blockchain

Starting  Node

# Purge chain cleans up any old data from running a `dev` node in the past
# You will be prompted to type `y`
./target/release/node-template purge-chain --dev

# Run your actual node in "development" mode
./target/release/node-template --dev

So we should make sure that docker engine is now running for containerisation and then we install kubernetes as well for our containerisation
ochestration management and then we start to role out all the scripts that l shared for creating pods.
