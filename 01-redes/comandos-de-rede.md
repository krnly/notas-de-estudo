# 🌐 Comandos de rede básicos

> Anotações de estudo — 12/09/2026

## Comandos

| Comando | O que faz |
|---|---|
| `ip a` | descobre o IP da máquina na rede (procurar o campo `inet`) |
| `ping google.com` | testa a conexão (`google.com` é só um exemplo) |
| `ss -tuln` | mostra as portas abertas |

> `ss -tuln`: `-t` TCP, `-u` UDP, `-l` só quem está escutando (listening), `-n` mostra números em vez de nomes *(complemento)*

## Portas comuns

| Porta | Serviço | Para que serve |
|---|---|---|
| 22 | SSH | acesso remoto |
| 80 | HTTP | site sem criptografia |
| 443 | HTTPS | site seguro (criptografado) |

## Lendo uma linha do `ss -tuln`

```
tcp   LISTEN   0   4096   127.0.0.54:53   0.0.0.0:*
```

- `tcp` → tipo de conexão
- `LISTEN` → serviço esperando conexão
- `127.0.0.54:53` → **IP local** + **porta 53**
  - `127.x.x.x` é o endereço de loopback: só aceita conexões da própria máquina *(complemento)*
  - porta 53 = **DNS**
- `0.0.0.0:*` → qualquer origem pode se conectar *(complemento)*

## DNS

Sistema que **traduz** nomes em endereços IP.

`google.com` → `142.250.x.x`
