# Documentação Introdutória Git.

Para usar o GIT você pode utilizar o Powershell já instalado no seu computador (caso for Windows), mas também pode utilizar pelo Git-bash.

> Sendo mais preferível o Git-bash porque a branch atual é visível pelo Git-bash, além de terem mudanças entre as suas semanticas.

## Como criar um Repositório Local.

> O seguinte código funciona para **Powershell e Git-bash**.

```bash
$ git init
```

Quando tudo ocorrer corretamente aparecerá na saída/output do código: 

```powershell
Output: Initialized empty Git repository in C:/Diretórios_especificados
```

>O Repositório Local é utilizado quando não temos internet e queremos criar o repositório localmente nos nossos computadores. 

### Como visualizar os arquivos do seu Repositório direto pelo editor de código:

O seguinte código funciona apenas com o **Git-bash**:

```bash
$ cd "Nome da pasta do seu Repositório"
$ ls -a
```

O seguinte código é funciona para o **Powershell**:

```powershell
dir "Nome_da_Pasta"
```

>Entretanto temos outra forma no Powershell:

```powershell
cd "Nome_da_Pasta_que_deseja_visualizar"
dir
```

### Como clonar um Repositório Remoto.

```bash
$ git clone "Url_do_Repositório_Remoto>
```

> Tem um atributo opcional que é o <directory> que seria a pasta que queremos que seja clonado o arquivo.

### Como vincular um Repositório Local a um Repositório Remoto.

Quando usamos a função para criar um repositório local:

```bash
$ git init
```

Usado quando criarmos um repositório Local no inicio do projeto, utilizamos o seguinte código para vincular o repositório local ao repositório remoto:

```bash
$ git remote add origin "url do Repositório Remoto"
```

> Pode se utilizar seus repositórios online e de outros usuários que utilizam o **Github**. 
## Como criar arquivos no Git-Bash.

Para criarmos um arquivo pelo **Git-Bash** utilizaremos:

```bash
$ touch "Arquivo_Criado.Formato do seu arquivo"
```

****EXEMPLO**** 
 - Criação de arquivo **.txt**.
```bash
$ touch text.txt
```
- Criação de arquivo **.html**.
```bash
$ touch index.html
```
- Criação de arquivo **.css**.
```bash
$ touch style.css
```

> Se enquadra para **todos** os tipos de arquivos (**.txt** , **.html** , **.css** , **.js** , **.json**, **.py** **.md** e etc...).


## Como criar arquivos no Powershell.

Para criarmos um arquivo pelo **Powershell** utilizaremos:

```powershell
ni "Arquivo_Criado.Formato do seu arquivo"
```

****EXEMPLO**** 
 - Criação de arquivo **.txt**.
```powershell
ni text.txt
```
- Criação de arquivo **.html**.
```powershell
ni index.html
```
- Criação de arquivo **.css**.
```powershell
ni style.css
```

> Se enquadra para **todos** os tipos de arquivos (**.txt** , **.html** , **.css** , **.js** , **.json**, **.py** **.md** e etc...).

### Como criar pastas.
```powershell
$ mkdir "Nome_da_pasta_que_deseja_Criar"
```

## Criação de Branchs.
Uma branch é nescessária para copiarmos o projeto principal (main) e fazermos uma mudanças, adições, e correções no código principal sem afetar o código principal.

Para criar uma nova branch devemos:
```bash
$ git branch "Nome_da_Branch_que_deseja_criar"
```

Para criar uma branch nova e entrar nela execute:

```bash
$ git checkout -b "Nome_da_Branch_que_deseja_criar"
```

> Utilize a o caractere **_** ao invés de espaços comuns para fácil referenciamento da branch no futuro.

A branch principal no início do projeto será: 
```powershell
* main
```
> Em certos Master pode ser a sua branch principal ao invés de main.

___
### Como visualizar as branchs.

```bash
$ git branch
```

**A Saída/Output será:**

```bash
*main
"Outras branch criada pelo usuário"
"Outras branch criada pelo usuário"
```

### Como mudar entre Branchs.
```bash
$ git checkout "Nome_de_Branch"
```
> Não Pode conter espaços.

 Utilize a tecla <kbd>TAB</kbd> do seu teclado para automaticamente completar o nome das suas branchs de forma correta.

## Como navegar entre pastas.

 Para entrar na pasta referenciada utilizamos:

```bash
$ cd <Diretorio_que_deseja_entrar>
```

Para sair da pasta atual utilizamos:

```bash
$ cd ..
```
  
## Como subir um arquivo para um repositório remoto.

Após criarmos nosso seguinte Repositório ou clonarmos um Repositório Remoto e fazermos as criações/modificações que desejamos, iremos digitar o seguinte código:

```bash
$ git status
```
    
> Tem nescessidade de ver as modificações que você executou, em qual branch você está, e se devemos fazer comentários.

Após isso iremos preparar nossos arquivos para a subida no Github com o seguinte código:

```bash
$ git add .
```

Após a preparação iremos comentar nossa mudança. **Atenção aos comentários realizados, para serem objetivos e claros sobre o que você faz no arquivo**:

```bash
$ git commit -m "Comentário sobre as modificações"
```
> Aspas duplas apenas são utilizadas quando seu comentário tem espaços. e Para comentar todos seus arquivos faça:

E para finalizar iremos subir o arquivo com o seguinte código: 

```bash
$ git push
```
## Pull, Como atualizar um Repositório Local.

 E quando temos um Repositório Online conectado em vários computadores, E se há uma atualização na branch principal o git pull irá atualizar os arquivos.
 
```bash
$ git pull
```

 Como ver a diferença antes e depois do pull.

```bash
$ git diff HEAD
```

> A 'HEAD' seria suas modificações mais recentes.

## Commit, Como comentar seus arquivos.

Após você adicionar os comentários a seus arquivos você deverá fazer um comentário, e para comentar você executará:

***É uma obrigação utilizar comentários***

```bash
$ git commit -m "Comentário desjado"
```

Para comentar todos seus arquivos execute:

```bash
$ git commit -a -m "Comentário desjado"
```

Para visualizar o histórico dos seus comentários deverá fazer o seguinte comando:

```bash
$ git log
```

### Como modificar seu último comentário

```bash
$ git commit --amend -m "Comentário atualizado"
```

## Push, maneiras de como executar.

Após preparar seus arquivos e executar o comentário Por padrão executaremos o:

```bash
$ git push
```

Também há como fazer o Push dos arquivos do repositorio Local ao Remoto pelo Seguinte comando 

```bash
$ git push -u origin master
```

>Funcionando na seguinte ordem:

```bash
 $ git push -u 'nome do repositorio remoto' 'nome da branch'
```

## Bibliografia

* [GIT Documentation](https://git-scm.com/docs)
* [GIT POWERSHELL](https://git-scm.com/book/pt-pt/v2/Appendix-A:-Git-em-Outros-Ambientes-Git-no-Powershell)
* [ Comandos Git](https://comandosgit.github.io)
* [BALTA.io](https://balta.io/blog/documentacao-com-github)
