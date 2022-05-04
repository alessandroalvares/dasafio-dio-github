	Chave SSH e Token

ssh-keygen -t ed25519 -c *e-email (vai gerar a chave publica e a privada, após vai pedidir senha, após ir na pasta que gerou pelo comando *cd ..., ls para ver as chaves, após ver a chave pública, *cat id_ed25519.pub, pegar a chave a jogar no github)

eval $(ssh-agent -s)

ssh-add id_ed25519 (aqui vai passar a chave privada), vai pedir a senha.


git config --global user.email "*email-do-github"
OBS: git config --global --unset user.email "*email-do-github" (aqui vai apagar, para poder mudar, tem que fazer o passo anterior).

git config --global user.name "*name-github"
OBS: git config --global --unset user.name  "*name-do-github" (aqui vai apagar, para poder mudar, tem que fazer o passo anterior).


git init (inicializa o git na pasta em questão)

ls -a (lista arquivos ocultos)

git add *nome do arquivo ou pasta

git commit -m "adiciona"

git remote add origin *link do repositorio no github

git remote -v

git push origin master (empurra o commit ao ao github)


git pull origin master (puxa o commit ao seu diretorio)



git clone *(url da pasta que quer clonar)

git status (ver o status da pasta)

git config --list 


git log
git log --oneline
git log -p
