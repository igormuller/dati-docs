# Comando para inclusão de nova preferência no banco

Abaixo INSERT para as preferencias, atentar-se a preference_model, e a tabela a qual refere-se o model.

```
INSERT INTO `dati`.`preferences` (`preference_model_id`, `preference_model`, `preference_description`, `preference_value`, `preference_status`)
  select distinct id, 'customer', 'numerarioICMSDebit', '', '1'
  from `dati`.`customers`;
```
