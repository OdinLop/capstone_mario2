# capstone_mario2
Second repo, has code to deploy into the EKS cluster
To run in local, run these commands in order in a terminal, make sure to have Docker Desktop running with WSL2 activated and Kubernetes Running as well
Pull this repo inside your terminal in a Linux Directory and run the following commands in order
First: kubectl apply -f deployment.yaml #to deploy the kubernetes cluster with the images
Second(Optional): kubectl get deployments #to verify everything deployed correctly
Third: kubectl apply -f ingress.yaml #to create the service that exposes the deployment to the internet
Fourth: kubectl get service mario-service #to get the IP to access our game! Look for EXTERNAL-IP