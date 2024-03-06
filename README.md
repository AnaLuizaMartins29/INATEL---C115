## Trabalho Docker C115
> Ana Luiza Martins 

### Descrição 
A aplicação simula uma comunicação cliente servidor, onde o cliente esta fornecendo os dados pelo frontend e o servidor é o bnco de dados, que armazena as respostas enviadas.

### Tecnologias
- Docker compose
- Python
- Nginx
- PostgresSQL
- HMTL + CSS

### Execução

Para subir o container
```
docker compose up -d
```

Para verificas os dados do banco
> Todos os dados
```
docker compose exec db psql -U postgres -d trabalho1 -c 'select * from perguntas'
```
> Somente as respostas
```
docker compose exec db psql -U postgres -d trabalho1 -c 'select respostas from perguntas'
```

Para parar a aplicação
```
docker compose down
```

Se desejar ver os serviços que estão rodando
```
docker compose ps
```
