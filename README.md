# Una breve explicación

Como primero debemos instalar dependencias del frontend y del backend para ello instalamos con 
`npm i` en front y serve 

## Base de datos

antes de ejecutar el serve por favor cree una base de datos llamada **storepoint** posterior a esto al ejecutar el serve se crearan automáticamente las tablas.



> En el archivo raiz de serve crear un archivo **.env** con estos datos: 
> dbName=*storepoint*
> dbUser=*nombreDeUsuario*
> dbPassword=*password*

<image
  src="./capts/Captura1.PNG"
  alt="Archivo"
  caption=".env">

 
# Ejecutar aplicación

Para ejecutar del **front** es con el comando `npm run dev` y para el **serve** `npm start` esto nos habilita un servidor local en el puerto 3000 en especifico 

# Insertar datos 

Insertar datos clientes, productos y de ultimo ya se puede ingresar las ventas


#EndPoints

`http://localhost:3000/cliente`

`http://localhost:3000/producto`

`http://localhost:3000/venta`

##Metodo Get para cliente

`http://localhost:3000/cliente`

##Metodo Post para cliente

`http://localhost:3000/cliente`

estructura de JSON para realizar en el metoo POST

`{
    "nombres": "Campo para insertar",
    "apellidos": "Campo para insertar",
    "direccion": "Campo para insertar",
    "telefono": "Campo para insertar",
    "email": "Campo para insertar"
}`

##Metodo Patch para cliente

`http://localhost:3000/cliente/**ClienteId**`

`{
    "nombres": "Nuevo campo actualizar",
    "apellidos": "Nuevo campo actualizar",
    "direccion": "Nuevo campo actualizar",
    "telefono": "Nuevo campo actualizar",
    "email": "Nuevo campo actualizar"
}`

##Metodo Get para produto

`http://localhost:3000/producto`

##Metodo Post para producto

`http://localhost:3000/producto`

`
{
    "nombre": "Campo para insertar",
    "descripcion": "Campo para insertar",
    "precio": "Campo para insertar",
    "stock": ValorNumerico
}
`

##Metodo Patch para producto

`http://localhost:3000/producto/productoId`

`
{
    "nombre": "Estufa samsumg 2000",
    "descripcion": "Estufa ",
    "precio": "1000.00",
    "stock": 25
}
`


##Metodo Get para venta

`http://localhost:3000/venta`

##Metodo Post para venta

estructura de JSON para realizar en el metoo POST

`http://localhost:3000/venta`

`{
    "clienteId": 1,
    "productos": [
        {
            "productoId":1,
            "cantidad": 2
        }
    ]
    
}
`
