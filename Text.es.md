# Formato de texto

El texto enviado por el servidor tiene que seguir el siguiente formato:
+ Las **Marcas de tiempo** son rodeadas por **parentesis**
+ Los **Espacios de nombre** son rodeados por **corchetes**
+ Los **Booleanos** & **Remitentes** son **opcionales**
    + Los **Booleanos** son representados por **+/-**
    + Los **Remitentes** deben ser seguidos por un **doble punto**
+ El **Contenido** debe ser formateado de una manera **recursiva**.

## Ejemplo en un registro de Chat
```
(2:53)[*] oko se ha unido
(2:53)[105.3][HC] oko: prueba!
(2:56)[*] Tiddy se ha unido
(2:56)[msg] oko: foo
(2:57)[msg] to oko: bar
(2:57)[*] Tiddy se ha ido
(2:58)[102.9][alarmas][casa] +mintphin
(3:01)[102.9][alarmas][casa] -mintphin
```
