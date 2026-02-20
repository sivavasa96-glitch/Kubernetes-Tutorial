 Kubernetes Manifest File:
 ===========================

 1. What is a Manifest File?

    A manifest file in Kubernetes is a YAML or JSON file that defines the desired state of a Kubernetes object.

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

    kind: 

    metadata:
    
    spec:
 
