##MY CKAD EXAM 16052020 notes

# 1. Network policy question:
This question has setup for you pod and network policy. You only need to view policy apply on which labels and then label the pod
For example:
There are some policy:
deny all
allow all
allow access proxy with label: proxy=true
allow access db with label: db=true

there are 3 pods:

your pod

proxy

db

Question: do not change any thing in network policy and do your pod can access proxy and db only
=> set labels db=true and proxy=true for your pod
# 2. LivenessProbe and ReadinessProbe
The question ask to add check: liveness and readiness. However, they will ask check liveness and readiness with each /path

example:

check liveness with path /started

check readiness with path /health

=> need to understand clearly the question which one apply for readiness and which one apply for liveness

# 3. Configmap and secret

this question easy

=> Let practice with configmap to present in pod:

    - present as an environment variable
    - present by loading environment file
    - present as volumes

# 4: volumes

this question need to practice:
    
    - How to mount an emty volume
    - how to create pv
    - how to create pvc
    - present volume from pvc
  
 # 5. 