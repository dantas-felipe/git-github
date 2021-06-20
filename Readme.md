<h1>Estudando como usar o Git</h1>

<h2>Comandos usados no Git</h2>

<h3>*Configurando Usuário</h3>
  <p>Antes de iniciar o git, temos que identificar para ele que é o usuário. Para isso usamos os comandos abaixo:</p>
  
    git config --global user.name "nome do usuário"
    git config --global user.email "email do usuário"

<h3>*Git init</h3>
  <p>Este comando cria um repositório Git vazio - basicamente um .git</p>
   
    git init

<h3>*Git Clone</h3>
  <p>O Git clone é um comando para baixar o código-fonte existente de um repositório remoto (como o Github, por exemplo).<br>
  Para baixar o código-fonte do repositório remoto (Github):</p>
  
    git clone <https://nome-do-link>

<h3>*Git Branch</h3>
  <p>Com branches, vários desenvolvedores podem trabalhar em paralelo no mesmo projeto simultaneamente.<br>
  Pode-se usar o comando git branch para criar, listar e excluir branches.

  <h4>Criando uma nova branch:</h4>

    git branch <nome-do-branch>
  
  <h4>Alternando entre as branch</h4>
  
    git checkout <nome-do-branch>
  
  <h4>Visualizando as branch</h4>
  
    git branch
  
  <h4>Deletando uma branch</h4>
  
    git branch -d <nome-do-branch>
    
  <h4>Mudando o nome de uma branch</h4>
  
    git branch -M <nome-do-branch>
  
<h3>*Git Status</h3>
  <p>O comando status do Git fornece todas as informações necessárias sobre o branch atual.</p>

    git status
    
<h3>*Git Add</h3>
  <p>Quando criamos, modificamos ou excluímos um arquivo, essas alterações ocorrerão em nosso ambiente local e <br>não serão incluídas no próximo commit (a menos que alteremos as configurações).</p>
  <p>Precisamos usar o comando git add para incluir as alterações de um arquivo em nosso próximo commit.</p>

  <h4>Para adicionar um arquivo:</h4>

    git add <arquivo>
  <h4>Para adicionar tudo de uma vez:</h4>

    git add .
  <p>O comando git add não altera o repositório e as alterações não são salvas até usarmos o git commit.</p>
  
<h3>*Git Commit</h3>
  <p>Este comando é como definir um ponto de verificação no processo de desenvolvimento, para o qual você pode voltar mais tarde, se necessário.</p>

    git commit -m "mensagem explicando a mudança no código"
    
<h3>*Git Push</h3>
  <p>Após confirmar as alterações, a próxima coisa que você deseja fazer é enviar as alterações para o servidor remoto.</p>

  <p>O comando git push envia e salva suas confirmações no repositório remoto.</p>

    git push <remote> <nome-do-branch>
    
<h3>*Git Pull</h3>
  <p>O comando git pull é usado para obter atualizações do repositório remoto.</p>
    
  Comando para atualizar tudo do repositório
  
    git pull 
  
  Comando para atualizar apenas uma branch
  
    git pull origin <nome-da-branch>
    
<h3>*Git Merge</h3>
  <p>Quando você conclui o desenvolvimento em sua branch e tudo funciona bem, a etapa final é mesclar as branches, isso é feito com o comando git merge.</p>

    git merge <nome-da-branch>
  
