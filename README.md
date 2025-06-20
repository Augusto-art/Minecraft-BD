# Projeto Minecraft BD <br>

## Agenda
### -Introdução
### -Desenvolvimento do Trabalho
### -Desafios Encontrados
### -Resultado
### -Referências <br><br><br>



## Introdução
### Nesta apresentação será abordado o desenvolvimento de um projeto de inventário inspirado no jogo Minecraft, utilizando tecnologias como HTML, CSS, PHP, Bootstrap e banco de dados MySQL.
### Falaremos sobre os elementos utilizados no projeto, as dificuldades enfrentadas, as funcionalidades criadas (como cadastrar, editar, excluir e exibir itens) e as principais diferenças entre a versão com arquivo.txt e a versão com banco de dados. <br><br><br>


## Desenvolvimento do Trabalho <br>
### O que foi utilizado?<br>

### -HTML/CSS: para estrutura e estilização básica do layout inspirado no Minecraft.
### -Bootstrap: para facilitar a responsividade e layout moderno.
### -MySQL: substituindo o inventario.txt para armazenar os dados com mais segurança e flexibilidade.
### -phpMyAdmin: interface visual para criação e manipulação do banco.<br><br><br>

## Por que essas tecnologias ?<br>

### PHP e MySQL formam uma base sólida para aplicações web dinâmicas.
### Bootstrap permite interface amigável e responsiva. <br><br><br>

## Estrutura da Tabela MySQL<br>

### Para que as ações de editar e excluir funcionasse corretamente, foi criada a seguinte estrutura:<br>

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
### -Menos seguro e difícil de escalar.<br><br>

## Agora (MySQL):<br>
### -Os dados são armazenados em colunas organizadas.<br>
### -A edição e exclusão são simples e diretas.<br><br><br>


## Desafios Encontrados (Principais)<br>

### -Ficar trocando de máquina.<br>
### -Manter o layout antigo mesmo com novas funcionalidades (editar e excluir).<br><br><br>

## Referências<br>

### -Documentação Bootstrap Link: https://getbootstrap.com <br>
### -Minecraft Wiki – para imagens e inspiração   Link: https://minecraft.fandom.com/wiki/Minecraft_Wiki  <br>
### -ChatGPT – auxílio na explicação e depuração de códigos   Link:https://chat.openai.com<br><br><br>

## Prints do Inventário<br>

![Inventario  at](https://github.com/user-attachments/assets/551590bc-b760-4a83-b12f-14b9b9c6be3f) <br>

![edição inve](https://github.com/user-attachments/assets/d5bbab73-ddf2-403a-9a3a-04bb5e8ffa96) <br>

![Cadastro immm](https://github.com/user-attachments/assets/cfe9cea0-5e80-48f0-98e6-6cc4e6ed530c) <br>

![xamp edit](https://github.com/user-attachments/assets/3a3b8b7f-ea09-4061-8afa-de42ec6c50ca)




















































