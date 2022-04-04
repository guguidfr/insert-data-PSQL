# insert-data-psql
- Clona el proyecto:
```
git clone https://github.com/guguidfr/insert-data-PSQL.git
cd insert-data-PSQL
```
- Edita el fichero 'hosts' con la dirección IP del servidor sobre el que quieres ejecutar el rol
```
vim hosts
```
- Edita las variables 'nombre_bd', 'from' y 'ruta_sql'.
  - nombre_bd = nombre de la base de datos que quieras crear (si no existe) y sobre la que quieres insertar datos
  - from = ruta del archivo .sql que quieres ejecutar. Por defecto es la ruta al fichero ```/roles/import/files/file.sql```
  - ruta_sql = ubicación en la que quieres guardar el archivo .sql en el servidor. Este fichero se borrará el final de la ejecución. Comenta la task correspondiente en ```/roles/import/tasks/main.yml``` si no quieres que esto ocurra.
```
vim ./roles/import/vars/main.yml
```
