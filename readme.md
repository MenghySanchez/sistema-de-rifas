Sistema de Rifas

Funcionalidades. 
0.- La cantidad de boletos disponibles se podra gestionar desde una vista de admin.
1.- El usuario podra ver los números que aun estan disponibles.
2.- El número de los ganadores se debera configurar en la vista del admin 
3.- Se debe permitir tener varias rifas en el mismo sistema. 
4.- Los usuarios podran ver las direntes rifas que existen y poder registrarse en las mismas , siempre y cuando la cantidad de boletos no este acabada
5.- Los usuarios podran ver en una pagina de participantes por rifa, a todos los participantes y una parte del numero del que posee su boleto 
6.- una vez que se registra un participante, debe llegar un mail o una notificacion de whatsapp al admin indicando que existe un nuevo participante. 
7.- si un participante gana una de las rifas , se le debe notificar al whatsapp o por email 
8.- al registrarse en una de las rifas y despues de haber realizado el pago, el usuario podrá descargar su ticket o boleto d forma difital 
9.- el usuairo podra ver sus boletos en linea solo con colocar su numero de cedula 



Formulario de registro de rifa :
1.- Nombre de la Rifa 
2.- Descripcion de la rifa 
3.- Terminos y condiciones 
4.- Fecha en que se va a realizar la rifa. En caso de que la rifa se haga una vez que todos los boletos sean vendidos, se establecera como fecha dos dias despues de que el ultimo boleto se venda. 
5.- descripcion del premio o premios (se debe poder agreagar una fotografia del mismo)


El registro se hace en cada rifa , por lo que el identificador de la rifa se usara para asociar el usuairo a la rifa que se esta registrando
Formulario de registro de usuario 
1.- número de cedula 
2.- número celular  (whatsapp)
3.- correo electronico 
4.- Nombre completo 


Vistas
1.- Login del Admin 
2.- Reset de contraseña del admin 
3.- Panel de todas las rifas | admin
4.- Panel de crear rifa | admin
5.- Panel de usuarios con las rifas en las que participan | admin
6.- Panel de todas las rifas | usuarios
7.- Panel de busqueda de rifas por número de cedula | cliente 
8.- Panel de boletos adquiridos | cliente
9.- Panel del boton de pago 
10.- Panel de Rifa | cliente 


Base de datos:
Table usuarios
    id del usuario : cedula 
    nombre del usuario: nombre 
    apellido del usuario : apellido
    email: correo del usuario 
    whatsapp: numero del telefono del usuario 
    
TABLE admin
    id admin
    nombre del admin
    apellido del admin ADD
    email 
    numero de telefono

TABLE Rifa 
    id de la rifa
    nombre de la rifa 
    cantidad de boletos disponibles 
    costo del boleto 
    fecha de rifa

table compra boleto
    id de la rifa
    id del cliente
    respuesta de la api
