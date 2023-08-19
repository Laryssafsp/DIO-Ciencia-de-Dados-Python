# configurando o GIT
git config

# limpar terminal
ctrl l

# para configuração do usuário tenha sempre o mesmo usuário, configuração será Global
git config -- global user.name "name"
git config -- global user.email "name@email"

# verificar
git config -- global user.name
git config -- global user.email

# retorna o nome da Branch padrão
git config init.defaulBranch 

# alterar Branch padrão 
git config --global init.defaulBranch main

# copiar um repositório
git clone url
# nome do user:
# senha: token do github

# Armazenar os repositórios do GitHub
## gerar um token para autenticação setting -> tokens -> developer setting -> personal access tokens -> tokens(classic)

# Salvar a credencial na máquina para não precisar realizar sempre o procedimento
## caso queira um salvamento temporário
git config credential.helper cache 
## caso queira um salvamento permanente
git config --global credential.helper store

# a partir deste momento, não irá solicitar a senha (token)

# retornar credencial
git config --global credential.helper

# mostrar caminho dos armazenamentos
git config --global --show-origin credential.helper

# exibir o conteúdo do arquivo
cat (.gitconfig) arquvio

# criar uma pasta
mkdir  <nome pasta>

# entrar pasta
cd <nome pasta>

# voltar
cd ..

# transformar em repositorio Git
git init

# exibir conteúdo 
cat config

# clonar
git clone <url> 
## clonar em uma nova pasta
git clone <url> nova pasta
## clonar uma branch específica
git clone <url> --branch <nome> --single-branch
### se não passar o nome, ele clona a principal main ou master

# Repositórios remotos
git remote -v

git remote add origin <url do repositório que deseja vincular>

# status no repositorio (área de preparação)
git status

