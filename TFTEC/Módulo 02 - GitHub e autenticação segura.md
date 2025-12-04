# Módulo 01 - Introdução ao Git e conceitos básicos.md

## Configurando o ambiente

- Mudando o diretório
```bash
cd "/g/Outros computadores/Meu laptop/SSD Externo/Education/GitHub"
```

- Criando a árvore de trabalho (diretório)

```bash
mkdir TFTEC
```

- Entrando no diretório
```bash
cd TFTEC
```

- Iniciando o git com a branche main (e não master)
```bash
git init -b main
```

- Criando o markdown

```bash
touch "Módulo 01 - Introdução ao Git e conceitos básicos.md"
```
## Lab 04

- Configurando nome e e-mail globalmente.

```bash
git config --global user.name "Felipe da Rocha Ferreira"
git config --global user.email "felipe179971@hotmail.com"
```
- Chegando as informações (precisar colocar 'q' para sair).

```bash
git config --list
```

- Configurando nome e e-mail localmente (vale apenas para um repositório específico).

Como esqueci de já criar com a branch se chamando 'main' (`git init -b main`), precisei renome depois. 
```bash
mkdir teste_config_local
cd teste_config_local
git init
git branch -m main
git config user.name "local"
git config user.email "local@hotmail.com"
git config --list --shwo-origin
```
Saindo do diretório de teste e excluíndo a pasta
```bash
cd "/g/Outros computadores/Meu laptop/SSD Externo/Education/GitHub/TFTEC"
rm -rf "/g/Outros computadores/Meu laptop/SSD Externo/Education/GitHub/TFTEC/teste_config_local"

```
## Lab 05 - Criar repositório local, fazer commits e visualizar logs
- Criando pasta do projeto
```bash
mkdir meu-projeto
cd meu-projeto
```
- Iniciando o repositório
```bash
git init -b main
```
- Criando arquivo de teste
Será um markdonw contendo o título 'Meu Projeto' dentro.
```bash
echo "# Meu Projeto" > README.md
```
- Vendo os arquivos que tem na pasta (menos os ignorados. para ver esses, tem que colcoar `ls -la`)
```bash
ls
```
- Abrindo o conteúdo do 'README.md'
```bash
cat README.md
```
- Verificando que 'README.md' existe mas ainda não está sendo rastreado (sem controle de versão - untracked).
```bash
git status
```
- Adicionando o arquivo para ser tracked (alterações acompanhadas). Adicionando apenas em um arquivo.
```bash
git add README.md
git status
```
- Adicionando comentário ('-m' = mensagem que vamos adicionar)
```bash
git commit -m "Primeiro commit: adicionei README"
git status
```
- Verificando o histórico de commits ('oneline' é para ver as mudanças)
```bash
git log --oneline
```
- Fluxo geral: 
    - git add: prepara as mudanças;
    - git commit: registra oficialmente no histórico;
    - git log: permite acompanhar que fez o quê e quando.
Saindo do diretório de teste e excluíndo a pasta
```bash
cd "/g/Outros computadores/Meu laptop/SSD Externo/Education/GitHub/TFTEC"
rm -rf "/g/Outros computadores/Meu laptop/SSD Externo/Education/GitHub/TFTEC/teste_config_local"

```


