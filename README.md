A VPC with EC2 with custom kubernetes installed and set.
and ever deployment is docrized and pushed to docker and 
then deployed into the already set up k8s cluster with 3
replicas and rolling deployment. I is only a staic angular page

- infrastructure is created using cloudformation scripts
 which are in the folder /aws
- few steps in   Kubernetes cluster initialization were done 
manually as this was first attemp at setting up and needed debugging (not a repetative task anyway)
- Dockerfile is in frontend (only frondend folder needs actual deployment)
- not creating new ec2 on deployment, but creating VMs on the same machine for cost reasons
 you can see pods being terminated / created in screenshot rolling.png
 And you can see the service my-service as load balance in screenshot my-service
- application accessable on 
http://ec2-3-127-223-111.eu-central-1.compute.amazonaws.com:31324/
