Migrate Wordpress
=================

Como migrar instalaciones de Wordpress entre servidor (local - remoto)  
### Recomendaciones

Tener copia de seguridad de la Base de Datos y de los archivos
Configurar Wordpress, archivo: wp-config.php
Actualizar URLs de Wordpress

	```
    UPDATE wp_options SET option_value = REPLACE(option_value,'dominio_viejo','dominio_nuevo');
    ```
    
    ```
    UPDATE wp_posts SET post_content = REPLACE(post_content,'dominio_viejo','dominio_nuevo');
    ```

    ```
    UPDATE wp_posts SET guid = REPLACE(guid,'dominio_viejo','dominio_nuevo');
    ```

    Opcional
    ```
    UPDATE wp_postmeta SET meta_value = REPLACE(meta_value,'dominio_viejo','dominio_nuevo');
    ```
    



