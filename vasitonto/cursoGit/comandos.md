# Documentación Script Pruebas-API
En este documento voy a describir cómo funciona el script que he conseguido hacer a duras penas.
## Funcionamiento ideal del programa.
A pesar de que el script está incompleto, mi idea consistía en realizar la autenticación una sola vez, y después de eso, el programa pide URLs para llamar a la API de NSX-T y las muestra, si son correctas, hasta que se "mate" el proceso, o se introduzca un carácter específico (por ejemplo, q). 
## Funciones.
### Función Parse-URL:
- Esta función no recibe parámetros. 
- Devuelve la cadena introducida por terminal. 
- Se espera que esta cadena tenga el formato proporcionado al copiarlo desde la aplicación de VMWare-NSX-T.

### Función intro-credenciales
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MDM3MDU4MCw4MDc5MTM2NzQsLTMzMj
Q1NTM2M119
-->