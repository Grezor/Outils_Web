# configuration de PHP
fichier php.ini dans le dossier a la racine : 
````
output_buffering = Off
expose_php = Off // pour cacher la version de php 
max_execution_time = 30 // 
error_reporting = E_ALL // 
display_errors = On //
log_errors = On // activer les logs d'erreur PHP
date.timezone = Europe/Paris // Modifie le fuseau horaire du serveur

```
## extensions 
````
// a activé
extension=curl
extension=intl
extension=mbstring
extension=pdo_mysql
```

- fichier php.ini rajouter le xdebug
```
// xdebug
zend_extension=xdebug
xdebug.start_with_request=yes
xdebug.client_host=127.0.0.1
xdebug.client_port=9000
xdebug.discover_client_host=1
xdebug.mode=debug
xdebug.remote_handler=dbgp
```