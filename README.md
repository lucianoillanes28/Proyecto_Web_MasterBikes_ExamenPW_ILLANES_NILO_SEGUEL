# Proyecto_Web_MasterBikes_ExamenPW_ILLANES_NILO_SEGUEL
Proyecto de pagina web en django con funcionalidad de carro de compras

1-. Instalar python Version 3.12.4-amd64 y django version 5.0.7 (INGRESAR EN LA TERMINAL DE VSCODE: py -m pip install Django==5.0.7).

2-. Arrancar el servidor desde esta direccion en la terminal C:\..\..\ProyectoWeb\ProyectoMasterBikes> osea cargar el servidor desde la carpeta ProyectoMasterBikes en el terminal.

3-. (OPCIONAL) Se recomienda abrir el proyecto desde una ventana de incognito ya que el cache a veces genera problemas al agregar y guardar productos.

4-. (OPCIONAL) En la App de servicios en la pestaña de models hay clases para que la bd cargue imagenes, en caso de que si quisieran agregar mas productos desde el admin de django
    se debe instalar en la terminal (pip install Pillow) en caso de no tener esa extension ya que esa es la que permite el manejo y visualizacion de fotos en el admin.

5-. Para entrar al admin de django este es el user y la pass : Usuario: admin // Contraseña: Plissken225@  y este el enlace http://127.0.0.1:8000/admin/

6-. Para entrar a la pagina pinchar este link una vez iniciado el servidor: http://127.0.0.1:8000/

7-. (ESTO ES SOLO PARA LA PESTAÑA DE CONTACTO) Existe una pestaña de contacto a la cual se le hizo un enlace de conexion a gmail en el settings del proyecto, 
    le inclui un correo con contraseña pero lamentablemente no se pudo hacer la conexion con el correo de gmail debido a que google ha deshabilitado la opcion 
    para permitir aplicaciones menos seguras asi que el metodo guarda el correo con su destinatario del admin pero no llega a la bandeja debido a ese problema,
    asi que esa funcion no estara completada hasta poder solucionar ese bug, EL OBJETIVO DE ESTA PESTAÑA ERA LA DE QUE EL USUARIO MANDE INFORMACION AL ADMIN.

8-. La pestaña de servicios es la que tiene la funcionalidad carro de compra, desde el admin del proyecto se agregaron 6 productos en este caso son distintos tipos de bicicicletas
    y cada una tiene un precio diferente, una descripcion y una imagen, la app de carro de compra esta configurada de la siguente manera, muestra todos los productos disponibles,
    en el cual tienen un boton que dice agregar al carro , a lo cual se agrega en el recuadro de mano derecha en el que se muesta la bicicleta seleccionada, la cantidad seleccionada,
    y el precio total del mismo producto seleccionado y al fin una sumatoria de todos los productos por la cantidad seleccionada de cada uno (PESTAÑA 100% FUNCIONAL).

9-. El proyecto consta de 7 app 
        -carro: es la que tiene las clases y definiciones para que el carro de compras agregue, elimine, reste y limpie el carro.
        -contacto: es la que tiene la clase para que el usuario pueda mandar un mensaje al admin.
        -media: es la que se encarga de recibir y guardar las imagenes ingresadas desde el admin.
        -ProyectoMasterBikes: es la app principal la cual tiene toda la configuracion necesaria en el settings, y los enlaces url del resto de apps.
        -ProyectoWebApp: es la clase padres que da la herencia a las demas app para la base de la pagina en html, head y footer, ademas del manejo de css y el home principal.
        -servicios: es la app que tiene la clase de servicios y la pestaña de servicios la cual muestra los servicios disponibles almacenados en la bd.
        -tienda: es la app que contiene el cuerpo de los productos y recibe las herencias de ProyectoWebApp para el manejo de la galeria de productos.


