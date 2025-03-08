Documentación del Programa de Punto De Venta
Descripción General
Este programa permite gestionar clientes, vendedores, productos y facturas, con acceso restringido según el tipo de usuario. Los datos de usuarios, clientes, vendedores y productos se almacenan en archivos de texto para su persistencia.

Inicio de Sesión
El programa inicia con una pantalla de Login, donde el usuario debe ingresar su ID y contraseña. Dependiendo de sus credenciales, se le asignará uno de los siguientes roles:

Administrador: Tiene acceso a todas las funciones.
Usuario Normal: Solo puede acceder a la gestión de facturas.
Las credenciales se encuentran en el archivo usuarios.txt con el siguiente formato:

ID,Nombre,Contraseña,TipoUsuario
1,Felipe,123456,administrador
2,Juan,123456,usuario
Ejecución del Programa
Para abrir el programa, puedes:

Ejecutar el archivo compilado: login.exe
Ejecutar el código fuente: python login.py
Estructura del Proyecto
El programa está dividido en diferentes módulos para una mejor organización:

login.py → Interfaz de inicio de sesión y conexión con otros módulos.
gestion_admin.py → Contiene todas las funciones de administración (clientes, vendedores, productos y facturas).
gestion_usuario.py → Contiene la gestión de facturas (única función accesible para usuarios normales).
Archivos de datos:
usuarios.txt → Almacena las credenciales de acceso.
clientes.txt → Almacena los datos de los clientes.
vendedores.txt → Contiene información de los vendedores.
productos.txt → Registra los productos disponibles.
facturas.txt → Guarda la información de las facturas generadas.
Funciones Disponibles
Para Administradores
show_gestion_clientes() → Gestiona clientes (agregar, eliminar, modificar, buscar).
ventana_usuarios() → Gestiona usuarios del sistema.
show_gestion_vendedores() → Permite administrar vendedores.
show_gestion_productos() → Maneja los productos disponibles.
show_gestion_facturas() → Administra las facturas generadas.
Para Usuarios Normales
show_gestion_facturas() → Permite ver y gestionar facturas.
Nota Importante
Si al ingresar un dato en cualquier función no se refleja en la pantalla, debes presionar 'Buscar' para actualizar la información.

Requisitos del Sistema
Python 3.x
Librerías necesarias: tkinter (interfaz gráfica)
Conclusión
Este programa ofrece una plataforma de gestión eficiente y organizada, con accesos diferenciados según el tipo de usuario. 🚀