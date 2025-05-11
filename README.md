# Gitea Docker by Everton Herculano.

Docker compose para Gitea Server MySQL.

<img src="https://about.gitea.com/img/home-screenshot.png" align="center" height="600px"/>


# Para Criar o Banco:

mariadb -u root -p <br>

create database gitea character set utf8 collate utf8_bin; <br>
create user gitea@localhost identified by 'SENHA DO BANCO DE DADOS'; <br>
use gitea; <br>
GRANT ALL ON gitea TO 'gitea'@'%' IDENTIFIED BY 'SENHA DO BANCO DE DADOS'; <br>
GRANT ALL PRIVILEGES ON gitea.* TO 'gitea'@'%' WITH GRANT OPTION; <br>
FLUSH PRIVILEGES; <br>
quit; <br>