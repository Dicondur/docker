docker version
docker info
docker run -it jboss/wildfly 

docker run -d jboss/wildfly 
docker ps
docker stop <ID/Name>


docker container ls-a
docker container run -it --name web jboss/wildfly bash
docker container rm -f <Name/ID>
docker container run -d --name web -p 3000:8080 jboss/wildfly

docker container logs <Name> -f
docker container run -d --name web -p 3000:8080 -v `pwd`/oftenUsed/CPWE:/opt/jboss/CPWE jboss/wildfly


docker container run -d --name web -p 3000:8080 -v `pwd`/CPWE:/CPWE jboss/wildfly


