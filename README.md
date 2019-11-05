# lib_siiau: Libreria para Python para extraer información de alumnos y profesores de la UdeG

### Extrae información de alumnos y profesores de la Universidad de Guadalajara

* #### __Dependencias__
    * python 2
    * requests

* #### __Método de uso__
```
# extraer nombre
from libSIIAU import Alumno
codigo = "123456789"
alumno = Alumno(codigo, "uno2ytres")
print "Nombre: %s" % alumno.nombre

# Validar codigo y NIP
from libSIIAU import Alumno
codigo = "123456789"
alumno = Alumno(codigo, "nip_incorrecto")
if alumno.valido:
    print "Codigo y nip correctos"
else:
    print "Codigo o nip incorrectos"
```
