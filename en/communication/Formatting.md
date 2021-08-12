# Text Formatting

Text sent by the server needs to follow this format:
+ **Timestamps** are surrounded by **parenthesis**
+ **Namespaces** should be surrounded by **squarebrackets**
+ **Booleans** & **Sender** are **optional**
    + **Booleans** are represented by **+/-**
    + **Sender** should be followed by a **colon**
+ **Content** can be formatted in a **recursive** manner.

## Example Chat Log
```
(2:53)[*] oko joined  
(2:53)[105.3][HC] oko: test!
(2:56)[*] Tiddy joined
(2:56)[msg] oko: foo
(2:57)[msg] to oko: bar
(2:57)[*] Tiddy left
(2:58)[102.9][snitches][home] +mintphin
(3:01)[102.9][snitches][home] -mintphin
```

