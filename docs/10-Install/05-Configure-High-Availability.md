# Choosing a HA

  Take me to [Lecture](https://kodekloud.com/courses/539883/lectures/9808328)
  
#### What happens when you loose the master node in your cluster?
- You must consider multiple master nodes in a a high availability environment configuration in your prod environment.
  
  ![haa1](../../images/haa1.PNG)
  
- It is better to have a load balancer of some kind configured infront of the master nodes that split traffic between the API servers. And then point kubectl utility to that load balancer 

  ![haa2](../../images/haa2.PNG)
  
- What about the scheduler and the controller manager?

  ![haa3](../../images/haa3.PNG)
 
  ![haa4](../../images/haa4.PNG)
 
- what about the etcd? With etcd we have two topologies that we can configure in kubernetes.
  - Stacked Topology
  
    ![haa5](../../images/haa5.PNG)

  - External ETCD Topology
    ![haa6](../../images/haa6.PNG)

#### Our Lab Design

 ![haa7](../../images/haa7.PNG)

   
#### K8s Reference Docs
- https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/high-availability/
- https://kubernetes.io/docs/tasks/administer-cluster/highly-available-master/

  
