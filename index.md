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

Outro aspecto importante é referente a rastreabilidade.  É possível ver as diferenças entre versões (git diff), podendo associar cada atualização a um issue ou pull request, o que permite aos membros das equipes de desenvolvimento, exercerem um trabalho remoto e desempenhar um trabalho off-line (em sua cópia local), sendo necessário a conexão para enviar suas mudanças (push/pull)
</p>


<p align = "justify">
A <a href = "#fig01">Figura 0.1</a> apresenta algumas ferramentas que controlam a revisão de código.
</p>

<table>
<thead>
  <tr>
    <td><center><img src="assets/images/fig01.png" width="60%"></center></td>
    <td><center><img src="assets/images/fig02.png" width="60%"></center></td>
    <td><center><img src="assets/images/fig03.svg" width="60%"></center></td>
  </tr>
</thead>
</table>
<p align = "left" id = "fig01"><b>Figura 0.1</b> Plataformas de controle de versão.</p>

<h1>O que é Git e GitHub?</h1>

<p align = "justify">
Git é um sistema de controle de versão distribuído, e serve para facilitar a edição do código-fonte de um projeto por múltiplos usuários de forma simultânea sem que as alterações sobrescrevam outras, e caso haja edições no mesmo local de um repositório (nome dado ao diretório de um projeto), por exemplo, o controle de versão armazena todo o histórico de alterações, sendo possível retornar à versão anterior do projeto, ou seja, à última vez em que ele foi salvo. Além disso, é possível saber que alterações foram feitas no projeto e por quem, o que facilita o controle.
  
Considere como exemplo o Google Docs, mas para código, onde é possível: visualizar o histórico completo, voltar para versões antigas e criar "cópias" (branches) para testar uma nova funcionalidade, por exemplo.

 Git e GitHub são conceitos diferentes. O GitHub é uma plataforma online que utiliza repositórios Git na nuvem como controlador de versão e permite e colabora com outras pessoas. No GitHub é possível armazenar seu código versionado com Git, compartilhar projetos com outras pessoas, trabalhar em equipe com controle de acesso, fazer pull requests, revisar código, automatizar testes, etc.

Existem outras plataformas similares, como:
- GitLab
- Bitbucket
- Azure DevOps

A Tabela a seguir, apresenta as principais diferenças entre os dois conceitos:
 <table>
  <tr>
    <th>Git</th>
    <th>GitHub</th>
  </tr>
  <tr>
    <td>Programa Local</td>
        <td>Plataforma online </td>

  </tr>
  <tr>
    <td>Salva e controla versões</td>
        <td>Hospeda os repositórios Git </td>

  </tr>
  <tr>
    <td>Funciona offline</td>
        <td>Funciona na web</td>

  </tr>
  <tr>
    <td>Ferramenta de desenvolvedor</td>
    <td>Interface gráfica + colaboração online</td>
  </tr>
 
</table>



Exemplo básico:<br></br>
git init                     # Inicia um repositório Git local <br></br>
git remote add origin https://github.com/usuario/repositorio.git<br></br>
git add .                    # Adiciona todos os arquivos<br></br>
git commit -m "primeiro commit"<br></br>
git push -u origin main      # Envia para o GitHub<br></br>

</p>
<p align = "justify">

Assim, com as duas plataformas trabalhando em cojunto, é possível usar o Git no computador para controlar seu código e em sequência, enviar esse código para o GitHub para backup e colaboração.

PRÉ-REQUISITOS
- Ter o Git instalado     <li><a href = "https://github.com">Plataforma Git</a></li>
- Ter uma conta no GitHub
- Ter um projeto local (ou pode criar uma pasta de teste)
</p>


<p align = "justify">
Em sequência, vamos iniciar este material pela instalação dos recursos necessários para uso do Git em um computador seja ele Linux ou Windows. Vamos instalar os seguintes programas:<br>
</p>

<ol>
    <li><a href = "https://git-scm.com/">Plataforma Git</a>;</li>
    <li><a href = "https://code.visualstudio.com">Visual Studio Code</a>;</li>
</ol>

<h1>Instalando o Git no Windows</h1>

A seguir, é descrito os principais para a instalaçao do git:

1- Acesse: https://git-scm.com/download/win para fazer o download do instalador

2- Execute o instalador (.exe).


3- Durante a instalação, deixe as opções padrão, exceto quando aparecer "Choose the default editor used by Git", que pode ser por exemplo:
 Visual Studio Code software.
 4- Na opção "Adjusting your PATH environment", escolha: "Git from the command line and also from 3rd-party software" 



4- Finalize a instalação.


5- No terminal do computador, verifique se o git foi instalado corretamente: 
$ git --version

Deve retornar algo como: git version 2.xx.x



<p align = "justify">
Após a instalação é necessário criar uma conta no repositório <i>online</i> <a href = "https://github.com/">GitHub</a>.
Após a criação do login, você pode configurar seu nome e email para usar com Git/GitHub:
$ git config --global user.name "Seu Nome"
$ git config --global user.email "seu@email.com"
</p>
<p align = "justify">

<h1>Instalando o GitHub no VSCode</h1>
<p align = "justify">

É possível acessar o GitHub diretamente a partir do IDE. Em particular, serão mostrados os passos necessários para configurar o GitHub no VSCode.
1- Instalar o Visual Studio Code no Windows: https://code.visualstudio.com/
2- Clique em Download for Windows ou macOS.
3- Execute o instalador:
4- No Windows, marque a opção "Add to PATH" e "Register Code as editor".
5- Após instalar, abra o VSCode.
6- Vá até a aba de extensões (ícone de quadrado no menu lateral esquerdo ou Ctrl+Shift+X)
7- Procure por GitHub e instale: GitHub Pull Requests and Issues (oficial da Microsoft)
8- Opcional: GitLens (melhora a visualização do histórico Git)
</p>
<p align = "justify">

  Ao usar o Git pela primeira vez  no VSCode:
1- Abra o terminal do VSCode (Ctrl+`` ou Terminal > New Terminal`)
2- Tente um comando Git, por exemplo: git clone https://github.com/seu-usuario/seu-repo.git
3- Se for sua primeira vez, o VSCode vai abrir uma janela solicitando que você faça login com sua conta GitHub
4- Autorize o VSCode a acessar seu GitHub
</p>
<p align = "justify">
Após o comando mostrado acima você pode verificar se o Git foi instalado corretamente no Visual Studio Code conforme a <a href = "#fig02">Figura 0.2</a>. Caso o símbolo de árvore de arquivos esteja presente a instalação foi bem sucedida.  
</p>

<center><img src = "assets/images/fig04.png" width = "100%"></center>
<p align = "left" id = "fig02"><b>Figura 0.2</b> Árvore de arquivos controlados pelo Git no Visual Studio Code.</p>


<p align = "justify">
  Assim,  a integração ativa é possível 
ver branches, commits e diffs no painel Source Control (ícone de ramificação), fazer commits, pull, push, tudo pelo VSCode. Além disso, pode-se criar e revisar pull requests (com a extensão GitHub), resolver conflitos visuais entre branches e por fim, visualizar quem alterou cada linha de código (com GitLens)
</p>
