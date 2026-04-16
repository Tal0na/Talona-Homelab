# 🏠 Home Lab - Atualização dos Containers

Este documento descreve o processo de atualização dos containers Docker no servidor Debian.

---

## 🖼️ Arquitetura do Home Lab

![Arquitetura](img/image.png)

---

## 🔄 Atualização dos serviços

Execute os comandos abaixo no diretório do projeto:

```bash
docker compose pull
docker compose down
docker compose up -d
```

### 📌 Explicação

* `docker compose pull` → baixa as imagens mais recentes
* `docker compose down` → para e remove os containers atuais
* `docker compose up -d` → sobe os containers atualizados em segundo plano

---

## 🧠 Observações

* O servidor roda múltiplos serviços via Docker (ex: Pi-hole, FreshRSS, Navidrome, Jellyfin)
* Acesso remoto é feito utilizando Tailscale
* Todos os serviços são mantidos atualizados manualmente com os comandos acima

---
