Primeira testagem além do curso

Método de push entre o Bash e o GitHub

códigos:

mkdir "nome da pasta" - Cria a Pasta
cd "nome da pasta" - Entra e navega entre as pastas, controle feito por colocação ou não de pontos
git init - Inicializa o repositório 
ls - para checagem dos arquivos do diretório
vi Readme.md - Abre o editor de texto
Dentro do comando vi, ou vim. Utilizar I ou Insert para digitar, Esc para finalizar e no final dshift: + wq para salvar e sair respectivamente
Após realizar as alterações quistas, utilizar os comandos seguintes para salvar e comitar
git add "nome do arquivo" sinalizar a existência do arquivo pro git
git status (checar se correu tudo certo ou se existem files untrackeds)
git commit -m "Nome da ação ou alteração realizada"
git remote add origin git@github.com:viniflopes/Repositorio"underline"particular.git (Partindo do principio de um repositorio ja criado no GitHub
git push -u origin master 

alguns comandos interessantes de ter em mente:
Login global: git config --global user.name "usuário"
Email do login: git config --global user.email "email@email.com"
Alteração do editor de texto: git config --global core.editor "comando do editor"

Para checagem: git config user.name, git config user.email, git config --list

Checagem do repertório: git status
Visualização de logs: git shortlog, git shortlog -sn (commit e pessoa), git log -- graph (modulo gráfico dos commits), git show "numeração de commit" (mostrar dados de um commit específico)

Checagem de integridade do repertório: git diff (revisão, mostrar o antes e depois de uma edição antes de commitar), git diff --name-only (mostra pra mostrar os nomes dos arquivos, não a log inteira

Desfazendo processos: git checkout "nome da file" (Desfaz a última edição realizada), git reset HEAD (volta ao estágio anterior ao comando git add), git reset --soft, --mixed, --hard (Comandos responsáveis por um checkout específico.
Soft: Cancela o commit do arquivo retornando pra forma de staged
Mixed: Cancela o Commit e volta antes do staged, antes do Add
Hard: Cancela o commit e tudo que foi feito


