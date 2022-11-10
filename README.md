# Documentação do projeto

## O que é o markdown?

O **markdown** é uma linguagem bem *legal*!

Comando do ~~markdown~~

Documentação do [Markdown](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

1. Abacate
2. Melancia
3. Abacaxi

- Games
- Filmes
- Músicas

Como colocar uma imagem

![Isso é uma imagem](./img/GitHub.jpg)

## Comando do git

...

git clone link_do repositório
...

Codigo html
```html
<html>
....
<html>
....

Codigo JavaScript
```JavaScript
const nome = "maria"
cosole.log(nome)
```
# Revisão dos comandos 

git add nome_de_um_arquivo -> prepara os arquivos para serem comitados (ou seja, gerado uma nova versão)
 
git commit -m "O que você fez?" -> gera uma versão dos arquivos adicionados com o comando do `git add`
 
git push origin main -> envia para o GITHUB
 
git pull origin main -> pega alterações que estão no github, mas não estão na minha máquina.
 
git clone link_do_repositório -> encontrado no botão code de um repositório
 
git status -> exibe o que foi alterado/adicionado/excluido do projeto.



# Branchs

São ramificações do projeto, o qual permite vários desenvolvedores, trabalharem em diferentes funcionalidades, sem bugar a versão estável.

## Principais branchs 

Branch main -> que é a branch principal, ou seja, a branch estável de aplicação. Versão que é disponibilizada aos clientes.

Branch developer -> é a branch utilizada pelos testers. Os quais vão testar as novas funcionalidades, correções de bugs etc.

## Outras branchs

Para cada nova funcionalidade ou correção de bugs é criada uma nova branch.

### Padrões para criar nomes de branchs

!IMPORTANTE! Nomes de branchs não tem acentos ou Ç

Para correção de bugs: fix_identificacao_do_bug
Exemplo: fix_cor_do_cabecalho

Para novas funcionalidades:
feat_identificacao_da_nova_funcionalidade
Exemplo: feat_integracao_com_google, feat_nova_tela_de_contato

Para atualizar documentação: doc_identificacao_da_alteracao
Exemplo: doc_adicionando_nova_imagem

Para criação/alteração de tarefas que não interfere no código:
chore_identificacao_da_modificacao
Exemplo: chore_atualizado_a_versao_do_banco

## Criação de novas branchs

git checkout -b nome_da_nova_branch
Exemplo: git checkout -b fix_botao_da_tela_login
Obs: O ideal é sempre criar as branchs a partir da main.

### Listar as branchs existentes

git branch list

### Trocar de branch
git switch nome_da_branch_que_deseja_entrar
Exemplo 01: git switch fix_botao_da_tela_login
Exemplo 02: git switch main

### Excluir uma branch
git branch -O nome_da_branch_que_deseja_excluir
Exemplo: git branch -O fix_botao_da_tela_login

