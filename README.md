///////////// CONFIGURAÇÕES ///////////////
// Configurar nome para os commits
git config --global user.name "Gustavo Santos"

// Configurar e-mail para os commits
git config --global user.email "gustavobruno.contato@ymail.com"

// Verificar nome, e-mail e editor configurados
git config user.name
git config user.email
git config core.editor
*  Para alterar usar git config --global core.editor "caminho do executável"  *
///////////////////////////////////////////


/////////// COMANDOS TERMINAL /////////////
pwd = Exibe em qual página está
ls = Mostra os arquivos da pasta
mkdir = Cria uma pasta "mkdir nomedapasta"
touch = Cria um arquivo "touch exemplo.txt" ou "touch teste/exemplo.txt" cria já dentro da pasta teste
cd = Navegar nas páginas "cd teste"
ls -a = Mostrar pasta do git
///////////////////////////////////////////


///////////// COMANDOS GIT ///////////////
git init = Criar um repositório local
git status = Mostra se foi feita e qual modificação/criação de arquivos
git add = Adicina as alterações mostradas no git status no container do commit "git add *"
git commit -m "comentário = Cria um commit contendo as alterações dos arquivos
git commit -am = já da um add + commit de uma só vez
git log = Mostra os commits mais detalhados
git log --oneline = Mostra os commits simplificados em uma só linha
git log --oneline --graph = Mostra grafos
git log --oneline --graph --all = Mostra ramificações
git branch = Mostra o Ramo em que o projeto está
git diff = Mostra as alterações feitas
Tecla Q destrava a digitação quando abaixo do terminal aparece (END)
///////////////////////////////////////////


//////////////// VERSÕES //////////////////	
// Rastrear alterações do commit
git checkout a8f7357

// Voltando para última versão
git checkout master

// Desfazendo alterações de arquivos ANTES de dar um ADD
git checkout * (ou a.txt por exemplo)

// Remover conteúdo que já foi dado ADD para dentro do conteiner ANTES de commitar
git reset HEAD
OBS: vai apenas remover de dentro do container, mas não vai desfazer as alterações ainda, para desfazer tem que usar o git checkout ainda depois de tirar os arquivos do container.

// Remover um commit e voltar a uma versão anterior
git reset --hard 885acae  (identificador do commit anterior)
///////////////////////////////////////////


////////////// RAMIFICAÇÃO ///////////////
// Criar novo ramo
git checkout -b ramoteste

// Ir para determinado ramo
git checkout master

// Mostrar ramificações
git log --oneline --graph --all

// Fusão do ramoteste com o master
