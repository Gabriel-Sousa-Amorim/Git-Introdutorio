# Documentação Introdutória Git.

Para utilizar você pode utilizar o Powershell já instalado no seu computador (caso for Windows), mas também pode utilizar pelo Git-bash.

Sendo mais preferível o Git-bash porque a branch atual é visível pelo Git-bash.


## Como criar um Repositório Local.

```powershell
$ git init
```

Quando tudo ocorrer corretamente aparecerá na saída/output do código: 

```powershell
Output: Initialized empty Git repository in C:/Diretórios_especificados
```

>O Repositório Local é utilizado quando não temos internet e queremos criar o repositório localmente nos nossos computadores. 

>Para visualizar os arquivos do seu Repositório direto pelo editor de código você terá que realizar os seguintes passos:

```powershell
$ cd "Nome da pasta do seu Repositório"
$ ls -a 
```

### Como clonar um Repositório Remoto.

```powershell
$ git clone "Url_do_Repositório_Remoto>
```

> Tem um atributo opcional que é o <directory> que seria a pasta que queremos que seja clonado o arquivo.

### Como vincular um Repositório Local a um Repositório Remoto.

Quando usamos a função para criar um repositório local:

```powershell
$ git init

$ ls -a
```

Usado quando criarmos um repositório Local no inicio do projeto, utilizamos o seguinte código para vincular o repositório local ao repositório remoto:

```powershell
$ git remote add origin "url do Repositório Remoto"
```

> Pode se utilizar seus repositórios online e de outros usuários que utilizam o **Github**. 
## Como criar arquivos no git:

Para criarmos um arquivo pelo código utilizaremos:

```powershell
$ touch "Arquivo_Criado.Formato do seu arquivo"
```

****EXEMPLO**** 
 - Criação de arquivo *.txt*.
 ```powershell
$ touch Text.txt
```
- Criação de arquivo *.html*.
```powershell
$ touch index.html
```
- Criação de arquivo *.css*.
```powershell
$ touch style.css
```

> Se enquadra para **todos** os tipos de arquivos (**.txt** , **.html** , **.css** , **.js** , **.json**, **.py** e etc...).

### Como criar pastas.
```powershell
$ mkdir "Nome_da_pasta_que_deseja_Criar"
```


## Criação de Branchs.
Uma branch é nescessária para copiarmos o projeto principal (main) e fazermos uma mudanças, adições, e correções no código principal sem afetar o código principal.

Para criar uma nova branch devemos:
```powershell
$ git branch "Nome_da_Branch_que_deseja_criar"
```

> Utilize a o caractere **_** ao invés de espaços comuns para fácil referenciamento da branch no futuro.

A branch principal no início do projeto será: 
```powershell
* main
```
> Em certos Master pode ser a sua branch principal ao invés de main.

___
### Como visualizar as branchs.

```powershell
$ git branch
```

**A Saída/Output será:**

```powershell
*main
"Outras branch criada pelo usuário"
"Outras branch criada pelo usuário"
```

### Como mudar entre Branchs.
```powershell
$ git checkout "Nome_de_Branch"
```
> Não Pode conter espaços.
> Utilize a tecla <kbd>TAB</kbd> do seu teclado para automaticamente completar o nome das suas branchs de forma correta.

## Como navegar entre pastas.

 Para entrar na pasta referenciada utilizamos:

```powershell
$ cd <Diretorio que deseja entrar>
```

Para sair da pasta atual utilizamos:

```powershell
$ cd ..
```
  
## Como subir um arquivo para um repositório remoto.

Após criarmos nosso seguinte Repositório ou clonarmos um Repositório Remoto e fazermos as criações/modificações que desejamos, iremos digitar o seguinte código:

```powershell
$ git status
```
    
> Tem nescessidade de ver as modificações que você executou, em qual branch você está, e se devemos fazer comentários.

Após isso iremos preparar nossos arquivos para a subida no Github com o seguinte código:

```powershell
$ git add .
```

Após a preparação iremos comentar nossa mudança. **Atenção aos comentários realizados, para serem objetivos e claros sobre o que você faz no arquivo**:

```powershell
$ git commit -m "Comentário sobre as modificações"
```
> Aspas duplas apenas são utilizadas quando seu comentário tem espaços. e Para comentar todos seus arquivos faça:

```powershell
$ git commit -a -m "Comentário desjado"
```

E para finalizar iremos subir o arquivo com o seguinte código: 

```powershell
$ git push
```
 ## Como atualizar um Repositório Remoto com o Pull.
 E quando temos um Repositório Online conectado em vários computadores, E se há uma atualização na branch principal o git pull irá atualizar os arquivos.
 
 ```powershell
$ git pull
```
