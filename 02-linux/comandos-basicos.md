# 🐧 Comandos básicos de Linux

> Anotações de estudo — 12/09/2026

## Navegação

| Comando | O que faz |
|---|---|
| `ls` | lista os arquivos da pasta (também serve pra confirmar que algo foi criado) |
| `cd pasta` | entra na pasta |
| `cd ~` | volta para a pasta pessoal (home) |
| `cd ..` | sobe um nível *(complemento)* |
| `pwd` | mostra onde estou |
| `whoami` | mostra o usuário |
| `clear` | limpa a tela |

## Arquivos e pastas

| Comando | O que faz |
|---|---|
| `mkdir pasta` | cria uma pasta |
| `touch arquivo.txt` | cria um arquivo vazio |
| `cp origem destino` | copia |
| `mv antigo novo` | renomeia ou move um arquivo |
| `rm arquivo.txt` | deleta (⚠️ não vai pra lixeira) |
| `find ~ -name "nome.txt"` | busca um arquivo a partir da pasta indicada |

## Editor nano

- `nano arquivo.txt` → abre e edita o arquivo
- `Ctrl + X` → sai (ele pergunta se quer salvar)

## Atalhos

- `Ctrl + Alt + T` → abre o terminal

## Dicas

- Colocar uma `/` no final do nome indica que é uma **pasta**. Ex.: `ls Linux/`
- Renomear uma pasta: `mv Linux/ Lin` → a pasta `Linux` passa a se chamar `Lin`
