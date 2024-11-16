# Sistema de Transporte Público de una ciudad

## Descripción del Problema

El problema consiste en modelar un sistema de transporte público donde se gestionan vehículos (buses, trenes, metros), rutas, paradas, conductores, pasajeros, tarifas y incidencias. El sistema debe permitir la operación eficiente de rutas, la asignación de vehículos y la gestión de incidencias, tarifas y horarios.

El sistema debe proporcionar una interfaz clara para el seguimiento de los pasajeros, los vehículos y el control de las incidencias, así como la gestión de las tarifas y horarios en tiempo real.

## Solución Propuesta

Para resolver este problema, se ha creado un modelo de dominio utilizando diagramas de clases, objetos y estados que describen los distintos componentes del sistema y sus interacciones. El sistema se ha modelado siguiendo un enfoque orientado a objetos, dividiendo la responsabilidad entre clases que representan elementos claves del sistema de transporte, como vehículos, rutas, paradas, pasajeros y incidencias.

### Modelo del Dominio

A continuación, se describen los diagramas utilizados para modelar el sistema:

#### Diagrama de Clases

El diagrama de clases representa las entidades principales y sus relaciones:

- **CentroControl**: Gestiona rutas, tarifas, horarios e incidencias.
- **Ruta**: Define el trayecto entre paradas y está asociada a un vehículo.
- **Horario**: Define los horarios de salida y llegada de los vehículos en una ruta.
- **Parada**: Punto de recogida y entrega de pasajeros en una ruta.
- **Vehículo (Bus, Tren, Metro)**: Representa los vehículos que operan en las rutas.
- **Pasajero**: Persona que utiliza el servicio de transporte.
- **Conductor**: Persona que opera los vehículos.
- **Incidencia**: Problemas o situaciones inesperadas que ocurren durante el servicio.
- **Tarifa**: Representa el costo de viajar en el transporte.

#### Diagrama de Objetos

El diagrama de objetos muestra instancias concretas del sistema en un momento dado. Este diagrama refleja los objetos que interactúan durante la operación del sistema de transporte.

#### Diagrama de Estados

Los diagramas de estados modelan los posibles estados en los que pueden encontrarse algunas entidades clave:

- **Pasajero**: Cambia de estado desde "Esperando" en la parada hasta "Llegado a Destino" después de completar su viaje.
- **Vehículo**: El ciclo de vida de un vehículo, desde "En Mantenimiento" a "Disponible", "En Ruta" y "Fuera de Servicio".

### Menú de Archivos en el Repositorio


1. **Modelo del dominio (PDF)**:
   - [Modelo del dominio PDF](images/modeloDelDominioPapel/parcial%20%2014%20%20November%202024.pdf): Documento escaneado con los diagramas de clases, objetos y estados creados a mano durante el parcial.

2. **Trabajo Parcial (Hecho a mano y convertido a UML)**:
   - [Modelo del Dominio Parcial SVG](images/modeloDelDominio-Parcial/): Contiene los diagramas en formato SVG de clases, objetos y estados realizados a mano y luego convertidos a UML.
   - [Modelo del Dominio Parcial UML](modelosUML/modeloDelDominio-Parcial/): Contiene los diagramas UML correspondientes a clases, objetos y estados.


3. **Mejoras en el Modelo (Iteración posterior)**:
   - [Modelo del Dominio Mejora SVG](images/modeloDelDominio-Mejora/): Diagramas en formato SVG mejorados después de la iteración.
   - [Modelo del Dominio Mejora UML](modelosUML/modeloDelDominio-Mejora/): Diagramas UML mejorados después de la iteración.


