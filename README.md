# Git

## Como criar/clonar Repositórios:

**Como criar um Repositório Local:**

 `git init`

> Quando tudo ocorrer corretamente aparecerá na saída/output do código: 

`Output: Initialized empty Git repository in C:/Diretórios especificados`

>O Repositório Local é utilizado quando não temos internet e queremos criar o repositório localmente nos nossos computadores. 

**Como clonar um Repositório Remoto:**

-> `git clone "Url do Repositório que deseja Clonar"`

> Pode se utilizar seus Repositórios Online e de outros usuários que utilizam o **Github**   
> 
## Como criar arquivos no Git:

Para criarmos um arquivo pelo código utilizaremos:

    touch "Seu arquivo.Formato do seu arquivo"
    

***EXEMPLO*** 
 - Criação de arquivo *.txt* 
touch text.txt

- Criação de arquivo *.html*
-> `touch index.html`
- Criação de arquivo *.css*
-> `touch style.css`

> Se enquadra para **todos** os tipos de arquivos (**.txt** , **.html** , **.css** , **.js** , **.json**, **.py** e etc...)

**Como criar pastas:**

-> `mkdir "Nome da pasta que deseja criar"`


## Criação de Branchs
Uma branch é nescessária para copiarmos o projeto principal (main) e fazermos uma mudanças, adições, e correções no código principal sem afetar o código principal 

**Para criar uma nova branch devemos:** 
`git branch "Nome da Branch que deseja criar"`

> Utilize a o caractere **_** ao invés de espaços comuns para fácil referenciamento da branch no futuro.

A branch principal no início do projeto será: 

     main/master
___
### Como visualizar as branchs:

`git branch`

A Saída/Output será:

    *main
    "Exemplo de outra branch criada pelo usuário"

  Como mudar entre Branchs:

      git checkout "Nome de Branch"

> Utilize a tecla <kbd>TAB</kbd> do seu teclado para automaticamente completar o nome das suas branchs de forma correta.

## Como vincular um Repositório Local a um Repositório Remoto:

Quando usamos a função para criar um repositório loc:

    git init

Usado quando criarmos um repositório Local no inicio do projeto, utilizamos o seguinte código para vincular o repositório local ao repositório remoto:

    git remote add origin "url do Repositório Remoto"

## Navegação entre pastas:
Para sair da pasta atual utilizamos:

    `cd ..` 

 Para entrar na pasta referenciada utilizamos:

    cd "nome da pasta"

## Como subir um arquivo para um repositório remoto 

Após criarmos nosso seguinte Repositório ou clonarmos um Repositório Remoto e fazermos as criações/modificações que desejamos, iremos digitar o seguinte código:

    git status
    

> Tem nescessidade de ver as modificações que você executou, em qual branch você está, e se devemos fazer comentários.

Após isso iremos preparar nossos arquivos para a subida no Github com o seguinte código:

`git add .`

Após a preparação iremos comentar nossa mudança. **Atenção aos comentários realizados, para serem objetivos e claros sobre o que você faz no arquivo**

    git commit -m "Seu comentário"
    

> Aspas duplas apenas são utilizadas quando seu comentário tem espaços.

E  para finalizar iremos subir o arquivo com o seguinte código 


 ___
