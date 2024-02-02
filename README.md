# register-challenge

Este repositório foi criado com o intuito de armazenar o código fonte para a criação da tela de cadastro para o desafio gerado pela empresa Alphacode. A tela de cadastro conta com um formulário onde o usuário deverá digitar seu nome, e-mail, profissão,

# Linguagem utilizada e estrutura do repositório

Este projeto foi desenvolvido utilizando o framework Bootstrap, HTML, CSS, JavaScript e PHP, além de possuir integração com banco de dados MySQL. O repositório foi organizado em duas pastas entituladas "styles" que armazena o código CSS e uma pasta entitulada "assets" para armazenar as imagens que serão utilizadas na tela de cadastro. Cada arquivo possui uma nomeação específica para fácil identificação e distinção

# Estrutura do banco de dados

Para testar o projeto, o usuário deve clonar o repositório Git em sua máquina. Recomenda-se a utilização do programa "XAMPP" como servidor web local. Após iniciar os servidores do XAMPP, procure pela pasta "htdocs" no diretório onde os arquivos do programa estão armazenados. O repositório do jogo deve estar localizado nessa pasta. Acesse o seguinte endereço no seu navegador: http://localhost/register-challenge, que abrirá uma página com os arquivos do projeto. Antes de acessar os arquivos, acesse a url: http://localhost/phpmyadmin/ onde o usuário terá acesso ao banco de dados MySQL. Essa interface do banco de dados possibilitará ao usuário criar o banco "alphacode". Após a criação do banco, utilize a SQL mostrada a seguir para a criação das tabelas. Se nenhuma mensagem de erro aparecer, o usuário pode acessar o arquivo "index.php" para começar seu cadastro!

CREATE TABLE IF NOT EXISTS contatos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    data_nascimento DATE NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    profissao VARCHAR(255),
    telefone VARCHAR(15),
    celular VARCHAR(15)
);

