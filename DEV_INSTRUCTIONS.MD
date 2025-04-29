# INICIAR CONTEINERS

```bash
docker-compose up --build
```

# ACESSANDO OS SERVIÇOS


Frontend (Vue.js): http://localhost:8081

Backend (Spring Boot): http://localhost:8080

Banco de Dados (PostgreSQL): localhost:5432 (com usuário usuario e senha senha).

# REINICIANDO O DOCKER COMPOSE

Para parar e remover os containers
```bash
docker-compose down
```

Para reiniciar com novas alterações
```bash
docker-compose up --build
```