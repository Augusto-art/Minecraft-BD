# Projeto Minecraft BD

## Agenda
### -Introdução
### -Desenvolvimento do Trabalho
### -Desafios Encontrados
### -Resultado
### -Referências






## Introdução
### Nesta apresentação será abordado o desenvolvimento de um projeto de inventário inspirado no jogo Minecraft, utilizando tecnologias como HTML, CSS, PHP, Bootstrap e banco de dados MySQL.
### Falaremos sobre o objetivo do inventário, os elementos utilizados no projeto, as dificuldades enfrentadas, as funcionalidades criadas (como cadastrar, editar, excluir e exibir itens) e as principais diferenças entre a versão com arquivo.txt e a versão com banco de dados.

###

## Desenvolvimento do Trabalho
### O que foi utilizado?

### -HTML/CSS: para estrutura e estilização básica do layout inspirado no Minecraft.
### -Bootstrap: para facilitar a responsividade e layout moderno.
### -MySQL: substituindo o inventario.txt para armazenar os dados com mais segurança e flexibilidade.
### -phpMyAdmin: interface visual para criação e manipulação do banco.

## Por que essas tecnologias ?

### PHP e MySQL formam uma base sólida para aplicações web dinâmicas.
### Bootstrap permite interface amigável e responsiva.

## Código usado no MySQL para funcionar a edição e exclusão

### Para que o projeto pudesse editar e excluir corretamente os registros no banco, foi essencial definir um campo Id como chave primária e autoincrementável:

CREATE TABLE mine (
  Id INT(11) NOT NULL AUTO_INCREMENT,
  nome_item VARCHAR(100) NOT NULL,
  qtd_item INT NOT NULL,
  img_item VARCHAR(255) NOT NULL,
  PRIMARY KEY (Id)
);






















