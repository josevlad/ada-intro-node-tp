# Node Trabajo Final

## Entrega

- Fecha: 29 de Julio de 2021

---

## Consigna

El objetivo del trabajo final es hacer un servidor que pueda exponer una API para los usuarios, permitiendo consultar, agregar, modificar y eliminar informacion de una base de datos hecha en MongoDB.

Como ejemplo, sugerimos este caso de uso, pero te invitamos a que pienses otro ejemplo que te motive y adaptes las consignas.

*Una cadena de hoteles argentinos necesita una API para conectar su front-end. La aplicacion lista hoteles de manera publica, pudiendo los usuarios finales consultar un listado filtrable de todos los hoteles disponibles y tambien consultar un hotel en particular.*


### Funcionalidades básicas (obligatorias)

Al pedir informacion de todos los hoteles la API debe enviar por cada uno de ellos:

- ID
- Nombre
- Ubicación (ciudad y provincia)
- Categoria de habitaciones *(ejemplo: presidencial, premium, comun)*
- Por cada categoria, precio por noche.
- Cantidad de habitaciones en total.
- Cantidad de habitaciones ocupadas en total.
- Porcentaje de ocupacion en total.
- Puntaje (del 0 al 5)

La API debe permitir filtrar los resultados del listado por:
- Ciudad
- Provincia
- Nombre
- Precio por noche de habitacion disponible *(ejemplo: el usuario pide solo hoteles con habitaciones cuyo precio por noche sea menor a $1000)*
- Puntaje *(ejemplo: el usuario pide solo hoteles con un puntaje mayor a 3)*

La API debe permitir ordenar los resultados por:
- Nombre (de la A a la Z o viceversa)
- Puntaje (de mayor a menor o viceversa)
- Precio de las habitaciones (de mayor a menor o viceversa, en cualquier categoría)
- Porcentaje de ocupación (de mayor a menor o viceversa)

Al consultar por un hotel en particular, a la informacion anterior se debe agregar:

- Por cada categoria, cantidad de habitaciones en total
- Por cada categoria, cantidad de habitaciones ocupadas
- Por cada categoria, cantidad de habitaciones disponibles
- Por cada categoria, porcentaje de ocupacion.
- Criticas de los usuarios, que se componen de un puntaje que va de 0 a 5 y un texto breve. (El "puntaje" de cada hotel debe calcularse con el promedio de estas criticas)
