<h1> Comandos docker </h1>

<h3> O que é uma imagem? </h3>
<p> A imagem no docker é um pacote leve, imutável que pode conter bibliotecas, códigos, sistemas operacionais. É a base para a construção de containers no docker.</p>

<h3> O que é um container? </h3>
<p> O container é a instancia em executação de uma imagem docker. </p>

<h3> Para o que serve o docker.file?</h3>
<p> O arquivo docker.file contém as instruções necessárias para que seja possível realizar a construção de uma imagem. </p>



<h3> Comandos gerais do docker: </h3>
<br>
<p> - Para verificar a versão instalada do docker: </p>

 ```
  docker version
  ```

<p> - Para adiciona um identificador customizado a sua imagem: </p>

 ```
  docker tag <id_da_imagem> <nome_desejado_para_imagem>:<nome_desejado_para_a_tag>
  ```

<h3> Comando em docker referênte a imagens: </h3>
<br>
<p> - Para listar todas as imagens já instaladas no computador: </p>

 ```
  docker images
  ```

<p> - Para baixar alguma imagem presente no docker hub</p>

```
  docker pull <id_da_imagem>
```

<p> - Para remover uma imagem baixada</p>

```
  docker rmi <id_da_imagem>
```

<p> O comando abaixo é capaz de construir uma imagem com base nas instruções escritas no dockerfile.</p>

```
  docker build <diretório_da_imagem>
```
<h3> Comandos em docker referente a containers: </h3>
<br>
<p> - Para iniciar um container já buildado anteriormente:</p>

```
 docker start <id_do_container>
```

<p> - Para parar um container:</p>

```
 docker stop <id_do_container>
```

<p> - Para parar um container:</p>

```
 docker stop <id_do_container>
```

<p> - Para listar container executando:</p>

```
 docker ps
```

<p> - Para listar container que já foram executados:</p>

```
 docker ps -a
```

<p> - Para executar um container em background:</p>

```
 docker run -d <id_do_container>
```

<p> - Para executar um container e expor ele a uma porta expecifica com uma porta especifica do container:</p>

```
docker run -p <numero_da_porta_a_ser_exposta_do_computador> : <numero_da_porta_a_ser_exposta_no_container> <id_do_container>
```

<p> - Para executar um container simples em modo iterativo: </p>

```
docker run -it <id_do_container>
```

<p> - Para executar um container simples em modo iterativo: </p>

```
docker run -it <id_do_container>
```

<p> - Para verificar os processos de um container em específico: </p>

```
docker top <id_do_container>
```

<p> - Para exibir os recursos sendo utilizados por um container em execução: </p>

```
docker stats <id_do_container>
```

<p> - Para exibir informações detalhadas de um container, em formato json: </p>

```
docker inspect <id_do_container>
```

<p> - Para copiar um arquivo em execução de um container: </p>

```
docker cp <id_do_containter>:/<workdir_do_container>/<arquivo_desejado> <diretório_e_arquivo_para_copia> 
```

<p> - Para exibir os logs de um container rodando: </p>

```
docker logs <id_do_container> -f
```

<p> - Para remover um container que já foi executado: </p>

```
docker rm <id_do_containter>
```

<p> - Para remover um container que está executando: </p>

```
docker rm <id_do_containter> -f
```

<p> - Para limpar os recursos que não são utilizados mais:</p>

```
docker system prune
```

