 Kubernetes Manifest File:
 ===========================

 1. What is a Manifest File?

    A manifest file in Kubernetes is a YAML or JSON file that defines the desired state of a Kubernetes object.

    A Manifest file is a configuration file that contains instructions about how an application or service should run.

2. Why Manifest Files Are Important:

    Kubernetes is declarative.

    Instead of running many commands, you write a YAML file describing:

        Application image
        Number of replicas
        Ports
        Storage
        Configuration
        Environment variables
 
3. Basic Structure of a Manifest File
    
    apiVersion: 

    ✅ apiVersion:

        This tells Kubernetes which API version to use for that object.

        Example:

            apps/v1 → for Deployment
            v1 → for Pod, Service, ConfigMap

    kind: 

        This tells what type of Kubernetes resource you want to create.

        Example:
           Pod
            Deployment
            Service
            Namespace

    metadata:

    ✅ metadata:

        This contains the basic details like name, labels, namespace.

        It is like the identity of the resource.

    spec:

        This is the main configuration part.

        It tells Kubernetes what exactly should be created and how it should behave.
 
 kubectl apply -f filename.yaml

 Manifest removal: Manifests can be removed when you need to completely remove a resource from the node. 
 Manifest upgrade: During an application upgrade, some resources might need to be removed while others are retained to preserve data.


 example of syntax:
 ==================
```hcl
 apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deploy
spec:
  replicas: 2
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx-container
        image: nginx
        ports:
        - containerPort: 80
```