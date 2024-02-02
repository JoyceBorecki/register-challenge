# Cadastro de Contatos

Este repositório foi criado para armazenar o código-fonte destinado à implementação da tela de cadastro para o desafio proposto pela empresa Alphacode.

## Linguagem Utilizada e Estrutura do Repositório

O projeto foi desenvolvido utilizando o framework front-end Bootstrap para fornecer estruturas de CSS e HTML, PHP para a lógica do servidor, e integração com o banco de dados MySQL. A interface também faz uso da biblioteca de fontes do Google. A organização do repositório inclui duas pastas principais: "styles", que armazena o código CSS, e "assets", destinada a armazenar as imagens utilizadas na tela de cadastro. Cada arquivo está nomeado de forma específica para facilitar a identificação e distinção.

## Estrutura do Banco de Dados

Para testar o projeto, siga os passos abaixo:

1. Clone o repositório Git para a sua máquina.
2. Recomenda-se o uso do programa "XAMPP" como servidor web local. Inicie os servidores do XAMPP.
3. Localize a pasta "htdocs" no diretório onde os arquivos do programa estão armazenados. O repositório do jogo deve ser colocado nessa pasta.
4. Acesse [http://localhost/register-challenge](http://localhost/register-challenge) no seu navegador para visualizar a página do projeto.
5. Antes de acessar os arquivos, vá para [http://localhost/phpmyadmin/](http://localhost/phpmyadmin/) para acessar a interface do banco de dados MySQL.
6. Crie um banco de dados chamado "alphacode".
7. Utilize a seguinte SQL para criar a tabela necessária:

```sql
CREATE TABLE IF NOT EXISTS contatos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(255) NOT NULL,
    data_nascimento DATE NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    profissao VARCHAR(255),
    telefone VARCHAR(15),
    celular VARCHAR(15)
);
```
8. Se não houver mensagens de erro, acesse o arquivo "index.php" para iniciar o processo de cadastro.
