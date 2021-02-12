# Estudo sobre a  ferramenta de controle de migração de base de dados Phinx

### Install & Run

1. `git clone https://github.com/robmorgan/guestbook-tutorial.git`

2. Migrations para aplicações PHP com Phinx

*Instalação
 
path_projeto:$ php composer.phar require robmorgan/phinx

path_projeto:$ mkdir db/migrations

path_projeto:$  php vendor/bin/phinx init

*Configurando o Phinx (phinx.yml)
 
No arquivo de configuração em environments deve conter as configurações para conexão com banco de dado	
	
Escrevendo migrations

path_projeto:$ php vendor/bin/phinx create PrimeiraMigrate

 20210212233848_primeira_migrate.php foi criado no diretório db/migrations , lá será escrito a migration

*Executando migrations

path_projeto:$ php vendor/bin/phinx migrate

path_projeto:$ php vendor/bin/phinx status

