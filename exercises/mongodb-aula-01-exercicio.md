# MongoDB - Aula 01 - Exercício
autor: Saulo Mendes Martins

## Importando os restaurantes

[10:52 PM]-[root@midia]-[/var/www/beMean/data/db] 
# mongoimport --db beMean --collection restaurantes --drop --file ../../restaurantes.json 
connected to: 127.0.0.1
Mon Nov  9 22:52:28.625 dropping: beMean.restaurantes
Mon Nov  9 22:52:31.005         Progress: 7285007/11880944  61%
Mon Nov  9 22:52:31.006             13500   4500/second
Mon Nov  9 22:52:32.155 check 9 25359
Mon Nov  9 22:52:32.172 imported 25359 objects


## Contando os restaurantes

MongoDB shell version: 2.4.14
connecting to: test
> use beMean;
switched to db beMean
> db.restaurantes.find({}).count()
25359
