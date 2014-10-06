Migrate Wordpress
=================

Como migrar instalaciones de Wordpress entre servidor (local - remoto)  
### Recomendaciones

Tener copia de seguridad de la Base de Datos y de los archivos
Configurar Wordpress, archivo: wp-config.php
Actualizar URLs de Wordpress

>
>	1. 	UPDATE wp_options SET option_value = REPLACE(option_value,'dominio_viejo','dominio_nuevo');
>	2.	UPDATE wp_posts SET post_content = REPLACE(post_content,'dominio_viejo','dominio_nuevo');
>	3.	UPDATE wp_posts SET guid = REPLACE(guid,'dominio_viejo','dominio_nuevo');
>	4. 	Opcional
		~~~
    	UPDATE wp_postmeta SET meta_value = REPLACE(meta_value,'dominio_viejo','dominio_nuevo');
    	~~~
 

    



