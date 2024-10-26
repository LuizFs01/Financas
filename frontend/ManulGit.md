1 - Criar uma Branch para Cada Programador:
> git checkout -b nome-do-programador

2 - Realizar Alterações no Código:

3 - Depois de fazer as alterações, adicione os arquivos que deseja commitar:
> git add .
Realizar o Commit:

4 - Faça um commit com uma mensagem descritiva:
> git commit -m "Descrição das alterações feitas"

5 - Fazer Pull das Mudanças do Repositório Remoto:
Antes de enviar suas mudanças, é uma boa prática trazer as alterações mais recentes da main (ou da branch principal):
> git checkout main
> git pull origin main

6 - Volte para a sua branch e mescle as alterações:
> git checkout LuizFreitas | > git checkout EduBolha
> git merge main

7 - Resolver Conflitos (se necessário):
> git add .
> git commit -m "Resolvendo conflitos"

8 - Envie suas alterações para o GitHub:
> git push origin nome-do-programador

Fazendo o Merge na Branch Principal
Criar um Pull Request (PR):

No GitHub, vá para a página do repositório e crie um pull request da sua branch para a branch principal. Isso permitirá que você revise as alterações antes de mesclar.
Revisão e Mesclagem:

# Clonar o repositório
git clone https://github.com/SEU_USUÁRIO/financas.git
cd financas/frontend/financas

# Criar uma nova branch
git checkout -b nome-do-programador

# Adicionar e commitar as alterações
git add .
git commit -m "Descrição das alterações feitas"

# Sincronizar com a branch principal
git checkout main
git pull origin main
git checkout nome-do-programador
git merge main

# Resolver conflitos (se houver)
git add .
git commit -m "Resolvendo conflitos"

# Enviar as alterações para o repositório remoto
git push origin nome-do-programador

# Criar um Pull Request no GitHub
Conclusão
Com esses passos e comandos, você e seu colega poderão trabalhar em paralelo em diferentes funcionalidades do projeto sem conflitos. Além disso, o uso de pull requests permite uma revisão de código, o que é sempre uma boa prática em projetos colaborativos.
