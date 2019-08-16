
# Erros Conhecidos e Soluções

Ao apresentar Too Many Request, executar os comandos abaixo.

Dentro do servidor
```
docker exec -it dati-php bash
php artisan cache:clear
php artisan config:clear
php artisan route:clear
```
Caso o problema não seja solucionado, acessar a pasta storage/framework/cache/data e remover todas as pastas dentro, ou apagar a pasta data, neste caso necessário incluir o .gitignore.

```
*
!.gitignore
```
