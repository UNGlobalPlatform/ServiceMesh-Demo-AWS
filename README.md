# ServiceMesh-Demo-AWS

Add steps Demo (conncurrent load comparison)
Tutorial : https://buoyant.io/2017/01/31/making-things-faster-by-adding-more-steps/ 
 
![alt text](https://github.com/linkerd/linkerd-examples/blob/master/add-steps/add-steps.png "Overview of demo architecture")

Code: https://github.com/linkerd/linkerd-examples/tree/master/add-steps

1.get all the examples
sudo git clone https://github.com/linkerd/linkerd-examples.git
2.go to the demo we want first
cd linkerd-examples/add-steps
3. add yourself to the docker group
sudo usermod -aG docker ${USER}
4. check this worked by LOGGING OUT then log back into the server & view the users groups
groups $USER
5.Build and tag image with the version number of the source release (useful later NOT latest)
sudo docker-compose build && docker-compose up -d
6. open http://ec2-52-16-38-85.eu-west-1.compute.amazonaws.com:3000 

7. open Prometheus  http://ec2-52-16-38-85.eu-west-1.compute.amazonaws.com:9090 

8. open Linkerd http://ec2-52-16-38-85.eu-west-1.compute.amazonaws.com:9990 


