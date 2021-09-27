# azuredevops-buildagent

1) Buildear la imagen con build.sh
2) Para customizar el agente editar el Dockerfile
3) Especificar el agent pool y el AZP Token dentro de deploy_agent.sh
4) Deployar el agente ejecutando deploy_agent.sh


# Se pueden agregar referencias a hosts de la misma red de la siguiente manera.

Se pude editar el build.sh de la imagen y agregar host en este caso por ejemplo a un host con sonarqube.

docker build --add-host=sonarqube.internal:192.168.100.135 -t azuredevops-dockeragent:latest .
