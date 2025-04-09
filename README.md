# SCRIPT DE CRIAÇÃO DE USUÁRIOS, GRUPOS E PERMISSÕES NO LINUX


## Descrição:
Este script automatiza a configuração de uma estrutura organizacional em um sistema Linux. Ele cria diretórios, grupos e usuários, além de definir permissões específicas para cada grupo, simulando uma divisão por setores.


## O que faz:
1. **Cria diretórios:**
   - `/publico`
   - `/adm`
   - `/ven`
   - `/sec`

2. **Cria grupos:**
   - `GRP_ADM`
   - `GRP_VEN`
   - `GRP_SEC`

3. **Cria usuários com senha criptografada:**
   - Grupo ADM: `carlos`, `maria`, `joao`
   - Grupo VEN: `debora`, `sebastiana`, `roberto`
   - Grupo SEC: `josefina`, `amanda`, `rogerio`

5. **Define permissões:**
   - Diretórios `/adm`, `/ven`, `/sec`: somente o dono e o grupo têm acesso (`chmod 770`)
   - Diretório `/publico`: acesso liberado para todos os usuários (`chmod 777`)


## Como usar:
```bash
# 1. Dê permissão de execução ao script
chmod +x nome_do_arquivo.sh

# 2. Execute o script como root
./nome_do_arquivo.sh
```

## Requisitos:
Sistema Linux com os seguintes pacotes instalados:
- bash
- openssl

## Aplicações:
Ideal para ambientes corporativos, educacionais ou laboratoriais, onde há múltiplos usuários e é necessário controlar o acesso por setor ou grupo de trabalho.

## Autor
Script criado para fins educacionais e organizacionais.


#### **💻Feito por Guilherme Gugelmin** 


