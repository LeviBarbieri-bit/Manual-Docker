
<p align="center">
  <img height="300" src="readme/img/logo.png" >
</p>

<p>
  Docker é um conjunto de plataforma de serviços que precisam de recursos de maquinas virtuais  utilizando sistema operacional para entregar software em pacotes chamados contêineres. 
 Docker é meio de criar arquiteturas incríveis, repleta de tecnologias.
</p>


# Docker RUN
  Comando utilizado para criar um container

```
docker run --name newcontainer [name_container]
docker run --name [name_container] -d busybox sleep 3600
docker run --name [name_container] -d -p 80:80 nginx
```

# Docker PS
Lista os container em execução, para listar os que não estão precisamos colocar o parâmetro -a
```
docker ps -a
```
# Docker INFO
Exibe um sumuário dos nossos container, como também especificações do nosso docker
```
docker info
```
# Docker EXEC
Adiciona um processo a mais no container
Vamos criar uma pasta dentro do container
```
docker exec [name_container] mkdir [diretorio]
```

# Acesso ao container com o serviço SH
```
docker exec -it [name_container] sh
```
# Docker STOP, START
Parar Container
```
docker stop [name_container]
```
Iniciar Container

```
docker start [name_container]
```
# Docker LOGS
Coletar o output do container, ótimo para debugar uma aplicação
```
docker logs [name_container]  
```

