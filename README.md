# 🐳 Nginx Estático com Docker

Servidor web estático com Nginx rodando em Docker, criado como projeto de aprendizado de Linux e Docker.

## Tecnologias

- Docker + Docker Compose
- Nginx (alpine)
- HTML

## Como rodar

**Pré-requisitos:** Docker instalado

```bash
# Clone o repositório
git clone https://github.com/devluiscavalcante/nginx-com-docker.git
cd nginx-com-docker

# Suba o container
docker compose up -d
```

Acesse **http://localhost:8080** no navegador.

## Comandos úteis

```bash
# Ver container rodando
docker ps

# Ver logs do Nginx
docker logs meu-nginx

# Entrar no container
docker exec -it meu-nginx sh

# Validar configuração do Nginx
docker exec meu-nginx nginx -t

# Parar o container
docker compose down
```

## 📚 O que aprendi

- Subir containers com Docker Compose
- Mapear portas e volumes
- Customizar configuração do Nginx via `nginx.conf`
- Criar página de erro 404 personalizada
- Validar configuração do Nginx sem reiniciar o container