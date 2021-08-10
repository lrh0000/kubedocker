# kubedocker
Dockerize and deploy a simple app to Kubernetes

# Quickstart Guide #


### Prerequisite ###

* Python 3.7 or higher
* Docker
* Kubernetes

### Testing on local ###

Install the requirements:
```
 pip install -r requirements.txt
```
Run the app:
```
python3 app.py 
```

### Building the Docker image ###
```
docker build -f Dockerfile -t app:latest .
```

### Deploying on Kubernetes ###
```
kubectl apply -f deployment.yaml
```
Verify the service and pods are in place:

```
kubectl get services
kubectl get pods
```

### Connecting to the console ###

Open a web browser and go to the address http://localhost:5000
