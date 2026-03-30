🚀 Guia de Consulta Rápida: Git (Cheatsheet)

Este guia contém os comandos mais utilizados no dia a dia para versionamento de projetos.

📂 Configurações Iniciais

Antes de começar, configure sua identidade para que os commits sejam atribuídos corretamente.

git config --global user.name "Seu Nome": Define o nome de usuário.

git config --global user.email "seuemail@exemplo.com": Define o e-mail.

git config --list: Lista todas as configurações atuais.

🛠️ Iniciando e Clonando

git init: Inicia um novo repositório Git na pasta atual.

git clone <url>: Clona um repositório remoto existente para sua máquina.

🔄 Ciclo de Trabalho (O Básico)

O fluxo padrão de salvar alterações.

git status: Verifica o estado atual (quais arquivos foram modificados).

git add <arquivo>: Adiciona um arquivo específico para a área de espera (staging).

git add .: Adiciona todos os arquivos modificados para a área de espera.

git commit -m "mensagem": Salva as alterações com uma descrição do que foi feito.

git commit --amend: Edita o último commit (cuidado se já tiver enviado para o servidor).

🌿 Branches (Ramos)

Essencial para trabalhar em novas funcionalidades sem quebrar o código principal.

git branch: Lista os ramos locais.

git branch <nome-do-ramo>: Cria um novo ramo.

git checkout <nome-do-ramo>: Alterna para o ramo especificado.

git checkout -b <nome-do-ramo>: Cria e já alterna para o novo ramo de uma vez.

git merge <nome-do-ramo>: Une o ramo especificado ao ramo atual.

git branch -d <nome-do-ramo>: Deleta um ramo (após o merge).

☁️ Repositórios Remotos (GitHub/GitLab)

Sincronização com o servidor.

git remote add origin <url>: Conecta seu repositório local a um servidor remoto.

git push origin <nome-do-ramo>: Envia seus commits locais para o servidor.

git pull: Baixa as novidades do servidor e já faz o merge no seu código.

git fetch: Baixa as novidades do servidor, mas não aplica as mudanças ao seu código (mais seguro para revisar).

⏪ Desfazendo Coisas

git checkout -- <arquivo>: Descarta as mudanças locais em um arquivo (volta ao estado do último commit).

git reset HEAD <arquivo>: Tira um arquivo da área de espera (unstage).

git reset --hard HEAD~1: Apaga o último commit e todas as mudanças feitas nele (use com cautela!).

git revert <hash-do-commit>: Cria um novo commit que desfaz as alterações de um commit específico (forma segura de desfazer).

🔍 Histórico e Logs

git log: Mostra o histórico de commits.

git log --oneline: Mostra o histórico de forma resumida (uma linha por commit).

git diff: Mostra as alterações exatas nos arquivos que ainda não foram adicionados.

📦 Guardando Temporariamente (Stash)

git stash: "Esconde" suas alterações atuais para limpar a pasta de trabalho sem precisar fazer commit.

git stash list: Lista o que está guardado.

git stash pop: Recupera as alterações guardadas e as aplica de volta.
