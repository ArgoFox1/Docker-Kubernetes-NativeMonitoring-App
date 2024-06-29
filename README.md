## THIS PROJECT BUILDED WITH DOCKER & KUBERNETES
## DOCKER DEPLOYMENT
1-**First open the terminal**
> ctrl+alt+t

2-**Go to the project folder**
>cd/path/to/your/folder

3-**Create container**
> docker run -p 5000:5000 emirhanmetin/py-flask

4-**Check container status**
> docker ps

5**Then its gives you 2 links click these links go straight to the website**
>  * Running on http://127.0.0.1:5000
>> * Running on http://172.17.0.2:5000

## KUBERNETES DEPLOYMENT
1-**First open the terminal**
> ctrl+alt+t

2-**Go to the Kubernetes folder**
> cd path/to/your/folder

3-**Check Kubernetes status**
> minikube status

4-**If its not running start minikube**
> minikube start

4-**Then Create service object**
> kubectl apply -f monitoring-service.yaml .

**if your not in the kubernetes folder** 
>kubectl apply -f monitoring-service.yaml path/to/your/folder

5-**Check service object status**
> kubectl get service -w

6-**Check deployment object**
> kubectl get deployment -w

7-**Then run service object**
> minikube service monitor

![Screenshot from 2023-12-19 11-19-51](https://github.com/ArgoFox1/Docker-K8S-NativeMonitoring-App/assets/105239243/0bd14bb2-f115-42b0-8c07-f83cd5cfd8c4)
