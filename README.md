<h1>questoes-da-prova2</h1>



<h2>Introdução ao GitHub</h2>

## O que é GitHub?
O GitHub é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo12. Em resumo, o GitHub é um serviço baseado em nuvem que hospeda um sistema de controle de versão chamado Git. Isso significa que os desenvolvedores podem colaborar e fazer mudanças em projetos compartilhados enquanto mantêm um registro detalhado do progresso.

## História e evolução do GitHub
O **GitHub** foi desenvolvido por Chris Wanstrath, J. Hyett, Tom Preston-Werner e Scott Chacon usando Ruby on Rails e começou em fevereiro de 2008. A empresa, GitHub, Inc., existe desde 2007 e está localizada em São Francisco. Desde então, o GitHub se tornou uma plataforma essencial para colaboração e hospedagem de código-fonte com controle de versão usando o **Git**. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou **Open Source** de qualquer lugar do mundo. Além disso, o GitHub é amplamente utilizado por programadores para divulgação de seus trabalhos ou para que outros programadores contribuam com o projeto. Ele promove fácil comunicação através de recursos como relatórios de problemas e solicitações de pull. Atualmente, o GitHub abriga mais de 100 milhões de projetos, incluindo alguns conhecidos mundialmente, como WordPress, GNU/Linux, Atom e Electron.


## Principais funcionalidades e benefícios
Controle de Versão Distribuído: Construído sobre o Git, o GitHub permite rastrear mudanças no código, reverter para versões anteriores e colaborar eficientemente.
Hospedagem de Repositórios: Você pode criar repositórios públicos ou privados para armazenar seu código-fonte e facilitar o compartilhamento e a colaboração.
Colaboração: Múltiplas pessoas podem trabalhar juntas em um projeto, criando ramificações para desenvolver recursos separadamente e mesclando-os quando prontos.
Relatórios de Problemas e Solicitações de Pull: Usuários podem relatar problemas e enviar solicitações de pull para propor alterações no código.
Integração com Ferramentas: O GitHub se integra a várias ferramentas de desenvolvimento.
GitHub Pages: Permite hospedar sites estáticos diretamente de seus repositórios.

<h3>Configuração Inicial</h3>

## Criando uma conta no GitHub:

  - Acesse o site do GitHub.
  - Clique em “Sign up” (ou “Inscreva-se”) e siga as instruções para criar sua conta.
  - Verifique seu e-mail para confirmar o cadastro.

## Instalando o Git e configurando no GitHub:
 - Instale o Git em seu computador. Você pode baixá-lo em [git-scm.com](https://git-scm.com/).
-Abra o terminal (ou prompt de comando) e configure seu nome de usuário e e-mail globalmente com os seguintes comandos:

```
$ git config --global user.name "Seu Nome"
```
```
$ git config --global user.email "seu@email.com"
```

## Primeiros passos: criando e clonando repositórios:

- Crie um novo repositório no GitHub clicando em “New” (ou “Novo”).
- Dê um nome ao repositório, escolha a visibilidade (público ou privado) e clique em “Create repository” (ou “Criar repositório”).
- Para clonar um repositório existente, copie o link do repositório no GitHub e execute o seguinte comando no terminal:
```
$ git clone <link-do-repositório>
```
<h4>Comandos Básicos do Git</h4>

##Estrutura de um Repositório Git

Um repositório Git é uma estrutura que armazena seu código-fonte e histórico de versões. Ele consiste em três áreas principais:
- Diretório de Trabalho (Working Directory): É onde você edita e cria arquivos do seu projeto os arquivos aqui não estão rastreados pelo Git.

- Índice (Staging Area): Também conhecido como área de preparação, aqui você seleciona quais mudanças deseja incluir no próximo commit e os arquivos adicionados ao índice estão prontos para serem confirmados.

-Histórico de Commits (Branches): O Git mantém um histórico de todas as versões do seu projeto, cada commit representa um estado específico do código e os commits formam uma sequência linear ou ramificada (branches).

## Iniciando um Repositório

-Instale o Git:
Baixe e instale o Git em seu computador

- Configuração Inicial: Configure seu nome de usuário e endereço de e-mail globalmente:
```
$ git config --global user.name "Seu Nome"
```
```
$ git config --global user.email "seu@email.com"
```
-Crie um Repositório: Navegue até o diretório do seu projeto usando o terminal e execute o comando git init para iniciar o rastreamento do repositório:
```
$ git init
```
-Adicione Arquivos ao Índice: Use git add <arquivo> para incluir arquivos no índice ou git add . para incluir todos arquivos:
```
$ git add arquivo1.txt
```
```
$ git add .
```
-Crie um Commit:
```
$ git commit -m "Mensagem descritiva"
```
## Principais Comandos
- ```git add```: Adiciona as mudanças na sua branch main ou em uma criada(caso tenha feito uma)
- ```git push```: Envia suas mudanças para um repositório remoto (como o GitHub).
- ```git pull```: Atualiza seu repositório local com as mudanças do repositório remoto.
- ```git branch```: Lista, cria ou exclui branches (ramificações) no seu projeto.

## Gerenciamento de Branches
- Use branches para desenvolver recursos separadamente e mesclá-los quando prontos.
- Crie uma nova branch com ```git branch nome-da-branch```.
- Alterne para uma branch com ```git checkout nome-da-branch```.
- Mescle branches com ```git merge nome-da-outra-branch```.





