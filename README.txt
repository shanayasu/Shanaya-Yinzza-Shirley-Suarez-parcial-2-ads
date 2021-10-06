Nombre: Shanaya Yinzza Shirley Suárez, Parcial 2do corte software

1) Explicación general del programa desarrollado, indicando qué necesidad busca
resolver. Incluya algunos detalles técnicos como el lenguaje usado y el ide en que se
desarrolla e instrucciones generales para ejecutar la aplicación en entorno local.

La necesidad que se tiene es el hecho de perder tiempo cuando se llega a un 
concesionario de autos al momento de no ser atendido directamente con la persona 
que le puede brindar una información mas adecuada de 
acuerdo a las capacidades de compra con las que cuente la persona o el cliente.

Cuando ingrese al concesionario tendrá la posibilidad de dar una descripción breve
del vehiculo que busca junto con el presupuesto con el que cuenta, de esta manera
será dirigido automaticamente a la persona mas ideal para atenderlo, adicionalmente
una vez se encuetre con nuestro empleado, tendrá la oportunidad de crear un nuevo
automovil, que dependiendo de la gama tendrá característica especiales que se
adecuan al presupuesto del cliente. 

el lenjuage usado es JAVA, se realizó en Netbeans IDE 8.2

2)Indique el nombre del primer patrón de diseño que usa

El primer patron de diseño que utilicé fue el patrón de diseño creacional Builder 

a) Justifique la selección y aplicación del patrón de diseño, es decir, qué necesidad
concreta tiene la aplicación y por qué escogió ese patrón para resolverla.

La razón para usar este patrón fue que dado que es para un concesionario de autos y
trabajamos con el presupuesto del cliente, podemos gerenar u ofrecer diferentes 
caracteristicas de autos para nuestros clientes y como este patrón permite crear
diferentes "productos" utilizando un mismo proceso de construcción lo seleccioné,
pues todos los autos tendran motor, llantas, pintura y otros atributos pero estos
variarán dependiendo del presupuesto y la gama que manejemos, por ejemplo si serán
accesorios o caracteristicas de alta, media o baja gama.

b) Indique los archivos y líneas de código en que se evidencia el uso del patrón

El patrón se ve reflejado puntualmente en el archivo AutomovilBuilder.java que tiene
la clase obstracta por ejemplo en la linea 21 a 23 creamos el automovil

en el archivo concesionario.java vemos como el la lineas del 16 al 24 tenemos el get y el set
y el la lineas 26 al 31 construimos las características puntuales

después el los archivos AutoAltaGama, AutoBajaGama y AutoMediaGama contamos con el extends 
del automovilBuilder y ya cada archivo con las caracteristicas únicas.

3) Indique el nombre del segundo patrón de diseño que usa

El segundo patrón de diseño que utilicé fue el patrón de diseño de comportamiento
Chain og responsability

a) Justifique la selección y aplicación del patrón de diseño, es decir, qué necesidad
concreta tiene la aplicación y por qué escogió ese patrón para resolverla.

La razón para usar el patrón de chain of responsability es principalmente que 
dependiendo del presupuesto con el que cuente el cliente tendremos un objeto 
que es capaz de resolver la solicitud, de manera que si uno lo puede resolverla,
esta pasará al sucesor, por ejemplo si un asistente de ventas no tiene un 
conocimiento puntual relacionado a un auto de alta gama, esta solicitud pasara 
al representante de ventas, el cual tiene un mayor conocimiento al respecto. 
Así cada manejador revisa la información que le llega, en este caso la 
información relacionada al auto y al presupuesto y el decide si se queda con 
ella o la pasa a su sucesor. 


b) Indique los archivos y líneas de código en que se evidencia el uso del patrón

El patrón se puede ver implementado en el archivo EmpresaShanayaConcesionario.java 
pues en las lineas de la 31 a la 49 se evidencia la cadena de mando que tendrá la 
empresa a la hora de trabajar con una solicitud, mostrando cual es el sucesor de 
cada objeto, para de esta manera seguir con la cadena de mando o responsabilidad. 

Tambien en el archivo de Headler en las lineas 35 a 36 se evidencia cuando se crea 
el objeto que permite ingresar la locicitud para que esta comience a circular con la
cadena de mando 

Después en los archivos AsesorComercial, SistenteVentas, DirectorVentas, 
GerenteVentas y RepresentanteVentas se ve reflejado que extienden del ManejadorOrden
para asi saber quien es su sucesor y ceder la solicitud y en caso de que ellos 
puedan resolverla podrán crear el auto deseado para mostrarle las caracteristicas 
al cliente, esto con ayuda del patrón builder.

Tambien en el archivo ManejadorOrden.java encontraran de la linea 14 a la 18 como 
funcionará la interface que permite asisnar un sucesor y asi tener las solicitudes 
que realice el cliente.


