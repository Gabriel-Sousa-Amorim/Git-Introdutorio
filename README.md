## Como criar/clonar Repositórios:

#### Como criar um Repositório Local:

 `git init`

> Quando tudo ocorrer corretamente aparecerá na saída do código: 

`Output: Initialized empty Git repository in C:/Diretórios especificados`

>O Repositório Local é utilizado quando não temos internet e queremos criar o repositório localmente nos nossos computadores. 

#### Como clonar um Repositório Remoto:

-> `git clone "Url do Repositório que deseja Clonar"`

> Pode se utilizar seus Repositórios Online e de outros usuários que utilizam o **Github**   
> 
## Como criar arquivos no Git:

-> `touch "Seu arquivo.Formato do seu arquivo"`

*EXEMPLO* 
 - Criação de arquivo *.txt* 
-> `touch text.txt`
- Criação de arquivo *.html*
-> `touch index.html`
- Criação de arquivo *.css*
-> `touch style.css`

> Se enquadra para **todos** os tipos de arquivos (**.txt** , **.html** , **.css** , **.js** , **.json**, **.py** e etc...)

#### Como criar pastas:

-> `mkdir "Nome da pasta que deseja criar"`


## Criação de Branchs (Para divisão de Partes de Trabalho, para não haver exclusões):
Para criar uma nova branch devemos: 
-> `git branch "Nome da Branch que deseja criar"`

> Utilize a o caractere **_** ao invés de espaços comuns para fácil referenciamento da branch no fututo.

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

Quando usamos isso e queremos vincular à um repositório local
  

    git init

Usado quando criarmos um repositório Local no inicio do projeto:  

    git remote add origin "url do Repositório Remoto"

## Navegação entre pastas:
Para sair da pasta atual utilizamos:

    `cd ..` 

 Para entrar na pasta referenciada utilizamos:

    cd "nome da pasta"

 
___


