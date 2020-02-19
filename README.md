Roteiro Git e Github
1. Crie uma pasta com seu nome, sem espaços e acentos
2. Inicialize esta pasta para ser um repositório versionado com o git
• git init
3. Crie um arquivo com nome de README.md. Adicione algum texto dentro dele.
4. Adicione o arquivo ao estágio "staged”
• git add README.md
5. Dê commit no arquivo criado. No commit use uma a mensagem "Primeiro commit"
• git commit -m "Primeiro commit"
6. Sua modificação está no repositório local apenas, agora criaremos um repositório no Github.
7. Crie um repositório na sua conta github chamado nome_de_usuario.github.io
8. Associe sua pasta local ao repositório criado
• git remote add origin git@github.com:xxxx/yyyy.git
• xxx é o nome de seu usuário
• yyy é o nome do repositório no github
9. Envie o arquivo criado para o repositório remoto
• git push -u origin master
10. Verifique as alterações no Github
11. Abra seu arquivo README.md e altere o seu conteúdo. Verifique o status.
12. Adicione o arquivo ao estágio "staged”
• git add README.md
13. Verifique o status
14. Remova o arquivo do estágio de “staged”. Remover para não ser commitado.
• git reset HEAD README.md
15. Remova todas as alterações feitas não commitadas no arquivo README.md. Com isso o
arquivo perderá todas as alterações feitas depois do último commit.
• git checkout README.md
Trabalhando com Branch
1. Padrão de nome da branch
• bch_dd-mm-aa (data da criação da branch)
2. Crie uma branch e mude para ela
• git checkout –b nome_branch
3. Crie um novo arquivo chamado index.html
4. Adicione o conteúdo no arquivo.
5. Faça o commit do arquivo. Verifique como fazer no exercício anterior.
6. Agora faça o merge da sua branch com a branch master
• git checkout master
• git merge nome_branch
7. Suba a modificação para o repositório remoto.(Github)
• git push
8. Verifique agora a sua branch maste no Github.
