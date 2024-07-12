# Documentación Script Pruebas-API
En este documento voy a describir cómo funciona el script que he conseguido hacer a duras penas.
## Funcionamiento ideal del programa.
A pesar de que el script está incompleto, mi idea consistía en un programa que pide las credenciales para la autenticación, y pide una entrada por terminal. Dependiendo de esta entrada, hará una cosa u otra, que se detalla más abajo. Si no hay errores de ejecución, se muestra la consulta y se vuelve a pedir una entrada.
## Funciones.
### Función Parse-URL:
- Esta función no recibe parámetros. 
- Devuelve una cadena. 

Esta función pide una cadena al usuario por la terminal, para realizar la consulta a la API de NSX-T. Se esperan 3 cadenas diferentes:
1. Una cadena vacía: Se autocompletará por defecto a la URL que pide todas las reglas de SERVAPP-PRO-
2. Una URL a algún recurso de la aplicación: Esta cadena debe tener la forma proporcionada al copiarla desde la aplicación de NSX-T Data Center. [Cómo copiar el path del recurso](https://drive.google.com/file/d/1o-cikh9H32egGpM3egRWnU4qHBkQoyuA/view?usp=sharing)
3. El carácter "q": Al introducir este carácter, el script se terminará a sí mismo.

### Función Intro-Cred:
- Esta función no recibe parámetros.
- Devuelve las cabeceras de autenticación que se usarán en el la solicitud a la API.

Esta función utiliza el cmdlet Get-Credential para pedir al usuario un par de nombre de usuario y contraseña, los convierte a Base64 y los mete en una tabla Hash que se enviará de cabecera a la solicitud de la API.
### Desarrollo general del programa 
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcyMDkzODI2NCwxOTIzNDU1MDA5LDE4NT
gwNDU3NzgsMTAwNzU1ODEwNiwtMTUwMzcwNTgwLDgwNzkxMzY3
NCwtMzMyNDU1MzYzXX0=
-->