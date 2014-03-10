# Migrate Wordpress

how to migrate wordpress from localhost to server

1. Tener copia de seguridad de la Base de datos y de los archivos
2. Configuracion Wordpress
    wp-config.php
    
    
3. Actualizar URLs de Wordpress
    UPDATE wp_options SET option_value = REPLACE(option_value,'dominio_viejo','dominio_nuevo');
    UPDATE wp_posts SET post_content = REPLACE(post_content,'dominio_viejo','dominio_nuevo');
    UPDATE wp_posts SET guid = REPLACE(guid,'dominio_viejo','dominio_nuevo');
    UPDATE wp_postmeta SET meta_value = REPLACE(meta_value,'dominio_viejo','dominio_nuevo');
    



