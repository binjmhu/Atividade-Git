# __Tutorial de Git e Github__
## __Integração com repositorios online no Git e Github__

### O que veremos nesse tutorial:
- Formas de criar um repositorio remoto e como anexar em um repositorio local
- Os principais comandos para enviar e receber codigos remotos
- Resoluções de determinados problemas que aparecem pelo caminho!


### Como criar um repositorio remoto
- Nessa etapa do desenvolvimento é possivel que você já tenha codigos e um versionamento do git localmente, o passo é mandar esse codigo para o repositorio remoto, para ser utilizado em qualquer lugar e trazer mais segurança ao usuario, empresas, etc.
- Após Criar uma conta no github, e criar um repositorio remoto, é possivel linkar um versionamento local com esse repositorio.

![Criação de repositorio remoto](https://imgur.com/a/AWhBdw7)

### Principais Comandos
- git remote add origin <Url_do_repositorio> ->
Com esse comando, é possivel salvar o progresso feito localmente em um repositorio remoto, refereciando pelo nome origin.

- git pull origin master -> 
Esse comanndo será utilizado para receber as informações que já está no repositorio remoto, e trazer para o local, assim é possivel atualizar seu codigo com outras alterações que estavam mais atualizadas.

- git push origin master -> 
Com esse comando é possivel enviar suas alterações, antes preparadas e commitadas, para o repositorio remoto, salvando as alterações.

- git branch / git branch -A -> 
Nos repositorios remotos é utilizado um sistema de branches, que seriam ramificações da branch principal do repositorio, onde é feita alterações a parte do resto do codigo, assim evitando conflitos na hora de juntas as partes, e deixando o processo de desenvolvimento menos complicado, além do comando com a terminação -A, que traz a lista de todas as branchs.

- git switch <nome_da_branch> ->
Utilizando esse comando é possivel alterar as branchs já criadas, assim tem um controle das alterações, assim sendo possivel modificar varias funcionalidades sem quebrar outras

- git checkout -b <nome_da_branch> -> 
Um jeito descompliado de criar branchs e dar um 'switch' direto, facilitando a vida do usuario
