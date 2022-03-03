# programacion

#Visual studio code

En ocasiones cuando se utiliza vs code en windows bajo OpenSSH se obtiene un error


openssh windows bad owner or permissions

Para solucionarlo lo que debe hacerse es eliminar la herencia de permisos de la carpeta c:/users/miusuario/.ssh 
para ello 

(1) se elige la carpeta, boton derecho propiedades>seguridad>opciones avanzdas y elegir el boton que dice "Deshabiltar herencia" [aplicar] [acptar]

(2) en el explorador entra a .ssh, es posible que te diga que no tienes permisos, pero si eres administrador entoces dile que te de permisos

(3) una vez que puedas entrar a la carpeta prueba que funcione, abriendo una ventana de cmd (no como administrador) y trata de conectarete a tu servidor

ssh prueba@mi.servidor.com -A

si habre entonces ya esta resuelto el problema :)

