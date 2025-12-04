# Módulo 02 - GitHub e autenticação Segura.md

## Configurando o ambiente

- Mudando o diretório
```bash
cd "/g/Outros computadores/Meu laptop/SSD Externo/Education/GitHub"
```

## Lab 03 - Testar conexão SSH com GitHub

- Testando conexão.

Na primeira vez que rodar, vai perguntar se a chave host é confiável (digitar yes)
```bash
ssh -T git@github.com
```
- Iniciando o git com branche main
```bash
git init -b main
```
- Fazendo conexão com repositório no GitHub (conexão ssh)
```bash
git remote add origin https://github.com/felipe179971/GitHub.git
```
- Criando arquivo README.md
```bash
echo "# Repositório GitHub" > README.md
```
- Adicionando ao controle de versão e comentando
```bash
git add .
git commit -m "primeiro commit"
```
- Enviando para o repositório (push)
```bash
git push -u origin main
```
