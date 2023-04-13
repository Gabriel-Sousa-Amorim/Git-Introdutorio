# Documentação Introdutória Git.
## Como criar um Repositório Local:

```bash
$ git init
```

Quando tudo ocorrer corretamente aparecerá na saída/output do código: 

```bash
Output: Initialized empty Git repository in C:/Diretórios_especificados
```

>O Repositório Local é utilizado quando não temos internet e queremos criar o repositório localmente nos nossos computadores. 

### Como clonar um Repositório Remoto:

```bash
$ git clone "Url_do_Repositório_Remoto>
```

> Tem um atributo opcional que é o <directory> que seria a pasta que queremos que seja clonado o arquivo.
 
### Como vincular um Repositório Local a um Repositório Remoto:

Quando usamos a função para criar um repositório local:

```bash
$ git init
```

Usado quando criarmos um repositório Local no inicio do projeto, utilizamos o seguinte código para vincular o repositório local ao repositório remoto:

```bash
$ git remote add origin "url do Repositório Remoto"
```

> Pode se utilizar seus repositórios online e de outros usuários que utilizam o **Github**. 
## Como criar arquivos no git:

Para criarmos um arquivo pelo código utilizaremos:

```bash
$ touch "Arquivo_Criado.Formato do seu arquivo"
```

****EXEMPLO**** 
 - Criação de arquivo *.txt*.
 ```bash
$ touch Text.txt
```
- Criação de arquivo *.html*.
```bash
$ touch index.html
```
- Criação de arquivo *.css*.
```bash
$ touch style.css
```

> Se enquadra para **todos** os tipos de arquivos (**.txt** , **.html** , **.css** , **.js** , **.json**, **.py** e etc...).

### Como criar pastas:
```bash
$ mkdir "Nome_da_pasta_que_deseja_Criar"
```


## Criação de Branchs
Uma branch é nescessária para copiarmos o projeto principal (main) e fazermos uma mudanças, adições, e correções no código principal sem afetar o código principal.

Para criar uma nova branch devemos:
```bash
$ git branch "Nome_da_Branch_que_deseja_criar"
```

> Utilize a o caractere **_** ao invés de espaços comuns para fácil referenciamento da branch no futuro.

A branch principal no início do projeto será: 
```bash
* main
```
> Em certos Master pode ser a sua branch principal ao invés de main.

___
### Como visualizar as branchs:

```bash
$ git branch
```

**A Saída/Output será:**

```bash
*main
"Outras branch criada pelo usuário"
"Outras branch criada pelo usuário"
```

### Como mudar entre Branchs:
```bash
$ git checkout "Nome_de_Branch"
```
> Não Pode conter espaços.
> Utilize a tecla <kbd>TAB</kbd> do seu teclado para automaticamente completar o nome das suas branchs de forma correta.

## Navegação entre pastas:

 Para entrar na pasta referenciada utilizamos:

```bash
$ cd <Diretorio que deseja entrar>
```

Para sair da pasta atual utilizamos:

```bash
$ cd ..
```
  
## Como subir um arquivo para um repositório remoto 

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
> Aspas duplas apenas são utilizadas quando seu comentário tem espaços.

E para finalizar iremos subir o arquivo com o seguinte código: 

```bash
$ git push
```
 ## Pull
 E quando temos um Repositório Online conectado em vários computadores, E se há uma atualização na branch principal o git pull irá atualizar os arquivos.
 
 ```bash
$ git pull
```
