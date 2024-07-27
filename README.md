<h1>questoes-da-prova2</h1>


## Sumário

1. [Introdução ao GitHub](#introdução-ao-github)
2. [Configuração Inicial](#configuração-inicial)
3. [Comandos Básicos do Git](#comandos-básicos-do-git)
4. [Trabalho Colaborativo](#trabalho-colaborativo)
5. [Funcionalidades Avançadas](#funcionalidades-avançadas)
6. [Boas Práticas e Dicas](#boas-práticas-e-dicas)   

# Introdução ao GitHub

### O que é GitHub?

O GitHub é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.  
Em resumo, o GitHub é um serviço baseado em nuvem que hospeda um sistema de controle de versão chamado Git. Isso significa que os desenvolvedores podem colaborar e fazer mudanças em projetos compartilhados enquanto mantêm um registro detalhado do progresso.

### História e evolução do GitHub
O **GitHub** foi desenvolvido por Chris Wanstrath, J. Hyett, Tom Preston-Werner e Scott Chacon usando Ruby on Rails e começou em fevereiro de 2008. A empresa, _GitHub, Inc._, existe desde 2007 e está localizada em São Francisco.  
Desde então, o GitHub se tornou uma plataforma essencial para colaboração e hospedagem de código-fonte com controle de versão usando o **Git**. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou **Open Source** de qualquer lugar do mundo.  
Além disso, o GitHub é amplamente utilizado por programadores para divulgação de seus trabalhos ou para que outros programadores contribuam com o projeto. Ele promove fácil comunicação através de recursos como relatórios de problemas e solicitações de pull. Atualmente, o GitHub abriga mais de **100 milhões de projetos**, incluindo alguns conhecidos mundialmente, como WordPress, GNU/Linux, Atom e Electron.


### Principais funcionalidades e benefícios
- **Controle de Versão Distribuído**: Construído sobre o Git, o GitHub permite rastrear mudanças no código, reverter para versões anteriores e colaborar eficientemente.  
- **Hospedagem de Repositórios**: Você pode criar repositórios públicos ou privados para armazenar seu código-fonte e facilitar o compartilhamento e a colaboração.  
- **Colaboração**: Múltiplas pessoas podem trabalhar juntas em um projeto, criando ramificações para desenvolver recursos separadamente e mesclando-os quando prontos.  
- **Relatórios de Problemas e Solicitações de Pull**: Usuários podem relatar problemas e enviar solicitações de pull para propor alterações no código.
- Integração com Ferramentas: O GitHub se integra a várias ferramentas de desenvolvimento.  
- **GitHub Pages**: Permite hospedar sites estáticos diretamente de seus repositórios.

# Configuração Inicial

### Criando uma conta no GitHub:

  1. Acesse o site do [GitHub](https://github.com/).
  2. Clique em “Sign up” (ou “Inscreva-se”) e siga as instruções para criar sua conta.
  3. Verifique seu e-mail para confirmar o cadastro.

### Instalando o Git e configurando no GitHub:
 - Instale o Git em seu computador. Você pode baixá-lo em [git-scm.com](https://git-scm.com/).
 - Abra o terminal (ou prompt de comando) e configure seu nome de usuário e e-mail globalmente com os seguintes comandos:

```powershell
$ git config --global user.name "Seu Nome"
```
```powershell
$ git config --global user.email "seu@email.com"
```

### Primeiros passos: criando e clonando repositórios:

- Crie um novo repositório no GitHub clicando em “New” (ou “Novo”).  
- Dê um nome ao repositório, escolha a visibilidade (público ou privado) e clique em “Create repository” (ou “Criar repositório”).  
- Para clonar um repositório existente, copie o link do repositório no GitHub e execute o seguinte comando no terminal:
```console
$ git clone <link-do-repositório>
```
# Comandos Básicos do Git

### Estrutura de um Repositório Git

Um repositório Git é uma estrutura que armazena seu código-fonte e histórico de versões. Ele consiste em três áreas principais:
- **Diretório de Trabalho *(Working Directory)***: É onde você edita e cria arquivos do seu projeto os arquivos aqui não estão rastreados pelo Git.

- **Índice *(Staging Area)***: Também conhecido como área de preparação, aqui você seleciona quais mudanças deseja incluir no próximo commit e os arquivos adicionados ao índice estão prontos para serem confirmados.

- **Histórico de Commits *(Branches)***: O Git mantém um histórico de todas as versões do seu projeto, cada commit representa um estado específico do código e os commits formam uma sequência linear ou ramificada (branches).

### Iniciando um Repositório

- Instale o Git:
Baixe e instale o Git em seu computador

- Configuração Inicial: Configure seu nome de usuário e endereço de e-mail globalmente:
```powershell
$ git config --global user.name "Seu Nome"
```
```powershell
$ git config --global user.email "seu@email.com"
```
- Crie um Repositório: Navegue até o diretório do seu projeto usando o terminal e execute o comando git init para iniciar o rastreamento do repositório:
```powershell
$ git init
```
- Adicione Arquivos ao Índice: Use `git add <arquivo>` para incluir arquivos no índice ou `git add .` para incluir todos arquivos:
```powershell
$ git add arquivo1.txt
```
```powershell
$ git add .
```
- Crie um Commit:
```powershell
$ git commit -m "Mensagem descritiva"
```
### Principais Comandos
- `git init`: É o responsável por iniciar um repositório Git no projeto, criando a pasta **.git**, que vai guardar as informações sobre as mudanças no código
- `git add <arquivo>`: Adiciona os arquivos à area de preparação (staging) para o commit, ou seja, informa ao git quais arquivos devem ser incluidos no próximo commit.
- `git commit`: Grava todas as alterações dos arquivos adicionados no comando anterior ao repositório, criando um novo "ponto na história" do projeto.
- `git push`: Envia suas mudanças para um repositório remoto (como o GitHub).
- `git pull`: Atualiza seu repositório local com as mudanças do repositório remoto.
- `git branch`: Lista, cria ou exclui branches (ramificações) no seu projeto.

### Gerenciamento de Branches
Use branches para desenvolver recursos separadamente e mesclá-los quando prontos.
- Crie uma nova branch com `git branch <nome-da-branch>`.
- Alterne para uma branch com `git checkout <nome-da-branch>`.
- Mescle branches com `git merge <nome-da-outra-branch>`.

# Trabalho Colaborativo

### Clonando e forkeando repositórios
**Clonar _(clone)_**: Cria uma cópia local do repositório do GitHub no seu computador e permite a contribuição direta a um projeto.  
```console
$ git clone <link-do-projeto>
```
**Forkear *(Fork)***: Cria uma cópia do repositório na sua conta do GitHub e possibilita a criação de novas funcionalidades sem afetar o projeto original, ramificando o projeto.
- No GitHub, clique no botão "Fork" na página do repositório
![botão fork](img\forkimg.png)

### Pull requests: como criar e gerenciar
- Criando Pull Request:
  1. Faça alterações desejadas no seu repositório.
  2. Envie as alterações para o GitHub:
      ```powershell
      $ git add .
      $ git commit -m "Descrição das suas alterações"
      $ git push origin <nome-da-branch>
      ```
  3. Na página principal do repositório no GitHub, escolha a branch que contém os seus commits e clique no botão "Compare & pull request" na faixa amarela que aparecerá acima dos arquivos.
  4. Adicione um título e uma descrição e clique em "Create Pull Request"  

- Gerenciando Pull Requests: Após o pull request, podem ser feitas revisões por outros desenvolvedores, que adicionarão comentários e sugestões. Se necessário, é possível fazer novas alterações no código enviá-lo (usando `git push`) para atualizar o Pull Request

### Revisão de código e merge de pull requests
- **Revisão de Código**: Como parte do gerenciamento das Pull Request nos seus projetos, a revisão de código vai garantir que a alteração do código do seu projeto manterá a qualidade e estilo de código já presente anteriormente, assim como assegurar que, mesmo com as alterações, o código ainda funcionará corretamente.

- **Merge**: Após a revisão e a aprovação, o Pull Request pode ser incorporado ao projeto principal. Geralmente, o dono do repositório realiza o merge no GitHub.

### Resolvendo conflitos
Conflitos acontecem quando duas pessoas alteram a mesma linha de código.
- Como resolver:
  1. O Git indicará os arquivos com conflito
  2. Abra o arquivo e analise as marcações conflito, da seguinte forma:
      ```powershell
      <<<<<<< HEAD
      Conteúdo que está na sua versão atual do arquivo (HEAD).
      =======
      Versão do outro desenvolvedor, vinda da branch especificada.
      >>>>>>> nome-da-branch-do-outro-desenvolvedor
      ```
  3. Edite o arquivo, escolhendo a versão correta ou mesclando as alterações manualmente.
  4. Salve o arquivo, adicione as alterações (`git add .`) e faça um novo commit.

# Funcionalidades Avançadas


# Boas Práticas e Dicas

