# configuration du php.ini 
```
Ajouter ou a décommenter dans votre fichier 
```
```ini
output_buffering = Off # tampon de sortie ob_clean() ...
expose_php = Off # pour cacher la version de php 
max_execution_time = 30 # Fixe le temps maximal d'exécution d'un script, en secondes
error_reporting = E_ALL # Fixe le niveau de rapport d'erreurs PHP
display_errors = On #
log_errors = On # activer les logs d'erreur PHP
date.timezone = Europe/Paris # Modifie le fuseau horaire du serveur

# Extensions [a activer]
extension=curl 
extension=intl
extension=mbstring
extension=pdo_mysql

extension=php_openssl.dll # update composer

# XDEBUG
zend_extension=xdebug
xdebug.start_with_request=yes
xdebug.client_host=127.0.0.1
xdebug.client_port=9000
xdebug.discover_client_host=1
xdebug.mode=debug
xdebug.remote_handler=dbgp
```

https://stackoverflow.com/questions/65162856/xdebug-step-debug-could-not-connect-to-debugging-client-tried-localhost900
