Nginx-Ingress setup on K8s
=======

Boilerplate setup for *Ingress* on *Kubernetes*. Exposes a HTTPS/HTTP **hello-world** API. The project is based on the guide given here: 
https://medium.com/@gokulc/setting-up-nginx-ingress-on-kubernetes-2b733d8d2f45

The steps described in the guide are automated using the ***deploy_to_minikube.sh*** script.

Assuming that you already have Kubectl and Minikube setup, you can simply run the script. To test the deployed the service, use the following commands: 

    curl http://api.sample.com/FooBar
    curl https://api.sample.com/FooBar -k
The certificate is self signed and hence will throw an SSL error. Bypass this using ***-k*** option of ***Curl***.


