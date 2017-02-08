# codeigniter3
# Codeigniter 3.1.3
# removed index.php from url
Reference: 
https://www.formget.com/codeigniter-htaccess-remove-index-php/

Add below code to a new file .htaccess

<IfModule mod_rewrite.c>
RewriteEngine On
RewriteBase /codeigniter3/
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule ^(.*)$ index.php/$1 [L]
</IfModule>

