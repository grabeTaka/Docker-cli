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



