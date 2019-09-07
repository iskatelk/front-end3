# front-end3
Приложение Angular демонстрирует поиск строк по различным словам на латинице и на русском, а также поиск по цифрам.
Приложение грузит список, передаваемый по api с одного сайта из интернета. Выводит имя и email различных людей.
Программа тестировалась на openserver. По пути localhost/front-end4/index.html. В папке front-end4 находятся файлы .htaccess, index.html.
Все остальные файлы должны быть скопированны в папку localhost (корень хоста)
Содержимое .htacctss.......
<IfModule mod_rewrite.c>
    RewriteEngine on
    # Don't rewrite files or directories
    RewriteCond %{REQUEST_FILENAME} -f [OR]
    RewriteCond %{REQUEST_FILENAME} -d
	Header set Access-Control-Allow-Origin "*"
	RewriteRule ^ - [L]
    
    # Rewrite everything else to index.html
    # to allow html5 state links
    RewriteRule ^ index.html [L]
</IfModule>

Содержимое index.html......
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>FrontEnd4</title>
  <base href="/">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="icon" type="image/x-icon" href="favicon.ico">
<link rel="stylesheet" href="styles.3ff695c00d717f2d2a11.css"></head>
<body>
  <app-root></app-root>
<script src="polyfills-es5.3aa54d3e5134f5b5b842.js" nomodule defer></script><script src="polyfills-es2015.fd917e7c3ed57f282ee5.js" type="module"></script><script src="runtime-es2015.24b02acc1f369d9b9f37.js" type="module"></script><script src="main-es2015.b4399c49820a5d4f76f8.js" type="module"></script><script src="runtime-es5.24b02acc1f369d9b9f37.js" nomodule defer></script><script src="main-es5.b4399c49820a5d4f76f8.js" nomodule defer></script></body>
</html>
-----------------------------------------------------------------------------------------------------------------
