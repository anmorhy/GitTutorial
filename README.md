## Instalando o GIT

* [Link com os downloads](https://git-scm.com/downloads)

## Criar um projeto novo

* Criar uma nova pasta no PC pra isso chamada `git`

* Abrir o VSCode nessa pasta

* Criar um novo arquivo `README.md`

* Salva o arquivo

* Abre o Git Bash que foi instalado na máquina (pode ser pelo terminal do VSCode mesmo)

* `git init` para inicializar o repositório

* Foi criada uma pasta `.git` onde fica as configurações do git

* `git add README.md` para colocar o arquivo na área de stagging 

* Esse `add` é necessário antes de darmos o commit 

* `git commit -m "First"` para dar o primeiro commit no repositório

* `git branch -M "main"` para alterar o nome da branch principal de `master` para `main`

## Repositório no Github

* Ir em `Criar novo repositório`
* Preencher as informações do projeto, então dar o nome do repositório, e criar
* Para passar o commit do meu repositório local (da minha máquina) para um repositório na plataforma do Github, usamos o `git remote add origin <link do repositório>`
* `origin` é o nome utilizado para referenciar o nosso repositório
Agora já temos o nosso repositório local conectado com o respositório do Github, porém o `commit` que damos na máquina não sobe automaticamente para a plataforma
* Para isso precisaremos empurrar, enviar para lá com o `git push -u origin main`

* O Arquivo ja se encontrará na plataforma Github

## Alterando e adicionando arquivo

* Adicionar conteudos a pasta ou alterar algo

* Subindo a alteração, pra isso segue `git add .` (agora ponto `.` pois adiciona todos os arquivos) e `git commit -m "Primeira alteração"`

* Lembrando que para alterar algo no nosso respositório do Github precisamos dar o push, então `git push origin main` (sem o -u)

* O verde com `+` e o vermelho com `-` mostra, os conteúdos que foram adicionados e editados dentro do código.

## Branch

* Nesse caso vamos adicionar um novo arquivo para desenvolver a nossa feature `page`

* Para criar `git checkout -b "new-page"`, assim criando uma branch
Esse comando além de criar a branch já entra nela com o checkout, 

* Vou então criar o arquivo, criar o `page.md`

* Coloca a alteração em stagging com o `git add .` e commitamos com o `git commit -m "nova pagina"`

* Para enviar usa `git push origin page`

* No Github, haverá 2 branches, a `main` e a `page`

## Merge

* Ir na branch principal `git checkout main` e fazer o merge com a branch `page` criada, com `git merge page`

* Tudo o que contem de alteração na branch `page` juntou com a `main`

* Para jogar no Github utiliza `git push origin main`

## Clone

* copiar o link do repositorio e colocar no terminal

* O comando para puxar o projeto para a sua máquina é o `git clone https://github.com/..`

## Pull

* Para Alterar no repositorio usar `git pull`, ele irá puxar todas as alterações feitas no repositório do Github para o seu repositório local

## Fork

* A ferramenta `fork`, Faz um clone do repositorio para o github

## Pull request

* Após realizar um fork no projeto e ele ter ido pra o github, poderá alterar o projeto

* Depois para salvar o projeto, dar o `git add .`, `git commit -m "validação de botões"` e `git push origin main`

* Isso significa que a branch do seu repositório está 1 commit "na frente" da branch original
