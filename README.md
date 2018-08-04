# Git
Comandos Git  

**Instalação**

	Linux
	Yum - yum install git-core
	Ubuntu - apt-get install git

	Mac
	Se vc estiver o MacPorts
	sudo port install git-core +svn +doc +bash_completion +gitweb

	Windows
	Baixa no site https://gitforwindows.org/

**Ajuda**  
git help

**Definir usuário**  
git config --global user.name "Jackson Paiva"

**Definir email**  
git config --global user.email "jackbpaiva@gmail.com"

**Saída colorida do Git**  
git config color.ui true

**Criar alias status**  
git config --global alias.st status

**Criar um novo repositório**  
git init

**Obter repositório existente**  
git clone /caminhopararepositorio

**Obter repositório remoto**  
git clone jackson@177.165.156.7:/path/to/repository

**Ignorar arquivos**  
.gitignore

**Interface gráfica para o git**  
gitk

**Adicionar um arquivo**  
git add teste.txt

**Adicionar um diretório**  
git add test

**Adicionar arquivos e diretórios**  
git add .

**Adicionar um aquivo que esteja no .gitignore**  
git add -f file.txt

**Remove um arquivo do índice do repositório**  
git rm filename.txt

**Visualizar todos os commits**  
git log

**Visualizar todos os commits de um determidado autor**  
git log --author=user

**Listar todos os repositório remotos**  
git remote -v

**Vincular um repositório local a um repositório remoto**  
git remote add origin git@github.com:jackson/teste.git

**Renomear repositório remoto**  
git remote rename origin teste

**Desvincular a um repositório remoto**  
git remote rm teste

**Salvar**  
git commit –m "mensagem"

**Ammend com o último commit**  
git commit --amend

**Exibe a lista de arquivos alterados**  
git status

**Envia para o servidor**  
git push origin master

**Faz checkout de uma branch**  
git checkout -b branch

**Lista as branches locais**  
git branch

**Lista as branches remotas**  
git branch -r

**Lista as branches já fundidas no master**  
git branch --merged

**Lista as branchs não fundidas no master**  
git branch --no-merged

**Exclui um ramo**  
git branch –d branch

**Cria uma branch**  
git branch bug-ABC

**Merge de alteracões (Você deve estar no branch em que deseja receber as alterações e passar o branch de onde você quer as alterações)**  
git merge bug-ABC

**Resetar uma branch**  
git reset --hard HEAD

**Atualiza a branch atual**  
git pull

**Busca as alterações. Mais não aplica ao repositório.**  
git fetch 

**Lista conflitos**  
git diff source-branch target-branch

**Criar tag**  
git tag v-1.1

**Tag anotada**  
git tag -a v-1.1 -m "Tag 1.1"

**Criar tag em um commit**  
git tag -a v-1.2 9fceb02

**Rebase branches**  
git checkout bug-ABC
git rebase master

**Visualiza todos os hashs**  
git reflog

**Interface Web - (webrick - Se vc possuir o ruby instalado)**  
git instaweb --httpd=webrick

**Git stash**  
git stash

**Restaurar uma stash antiga**  
git stash apply nome
git stash apply stash@{id}

**Procurar por erros**  
git blame

**Procurar frases, texto**  
git grep java

**Executa o* Garbage Collection**  
git gc --auto

**Voltar um commit**  
git reset

**Verificar consistência do repositório**  
git fsck

