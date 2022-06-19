# php_ordemservicos
Sistema de Ordem de Serviços em PHP

Requisitos: 
Servidor Linux com cPanel (cPanel.net), Apache, Php 5.3+, Apache, Banco 
MySQL, phpMyAdmin 

Configuração Básica e Instalação do Banco de Dados
Acesse o cPanel - o gerenciador de Banco de dados MySQL, crie o Banco de 
Dados MySQL, o Usuário de acesso ao banco + senha, depois atribua todas as 
permissões do usuário ao Banco. 
Abra o phpMyAdmin, selecione o banco que criou e importe a base de dados 
(BANCO-DE-DADOS.sql) que está dentro da pasta /INSTALACAO 
Arquivo de conexão com o banco: 

Na pasta /Script, acesse o seguinte arquivo: 
/application/config/database.php 
Edite as informações do banco de dados, usuário e senha para conexão com o 
banco entre as linhas 51 a 54 depois salve e feche. 
$db['default']['hostname'] = 'localhost'; $db['default']['username'] = 
'USUARIOCPANEL_USUARIOBANCO'; $db['default']['password'] = 'SENHA'; 
$db['default']['database'] = 'USUARIOCPANEL_BANCO'; 
Também acesse o seguinte arquivo /application/config/config.php 
Edite a URL do de instalação do script com pasta caso instale em uma pasta, que 
está na linha 17. 
$config['base_url'] = 'http://www.SEUSITE.com.br/PASTA'; //INSIRA AQUI A URL 
DO SITE COM A PASTA DE INSTALAÇÃO 
Agora compacte o conteúdo da pasta /Script em um arquivo .zip e faça o upload 
deste arquivo zipado pelo Gerenciador de Arquivos do cPanel e assim que 
finalizar o upload descompacte o .zip lá pelo gerenciador mesmo. 
E pronto! 

Acesso: 
www.seusite.com/PASTA 
Email: admin@admin.com Senha: 123456 
O logotipo se encontra dentro da pasta assets/img. Caso queira trocá-lo, basta 
substituir pelo logo desejado com o mesmo nome (logo.png
