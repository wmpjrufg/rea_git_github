---
title: Seja bem-vindo!
layout: home
nav_order: 1
---

<h1>O que vamos ver?!</h1>

<p align = "justify">
Este material tem como objetivo central oferecer aos alunos, professores e qualquer pessoa que deseja entender o funcionamento básico das ferramentas de versionamento de código. Neste caso a ferramenta empregada será o Git e GitHub.<br><br>
Este material é utilizado dentro do Grupo de Pesquisa e Estudos em Engenharia (GPEE) que é liderado pelo professor <a href="http://lattes.cnpq.br/2268506213083114" target = "_blank" rel = "noopener noreferrer">Wanderlei Malaquias Pereira Junior</a>.
<br><br>
Este material aborda os seguintes tópicos:
</p>

<table>
  <tr>
    <td style = "width:70%;">
        <ol>
            <li>Configurações e primeiros passos no versionamento</li>
            <li>Git e Git Hub na prática</li>
            <li>Boas pŕaticas</li>
            <li>Desafios</li>
        </ol>
    </td>
    <td style = "width:30%;"><center><img src = "assets/images/fig00.png" width = "60%"></center></td>
  </tr>
</table>


<h1>O conceito de controle de versão</h1>

<p align = "justify">
O Git é um <i>software</i> de gerenciamento de versão em documentos. Essa temática é um braço da engenharia de <i>software</i> que consiste em uma junção de técnicas para rastrear e controlar alterações sobre um código ou conjunto de códigos.
<br><br>
Um controle de versão simplificado poderia ser por representado por um usuário mudando o nome do arquivo a medida que o mesmo fosse alterado.
</p>

<p align = "justify">

O controle de versão (como o Git) é essencial em um repositório de software porque ele resolve vários problemas fundamentais do desenvolvimento. Pois,  pode-se ver quem fez o quê, quando, e por quê, sendo portanto, útil para 
encontrar erros introduzidos em alterações passadas, reverter para versões anteriores e acompanhar o progresso e a evolução do projeto. 

Além disso, o controle de versão permite que várias pessoas trabalhem no mesmo código ao mesmo tempo, pois cada pessoa pode ter sua própria branch (ramo), evitando sobrescrever o trabalho dos outros, mas tambem mesclar as alterações quando necessário

Com relaçao segurança, com o repositório salvo no Git (e idealmente em um serviço como GitHub/GitLab), se alguém apagar um arquivo acidentalmente, é fácil recuperar

Se o projeto apresentar falha após uma alteração, pode voltar para uma versão que funcionava anteriormente, pois  o código fica salvo remotamente, como um backup.
<br><br>

Outro aspecto importante é referente a rastreabilidade.  É possível ver as diferenças entre versões (git diff), podendo associar cada atualização a um issue ou pull request.
</p>





<p align = "justify">
A <a href = "#fig01">Figura 0.1</a> apresenta algumas ferramentas que controlam a revisão de código.
</p>

<table>
<thead>
  <tr>
    <td><center><img src="assets/images/fig01.png" width="60%"></center></td>
    <td><center><img src="assets/images/fig02.png" width="60%"></center></td>
    <td><center><img src="assets/images/fig03.svg" width="600%"></center></td>
  </tr>
</thead>
</table>
<p align = "left" id = "fig01"><b>Figura 0.1</b> Plataformas de controle de versão.</p>

<h1>O que é Git e por que ele é usado?</h1>

<p align = "justify">
Git é um sistema de controle de versão distribuído, e serve para facilitar a edição do código-fonte de um projeto por múltiplos usuários de forma simultânea sem que as alterações sobrescrevam outras, e caso haja edições no mesmo local de um repositório (nome dado ao diretório de um projeto), por exemplo, o controle de versão armazena todo o histórico de alterações, sendo possível retornar à versão anterior do projeto, ou seja, à última vez em que ele foi salvo. Além disso, é possível saber que alterações foram feitas no projeto e por quem, o que facilita o controle.
</p>

{: .note }
> Git e GitHub são conceitos diferentes. O GitHub é uma plataforma <i>web</i> que utiliza a o Git como <i>framework</i> controlador de versão.

<p align = "justify">
Vamos iniciar este material pela instalação dos recursos necessários para uso do Git em um computador seja ele Linux ou Windows. Vamos instalar os seguintes programas:<br>
</p>

<ol>
    <li><a href = "https://git-scm.com/">Plataforma Git</a>;</li>
    <li><a href = "https://code.visualstudio.com">Visual Studio Code</a>;</li>
</ol>

<p align = "justify">
Após a instalação é necessário criar uma conta no repositório <i>online</i> <a href = "https://github.com/">GitHub</a>.
</p>

{: .highlight-title }
> Testando o git
>
> Para verificar se o git foi instalado corretamente. Reinicie o computador vá até o terminal do seu computador e digite o seguinte comando: `git --version`.Provavelmente após a execução aparecerá no terminal a versão do git, por exemplo: `git version 2.34.1`.

<p align = "justify">
Após o comando mostrado acima você pode verificar se o Git foi instalado corretamente no Visual Studio Code conforme a <a href = "#fig02">Figura 0.2</a>. Caso o símbolo de árvore de arquivos esteja presente a instalação foi bem sucedida.  
</p>

<center><img src = "assets/images/fig04.png" width = "100%"></center>
<p align = "left" id = "fig02"><b>Figura 0.2</b> Árvore de arquivos controlados pelo Git no Visual Studio Code.</p>
