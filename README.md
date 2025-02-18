# ae-suplementaria-bim2-aa2025

## Sistema de Reservas para un Centro Deportivo

Un centro deportivo ofrece diversas actividades como Natación, Gimnasio, Tenis y Yoga. Actualmente, la gestión de las reservas se realiza de manera manual, lo que genera problemas en el tema de cupos y la dificultad para visualizar las reservas realizadas.

Para solucionar estos inconvenientes, se requiere desarrollar un programa en Python que permita hacer lo siguiente:

* Registrar a los clientes que desean realizar una reserva.
* Mostrar la lista de actividades y su disponibilidad de cupos.
* Validar la disponibilidad de cupos antes de confirmar la reserva.
* Almacenar las reservas realizadas y permitir su consulta.

### Requerimientos

* El usuario ingresará su nombre y apellido.
* Se mostrará un listado de actividades con la cantidad de cupos disponibles.
* El usuario deberá seleccionar una actividad para reservar.
* Si hay cupos disponibles, la reserva será confirmada y el cupo del actividad se actualizará.
* Si no hay cupos disponibles, se debe indicar al usuario
* Se debe permitir visualizar la lista de reservas registradas
* Usar de forma obligatoria las estructuras dadas en los siguientes apartados. Debe comentar con sus palabras la razón de uso y funcionamiento de la función obtener_nombre
* Debe crearse un menú:
  * Reservar una actividad.
  * Ver reservas.
  * Salir del sistema.
  

Considerar:
* Usar funciones en la solución
* En el archivo donde se desarrollará la solución debe usar las siguientes estructucturas
```
# Lista de actividades disponibles
actividades = ["Natación", "Gimnasio", "Tenis", "Yoga"]

# Cupos disponibles por actividad
cupos_disponibles = [13, 15, 14, 12]  # Cupos iniciales para cada actividad

# Relación entre actividades y cupos_disponibles: Natación tiene 13 cupos, Gimnasio tiene 15 cupos, etc.

# Lista para almacenar las reservas realizadas
mis_reservas = []

# Usar la siguiente función de forma obligatoria

# Función
def obtener_nombre():
    nombre = input("Ingrese nombre: ").strip()
    if nombre:  
        return nombre
    print("El valor para nombre no puede estar vacío.")
    return obtener_nombre()  

```
