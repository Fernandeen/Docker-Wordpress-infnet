# Rodando Containers Docker via ansible

Neste projeto estou utilizando 4 roles para descrever as tarefas da automacao:

* Server
* Docker
* Config
* Run

Onde cada role e encarregada de uma etapa do projeto

### A role **Server**:
E encarregada de instalar pacotes basicos na infraestrutura do servidor.
### A role **Docker**

E encarregada de realizar a instalacao do Docker no servidor.

### A role **Config**
Realiza configuracoes basicas de diretorios e usuario no servidor, necessarias para a persistencia de dados do mysql.

### A role **Run**
Executa os containers Mysql e Wordpress de forma integrada, completando desta forma o Deploy.
Esta role tambem configura os containers para inicializarem durante a execucao do sistema atraves do systemd
