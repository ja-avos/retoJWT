# Reto JWT

Pasos para probar:

Desde el directorio del proyecto:

1. Ejecutar npm install
2. Ejecutar npm start

3. Abrir las colecciones de /postman_collections/ en Postman.
4. Probar cada colección manualmente (no probar de forma automática).

##### Se puede evidenciar en las colecciones que solo los usuarios con ciertos roles pueden ejecutar ciertas acciones. Las capacidades de los roles son las siguientes:
* none: ["viewStores", "viewProducts"],
* client: ["viewStores", "viewClient", "viewProducts", "viewCart", "buyProducts", "checkout", "editUser"],
* owner: ["viewStores", "viewProducts", "addProduct", "deleteProduct", "editStore"],
* admin: ["viewClients", "viewStores", "viewProducts", "addProduct", "editStores"]

#### Nota
En postman cada vez que se ejecuta la petición de login se actualiza la variable de colección *rol_token* que será usada en las siguientes peticiones en el header de *Authorization*. No hay que modificarla.
