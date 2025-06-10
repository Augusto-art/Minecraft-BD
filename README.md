# Projeto Minecraft BD <br>

## Agenda
### -Introdução
### -Desenvolvimento do Trabalho
### -Desafios Encontrados
### -Resultado
### -Referências <br><br><br>



## Introdução
### Nesta apresentação será abordado o desenvolvimento de um projeto de inventário inspirado no jogo Minecraft, utilizando tecnologias como HTML, CSS, PHP, Bootstrap e banco de dados MySQL.
### Falaremos sobre o objetivo do inventário, os elementos utilizados no projeto, as dificuldades enfrentadas, as funcionalidades criadas (como cadastrar, editar, excluir e exibir itens) e as principais diferenças entre a versão com arquivo.txt e a versão com banco de dados. <br><br><br>


## Desenvolvimento do Trabalho <br>
### O que foi utilizado?<br>

### -HTML/CSS: para estrutura e estilização básica do layout inspirado no Minecraft.
### -Bootstrap: para facilitar a responsividade e layout moderno.
### -MySQL: substituindo o inventario.txt para armazenar os dados com mais segurança e flexibilidade.
### -phpMyAdmin: interface visual para criação e manipulação do banco.<br><br><br>

## Por que essas tecnologias ?<br>

### PHP e MySQL formam uma base sólida para aplicações web dinâmicas.
### Bootstrap permite interface amigável e responsiva. <br><br><br>

## Código usado no MySQL para funcionar a edição e exclusão<br>

### Para que o projeto pudesse editar e excluir corretamente os registros no banco, foi essencial definir um campo Id como chave primária e autoincrementável:<br>

CREATE TABLE mine (<br>
  Id INT(11) NOT NULL AUTO_INCREMENT,<br>
  nome_item VARCHAR(100) NOT NULL,<br>
  qtd_item INT NOT NULL,<br>
  img_item VARCHAR(255) NOT NULL,<br>
  PRIMARY KEY (Id)<br>
); <br>

### Isso permite que cada item seja identificado de forma única via URL, como editar.php?id=3 ou excluir.php?id=4.<br><br><br>

## Resultado<br>

### Abaixo, mostramos trechos importantes do projeto e o que eles fazem:<br>

### Cadastro (cadastro.php)<br>

 ![cadastro BD](https://github.com/user-attachments/assets/827b26ee-98df-49be-b363-4ffe370391e2)<br>


### Esse código cadastra um item com nome, quantidade e imagem (via URL) no banco MySQL.<br><br>

## Inventário (inventario.php)<br>

![inventario Bd](https://github.com/user-attachments/assets/741875c2-3bbc-4331-b121-5fe488135d87) <br><br>

### Esse trecho consulta os itens cadastrados no banco e os exibe nos 36 slots do inventário. <br><br>

## Edição (editar.php)<br>

![editar BD](https://github.com/user-attachments/assets/c5a3026e-404b-463f-92dc-33dae94c1901) <br><br>

### Esse código atualiza os dados de um item específico com base no Id recebido pela URL.<br><br>

## Exclusão (excluir.php)<br>

![Excluir Bd](https://github.com/user-attachments/assets/fcff58c0-b66a-49d7-8117-a28b11358bb4) <br><br>

### Esse trecho deleta um item específico do banco, também usando o Id.<br><br>

## Diferenças principais: .txt vs MySQL<br>

## Antes (arquivo.txt):<br>
### -Os dados eram salvos em texto plano no formato nome|quantidade|imagem.<br>
### -Para sobrescrever ou editar, era necessário reprocessar o arquivo inteiro.<br>
### -Menos seguro e difícil de escalar.<br>

## Agora (MySQL):<br>
### -Os dados são armazenados em colunas organizadas.<br>
### -A edição e exclusão são simples e diretas.<br>
### -Fácil de integrar com painéis, relatórios e outros sistemas.<br>
### -Permite o uso de URLs remotas para imagens.<br><br><br>

## Desafios Encontrados<br>

### -Conectar corretamente o PHP com o banco de dados.<br>
### -Corrigir erro de nomes de colunas na tabela.<br>
### -Manter o layout antigo mesmo com novas funcionalidades (editar e excluir).<br><br><br>

## Referências<br>

### -W3Schools - PHP e MySQL  Link: https://www.w3schools.com <br>
### -Documentação Bootstrap Link: https://getbootstrap.com <br>
### -Minecraft Wiki – para imagens e inspiração   Link: https://minecraft.fandom.com/wiki/Minecraft_Wiki  <br>
### -ChatGPT – auxílio na explicação e depuração de códigos   Link:https://chat.openai.com






















































