# Curso Git desde cero
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos.

### Zonas de Git
1. Directorio de trabajo
2. Área de preparación
3. Directorio Git

### Flujo de trabajo básico de Git
Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam, itaque expedita. Exercitationem omnis, odit ipsum libero possimus modi corporis qui ratione laborum! Quam ducimus magni, harum cum ea nihil impedit Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus id voluptatibus accusantium nam tempore quo laudantium incidunt, omnis quia sunt vero ab, nihil ea veritatis, quibusdam ut mollitia rem commodi!

Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam, itaque expedita. Exercitationem omnis, odit ipsum libero possimus modi corporis qui ratione laborum! Quam ducimus magni, harum cum ea nihil impedit Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus id voluptatibus accusantium nam tempore quo laudantium incidunt, omnis quia sunt vero ab, nihil ea veritatis, quibusdam ut mollitia rem commodi!

### Configurando Git por primera vez
```
call y apply tienen como primer argumento el nuevo contexto de la función, el cual en este caso es null debido a que no es necesario tener un contexto definido para este ejemplo. Para el caso de call el resto de argumentos deben ser los mismos de la función al ser ejecutada, mientras que para el caso de apply solo toma un segundo argumento, un arreglo, el cual contiene todos los argumentos de la función a ejecutar.

apply tiene una ventaja con respecto a call, que es permitir pasar los argumentos de forma dinámica. En el caso de call, cada parámetro debe ser pasado dentro del método, como un parámetro más; en el caso de apply, solo basta agregar un elemento en el segundo parámetro, que es un arreglo.
```

Ésta Línea fue creada en la rama master.

## Configuración SSH en windows
Usando git Bash seguimos los siguientes pasos:

`git remote add name_remote url_ssh`
`git remote add github git@github.com:NormanJaimes/notas-git.git`
1. Creamos una carpeta llamada `llaves-ssh` en el disco `C` para evitar problemas de rutas.
2. Ejecutamos el comando `ssh-keygen -t rsa -C "mi-correo@ejemplo.com"`.
El correo debe ser el mismo con el que nos registramos en Github para evitar posibles problemas.
Cundo nos pida la ruta escribimos `/c/llaves-ssh/github_rsa`.
3. Iniciamos ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"`.
4. Agregamos la llave shh generada a ssh-agent ejecutando el comando `ssh-add /c/llaves-ssh/github_rsa`

5. Usar el comando `cat /c/llaves-ssh/github_rsa.pub`
Con éste comando emos el contenido del archivo, copiamos todo el texto que nos muestra.

6. Ir a las configuraciones de nuestro perfil de Github y agregar una nueva llave SSH con el contenido que hemos copiado de github_rsa.pub

Desde ahora podemos hacer pull y push sin que github nos esté pidiendo nombre de usuario y contraseña.