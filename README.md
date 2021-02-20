## <h1>Docker</h1> 


# Docker RUN
  Comando utilizado para criar um container

```
docker run --name newcontainer hello-world
docker run --name hello -d busybox sleep 3600
docker run --name site -d -p 80:80 nginx
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
docker exec hello mkdir teste
```

# Acessando o container com o servico SH
```
docker exec -it hello sh
```
