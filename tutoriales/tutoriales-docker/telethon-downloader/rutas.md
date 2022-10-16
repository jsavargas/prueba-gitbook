---
description: Rutas y como descargar archivos por tipo de archivos
---

# Rutas

En **/config** tenemos el archivo "config.ini" donde podremos agregar rutas especiales por extension de archivos.&#x20;

Ejemplo: si queremos que los archivos mp3 se descargen en otra ruta, aca se lo podemos indicar

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

En este ejemplo:

* Los archivos epub se descargarán en  /download/epub&#x20;
* Los archivos pdf se descargarán en /download/pdf&#x20;
* Los archivos cbr se descargarán en /download/pdf&#x20;
* Y los archivos mp3 se descargarán en /download/mp3&#x20;

Tambien podemos descargar en rutas dependiendo del nombre de archivo usando expresiones regulares

Ejemplo: si queremos que el archivo "_**Mi serie favorita S01E01.mkv**_" se descarge en la carpeta series "_**/series/Mi Serie Favorita (2022)/**_" podemos crear una regla para que todos los archivos que contengan "Mi Serie Favorita" se descargen directamente en esa ruta.

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

En mi ejemplo, los archivos que dicen "_**#PobreNovio \_ Capítulo 98 \_ Mega.mp4**_" se descargan directamente en "_**/series/Poor Boyfriend (2021)/Season 01**_". Para esto tuve que agregar una nueva ruta en el YML:

* **/mnt/user/media/media/series/:/series**

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption><p><em><strong>/series/Poor Boyfriend (2021)/Season 01</strong></em></p></figcaption></figure>

