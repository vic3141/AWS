# AWS
## What is cloud computing
- cloud computing is the delivery of computing services including servers,storage,databases,networking,software etc.
## benfits 
- faster time to market
- scalability and flexibility
- cost savings
- better collaboration
- advanced security
- data loss prevention
## disadvantage 
- risk of vendor lock-in
- less control over underlying cloud insfra
- concerns about security risks like data privacy and online threats
- integration complexity with exisiting systems
- unforseen costs and unexpected expenses

![image](https://github.com/vic3141/AWS/assets/143579487/db4864e1-8745-4611-827a-521214c9bd99)

![image](https://github.com/vic3141/AWS/assets/143579487/2f722b21-8ee7-4410-8855-f56fb112cd31)

- example of private implementation softwares : openstack , opennebula

## Hyperscalars : A hyperscaler is a type of large-scale data center that offers massive computing resources, typically in the form of an elastic cloud platform. Organizations use them to deploy and manage large-scale applications and services.

![image](https://github.com/vic3141/AWS/assets/143579487/eee1f7c7-7d8a-41bd-ad85-243d0951a40c)

![image](https://github.com/vic3141/AWS/assets/143579487/2142280c-b78f-4b1d-85a5-4c5732ec4723)

## Compute services 
- EC2  
- ECS/EKS : containerized services `
  - Fargate
- lambda : serverless 

## Storage Services
- S3
- EBS : Amazon Elastic Block Storage is a storage service wherein each block of storage acts like a separate hard drive (volume) . 
- EFS : dont need to assign any volume , can do on its own , seamless storage , database on EC2 instances 
- Archival service - Glacier : Amazon Glacier is extremely low cost, secure, and durable storage service for data archiving and
backup. That data stored which are not needed instantly , eg old data . Takes time min 4 hours or 1 day to retrieve request ( S3 instantly returns request)

## Network Services
- VPC : own insolated environment in a public cloud
- Domain Name Service - Route 53

![image](https://github.com/vic3141/AWS/assets/143579487/8c3f990c-f288-43ba-bd9e-c572f5f33315)

- public subnet : can receive traffic from outerworld 
- private subnet : cannot receive traffic from outerworld but may or may not send traffic to outerworld

![image](https://github.com/vic3141/AWS/assets/143579487/c066d6c6-851e-4954-bade-f45341184e47)
![image](https://github.com/vic3141/AWS/assets/143579487/d9ea1371-4c64-4d0f-8a5f-814749db652e)


![image](https://github.com/vic3141/AWS/assets/143579487/1c87954f-a235-467a-b769-7baeb93d1a98)
![image](https://github.com/vic3141/AWS/assets/143579487/e07ca403-79c9-49b7-9dfa-1c58197ac7e2)
![image](https://github.com/vic3141/AWS/assets/143579487/7de933b4-58a8-4c35-9864-d2f105073529)

![image](https://github.com/vic3141/AWS/assets/143579487/49e0f0a8-d001-44e2-b37c-3bbd11342180)
![image](https://github.com/vic3141/AWS/assets/143579487/22c3bc38-b29b-4df6-8a9a-d61a0e3cde96)

- **Apache web server works on layer 7 , using single apache server one can deploy multiple applications on different ports based on paths (URLbased) (virtual hosts) . virtual hosting can only work on layer 7**

## Application based LB 
- key pair : kind of like a password (public key is username; private key is password)
  - PPK (PuTTY Private Key) and PEM (Privacy Enhanced Mail) are two file formats that are commonly used for SSH and SSL/TLS connections. While PPK files are primarily used with PuTTY on Windows, PEM files are more widely supported and can be used with various tools and platforms

- security groups : A security group controls the traffic that is allowed to reach and leave the resources that it is associated with. For example, after you associate a security group with an EC2 instance, it controls the inbound and outbound traffic for the instance. When you create a VPC, it comes with a default security group. (acts as a firewall)

![image](https://github.com/vic3141/AWS/assets/143579487/20a849fc-c635-47ff-989b-a94fb441e9d1)

![image](https://github.com/vic3141/AWS/assets/143579487/d2481142-8ee1-42a8-86a3-d35902f76f9b)

![image](https://github.com/vic3141/AWS/assets/143579487/87b9cbed-5b4d-460f-a2cf-928c308597de)

![image](https://github.com/vic3141/AWS/assets/143579487/1790d0be-d703-43e1-b17b-bbb776b2acd6)

### Creating a target group 
- Your load balancer routes requests to the targets in a target group and performs health checks on the targets.
- LB routes traffic to target group then traffic group routes traffic to the back end ec2 instances or IP addresses etc

![image](https://github.com/vic3141/AWS/assets/143579487/042ae8ef-3b6f-4484-8f13-e47b5178222f)
![image](https://github.com/vic3141/AWS/assets/143579487/5b2aad79-4cef-4e6a-a6d6-b7768230933d)
![image](https://github.com/vic3141/AWS/assets/143579487/76a0fec4-374e-450e-9dfc-0359e0e94be9)
![image](https://github.com/vic3141/AWS/assets/143579487/dd34166d-6c25-4485-a300-776e886f6224)
![image](https://github.com/vic3141/AWS/assets/143579487/561e46b6-d844-4692-99da-1ee972ce0f97)

### Autoscalling

![image](https://github.com/vic3141/AWS/assets/143579487/193c7b8d-033f-4ded-a019-982dd93337b0)

### Creating launch template

![image](https://github.com/vic3141/AWS/assets/143579487/8841b94c-3fa5-414e-9c66-084208680df3)
![image](https://github.com/vic3141/AWS/assets/143579487/bda7bcb4-519f-4eb0-9bd7-13fa4ec827a9)
![image](https://github.com/vic3141/AWS/assets/143579487/3ee3ed76-97e3-4fc4-8a58-36a47bb3cc82)
![image](https://github.com/vic3141/AWS/assets/143579487/04724b02-0c5c-47d4-8763-c03d6750729f)
![image](https://github.com/vic3141/AWS/assets/143579487/2bbd03f1-d5ad-4efc-a2dd-4bd625e9d52c)
![image](https://github.com/vic3141/AWS/assets/143579487/5c48cb8b-46c6-4274-8596-6da8dbdbe6e5)
![image](https://github.com/vic3141/AWS/assets/143579487/29defef4-3ee2-40d8-a433-64a16f3551e7)

### Creating scalling policies

![image](https://github.com/vic3141/AWS/assets/143579487/0446a577-c5a5-4a00-9b41-b1df4e080dbc)
![image](https://github.com/vic3141/AWS/assets/143579487/1f423358-ae9d-4519-99b8-5d64879b95c9)

### Artificial load
```bash
htop
```
![image](https://github.com/vic3141/AWS/assets/143579487/0255232c-f618-4592-949e-a913a04b72ff)

- currently 0
- making instance count to a high number

```bash
seq 999999999999999999 > /dev/null &
```

![image](https://github.com/vic3141/AWS/assets/143579487/4ab31172-f726-4a7f-b74e-7f5bcee20cc6)

![image](https://github.com/vic3141/AWS/assets/143579487/0f73db76-3228-4aee-ad33-b56acbe1f395)
![image](https://github.com/vic3141/AWS/assets/143579487/75691161-21ec-4cec-9a1a-cd4a887b8b84)
![image](https://github.com/vic3141/AWS/assets/143579487/347c1440-1121-4d8e-ac67-563964073f24)

- going to the DNS name and reloding will take you to diff targets(3)
- this is **Round Robin** at work

## AWS CLI : The AWS Command Line Interface (AWS CLI) is a unified tool to manage your AWS services. With just one tool to download and configure, you can control multiple AWS services from the command line and automate them through scripts.
- BOTO library in python

![image](https://github.com/vic3141/AWS/assets/143579487/d2270331-32f1-4fa6-986e-2d1f4f37e682)
![image](https://github.com/vic3141/AWS/assets/143579487/a4f325b9-621f-4383-9fde-06104b5767fc)

```bash
sudo snap install aws-cli
```

```bash
aws configure
```

![image](https://github.com/vic3141/AWS/assets/143579487/cb9d0c94-436d-4507-9047-4c080650d766)

- in security credentials, before creating access keycopy and paste PU, PrK and fill location and format in terminal
- give user access

![image](https://github.com/vic3141/AWS/assets/143579487/e44b04d6-f774-49ba-ab79-9dda2df6c123)

![image](https://github.com/vic3141/AWS/assets/143579487/2f0fd436-65e1-4478-8800-07045e8fa359)
![image](https://github.com/vic3141/AWS/assets/143579487/297cb8e6-0979-4892-8d26-2b466a5cd361)

- after creating instance

```bash
aws ec2 describe-instances
```

![image](https://github.com/vic3141/AWS/assets/143579487/beec9fe6-fc62-4bc1-b956-32b8692e00df)
![image](https://github.com/vic3141/AWS/assets/143579487/682f7908-4202-4188-ad06-c7db1c7e09c6)
![image](https://github.com/vic3141/AWS/assets/143579487/1ff58629-32ff-48b3-8d1c-b437542949db)
![image](https://github.com/vic3141/AWS/assets/143579487/692d3890-e463-488c-9769-f01210dd63aa)

![image](https://github.com/vic3141/AWS/assets/143579487/e4ffb1ae-65ca-4281-a1b5-d802f580ee1b)
![image](https://github.com/vic3141/AWS/assets/143579487/0919fe4f-9cf4-435b-a1f0-bb6cadad529d)
![image](https://github.com/vic3141/AWS/assets/143579487/9989c440-33db-4fbf-be0d-2039a27cb6cd)
![image](https://github.com/vic3141/AWS/assets/143579487/80f014d1-790c-4a9b-bd31-3b33caea0b4c)

- docker image to create art load
- pods : Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. A Pod (as in a pod of whales or pea pod) is a group of one or more containers, with shared storage and network resources, and a specification for how to run the containers.

![image](https://github.com/vic3141/AWS/assets/143579487/d58730fa-cff1-4b82-90b0-f1c92c7daff4)

- daemon sets : works on nodes where pods are running , can manage all your agents eg if we are runninf 5 ec2 instances behind the k8s cluster then we can run 1 daemon set and that daemon set wil take care of all the agents 

## CLOUD 9
- cloud based IDE (vscode , pycharm etc)
- provides IDE on browsers

![image](https://github.com/vic3141/AWS/assets/143579487/5ce3ccb5-cc03-4de8-a5e7-bdd780a08ce2)
![image](https://github.com/vic3141/AWS/assets/143579487/af8c4a85-5348-40e9-b818-d68c277d8f67)
![image](https://github.com/vic3141/AWS/assets/143579487/f7c245d0-24cc-4df3-892f-5357878749e1)

- after confiugring aws cli on cloud 9 (scroll up) 
-  configure EKS ctl and kubectl [link for installation](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/setting-up-eksctl.html)

![image](https://github.com/vic3141/AWS/assets/143579487/6fad48a9-c456-4cf1-8d97-143eb0ad0369)

- Lauching a cluster

```bash
  eksctl create cluster --name test --version 1.28 --nodegroup-name ng.default --node-type t3.micro --nodes 2 --managed
```

![image](https://github.com/vic3141/AWS/assets/143579487/b20bc77c-86a5-4462-851e-749ab88cae84)

- yaml file for nginx container launched with official nginx image
  ``` bash
     apiVersion: apps/v1
  kind: Deployment
  metadata:
      labels:
          environment: test
      name: test
  spec:
      replicas: 1
      selector:
          matchLabels:
               environment: test
      template:
          metadata:
              labels:
                  environment: test
          spec:
              containers:
              - image: nginx:1.16
                name: nginx

  ```
``` bash
  nano nginx-deployment.yaml
```
- kubectl is the thing using which we will be creating , launching the resources , creating pods , troubleshooting cluster using kubectl
- we will apply this file using kubectl
  ``` bash
    kubectl apply -f nginx-deployment.yaml
  ```

  ![image](https://github.com/vic3141/AWS/assets/143579487/994dd934-50c5-459b-882e-cead84878421)

- to see pods used by kubectl

![image](https://github.com/vic3141/AWS/assets/143579487/d052d667-04f9-45d5-b105-79e57cf8d7fd)

- autoscaler used by eks

![image](https://github.com/vic3141/AWS/assets/143579487/52b1b093-d44c-4f50-b537-7ff8fa862180)

- can scale it

![image](https://github.com/vic3141/AWS/assets/143579487/6134157f-bc57-494b-b52e-625c4110014c)

- install matrix server , will continue to moniter the cpu matrix ,without this will not show how much resources are utilised 
``` bash
kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
```

- creating php-apache autoscaling yaml file for horizontal pod autoscaling
  ``` bash
  apiVersion: apps/v1
  kind: Deployment
  metadata:
    name: php-apache
  spec:
    selector:
      matchLabels:
        run: php-apache
    template:
      metadata:
        labels:
          run: php-apache
      spec:
        containers:
        - name: php-apache
          image: registry.k8s.io/hpa-example
          ports:
          - containerPort: 80
          resources:
            limits:
              cpu: 500m
            requests:
              cpu: 200m
  ---
  apiVersion: v1
  kind: Service
  metadata:
    name: php-apache
    labels:
      run: php-apache
  spec:
    ports:
    - port: 80
    selector:
      run: php-apache
  ---
  
  apiVersion: autoscaling/v1
  kind: HorizontalPodAutoscaler
  metadata:
    name: php-apache
    namespace: default
  spec:
    scaleTargetRef:
       apiVersion: apps/v1
       kind: Deployment
       name: php-apache
    minReplicas: 1
    maxReplicas: 10
    targetCPUUtilizationPercentage: 50
  ```

```  bash
nano hpa.yaml
```
- deploying
  ``` bash
  kubectl apply -f hpa.yaml
  ```

![image](https://github.com/vic3141/AWS/assets/143579487/6150163a-9fc5-40f9-bc4a-ace95374b845)
![image](https://github.com/vic3141/AWS/assets/143579487/49bf486b-0cb7-4462-b2d4-229fc50c761b)

- artificial load
  ``` bash
  kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"
  ```

- creating a load balancer type service
  
![image](https://github.com/vic3141/AWS/assets/143579487/0de5b105-5648-4b42-a724-efa8bc8a081c)

https://kubernetes.io/docs/tasks/access-application-cluster/create-external-load-balancer/

- creating nodeport service

![image](https://github.com/vic3141/AWS/assets/143579487/d056ef30-5cef-44b5-b4e2-ced9748c6978)
![image](https://github.com/vic3141/AWS/assets/143579487/d5f9249b-9b50-43ae-a21f-f64961a9b029)

![image](https://github.com/vic3141/AWS/assets/143579487/0b5d45ba-0997-42b7-94a9-073260c4abaf)

#EKS

![image](https://github.com/vic3141/AWS/assets/143579487/10c05b97-78f2-49d5-ba95-9deccb681e8b)
![image](https://github.com/vic3141/AWS/assets/143579487/671962db-b276-4113-834d-892cade22607)
