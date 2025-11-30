# ae-suplementaria-bim2-aa2025

## Sistema de Inscripción para Talleres Culturales en una Casa de la Juventud

Una Casa de la Juventud ofrece diversos talleres culturales como “Pintura”, “Danza Moderna”, “Teatro” y “Guitarra”.
Actualmente, la gestión de las inscripciones se realiza de manera manual, lo que provoca errores en el control de cupos y dificulta visualizar las inscripciones realizadas.

Para solucionar estos inconvenientes, se requiere desarrollar un programa en Python que permita:

* Registrar a jóvenes que desean participar en un taller.
* Mostrar la lista de talleres y su disponibilidad de cupos.
* Validar la disponibilidad antes de confirmar la inscripción.
* Guardar todas las inscripciones en una lista y permitir su consulta.

### Requerimientos

* El usuario ingresará nombre y apellido del participante.
* Se mostrará un listado de talleres con la cantidad de cupos disponibles.
* El usuario seleccionará un taller para inscribirse.
* Si hay cupos disponibles, la inscripción será confirmada y el cupo del taller se actualizará.
* Si no hay cupos, se deberá informar al usuario.
* El sistema debe permitir visualizar todas las inscripciones realizadas.
* Se debe usar de forma obligatoria las estructuras definidas en los apartados siguientes.
* Se debe comentar con sus palabras la razón de uso y funcionamiento de la función obtener_nombre.
* El sistema debe incluir un menú con:
    * Inscribirse en un taller
    * Ver inscripciones
    * Salir del sistema

### Considerar:
* Usar funciones en la solución
* En el archivo donde se desarrollará la solución debe usar las siguientes estructucturas, de forma obligatoria.

```

# Lista de talleres disponibles
talleres = ["Pintura", "Danza Moderna", "Teatro", "Guitarra"]

# Cupos disponibles por taller
cupos = [12, 15, 8, 10]   # Cupos iniciales para cada taller

# Relación entre talleres y cupos:
# - Pintura tiene 12 cupos
# - Danza Moderna tiene 15 cupos
# - Teatro tiene 8 cupos
# - Guitarra tiene 10 cupos

# Lista para almacenar inscripciones
inscripciones = []


# Función obligatoria
def obtener_nombre():
    nombre = input("Ingrese nombre: ").strip()
    if nombre:
        return nombre
    else:
        print("El nombre no puede estar vacío.")
        return obtener_nombre()

```

### Flujo de datos esperado
1. El usuario ingresa su nombre (validado por obtener_nombre) y apellido.
2. Se muestran los talleres con sus cupos disponibles.
3. El usuario selecciona un taller.
4. Se valida si existen cupos:
    5. Si hay cupos → Se registra la inscripción y se descuenta un cupo.
    6. Si no hay cupos → Se muestra un mensaje de error.
7. La inscripción se almacena en la lista inscripciones como un diccionario o lista interna.
8. El usuario puede visualizar todas las inscripciones registradas.
9. El programa continúa hasta que el usuario elija salir.
