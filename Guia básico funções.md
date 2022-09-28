primeiros passos no github <br>
esses comandos configuram seu usuário e e-mail globais do Git:<br>

*git config --global user.name "<seunome>"* <br>
*git config --global user.email <seuemail>*


esse comando inicializa um repositório vazio:


**git init**  <br>

esse comando conecta o repositório vazio com o repositório do GitHub:
git remote add origin <link do repositório>


Para que essa alteração esteja no seu GitHub, é preciso primeiro colocar esse arquivo em “stage”, ou seja, pronto pra ser commitado. Então abra o GitBash e digite o seguinte código:

esse comando adiciona o arquivo criado para ser commitado
**git add "readme.md"** esse comando adiciona TODOS os novos arquivos criados para serem commitados
git add.

Agora que o arquivo está pronto, é preciso “commita-lo”, ou seja, empacotá-lo para ser enviado ao repositório. Digite os seguintes códigos e a mensagem do commit, que serve para identificar quais alterações foram feitas em cada etapa do versionamento.

esse comando efetiva o commit:

__git commit -m "mensagem aqui"__  <br>

esse comando manda as alterações para seu GitHub:

__git push -u origin <my-branch>__


esse comando mostra o estado do repositório:
git status

comandos de histórico de ações:

**git log** (mostra todas as alterações) <br>
**git log** --oneline (mostra o histórico resumido) (br)
**git log -p** (detalha cada alteração)<br>
**git diff <numero>..<numero>** (mostra as diferenças entre 2 commits)

comandos que desfazem ações:

**git checkout -- <arquivos>** (antes do add)  <br>
**git reset HEAD <arquivos>**   <br>
**git checkout -- <arquivos>** (depois do add e antes do commit)   <br>
**git revert** (depois do commit)



# Reforçando

definir o email:

**git config --global user.email <gerhardt1312@gmail.com>**

GIT INIT: **git init**

GIT ADD: **git add temp.txt**

GIT CLONE: Se o repositório estiver em um servidor remoto, use: **git clone <e-mail a ser clonado>**

Por outro lado, se uma cópia de trabalho de um repositório local for criada, use: **git clone /path/to/repository**


GIT COMMIT: Uso: **git commit –m “coloque sua mensagem aqui”**

GIT STATUS:**git status**

GIT PUSH: Um simples envio envia as alterações feitas para o ramo mestre do repositório remoto associado ao diretório de trabalho.

Por exemplo:

**git push origin master**

GIT REMOTE: **git remote –v** <br>

Esse comando permite que o usuário se conecte a um servidor remoto:

**git remote add origin <93.188.160.58>**

GIT BRANCH:Para listar todos os ramos presentes no repositório, use:

git branch

Para excluir um ramo: **git branch –d <branch-name>**


GIT PULL: Para mesclar todas as alterações presentes no repositório remoto para o diretório de trabalho local, o comando pull é usado. Uso: git pull

GIT MERGE:O comando git merge é usado para mesclar uma ramificação no ramo ativo. Uso: **git merge <branch-name>**