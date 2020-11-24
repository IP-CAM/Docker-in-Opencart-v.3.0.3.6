## Docker
- Iniciar Docker
```bash
docker-compose up -d
```

- Primeira vez carregar dados do DB opencart apos iniciar o docker
```bash
docker exec -i mysql-opencart mysql -uroot -p1234 < db/opencartclean.sql
```

- Acessar opencart
http://localhost
http://localhost/admin

User: Admin
Password: 1234


- Parar Docker
```bash
docker-compose down
```

- Reiniciar Nginx
```bash
docker exec -it nginx-opencart service nginx restart
```