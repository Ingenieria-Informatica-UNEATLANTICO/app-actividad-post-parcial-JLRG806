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

El diagrama de objetos muestra instancias concretas del sistema en un momento dado. Este diagrama refleja los objetos que interactúan durante la operación del sistema de transporte:

- **Ruta1**: Una ruta específica que conecta varias paradas y tiene asignado un vehículo.
- **Bus1**: Un vehículo específico (de tipo Bus) que sigue un horario y es operado por un conductor.
- **Pasajero1**: Un pasajero que paga una tarifa y viaja en un vehículo de la ruta.

#### Diagrama de Estados

Los diagramas de estados modelan los posibles estados en los que pueden encontrarse algunas entidades clave:

- **Pasajero**: Desde el estado de "Esperando" en la parada, pasando por "Abordando", "En Transito" y finalmente "Llegado a Destino".
- **Incidencia**: Los estados de una incidencia, desde "Reportada", pasando por "En Evaluación", "En Proceso de Solución" y finalmente "Resuelta".
- **Vehículo**: El ciclo de vida de un vehículo, desde "En Mantenimiento" a "Disponible", "En Ruta" y "Fuera de Servicio".

## Objetivos del Proyecto

- **Modelado del Sistema**: Crear un modelo de clases que represente correctamente los componentes del sistema de transporte.
- **Simulación de Estados**: Usar diagramas de estados para describir el comportamiento dinámico del sistema.
- **Gestión de Incidencias**: Implementar una solución para gestionar las incidencias durante el servicio de transporte.
- **Simulación de Operaciones**: Modelar los movimientos de los vehículos y la interacción con los pasajeros.

## Estructura del Proyecto



### Menú de Archivos en el Repositorio

- [Modelo del Dominio Parcial](images/modeloDelDominio-Parcial/): Contiene los diagramas de clases, objetos y estados que describen el sistema de transporte público hechos a mano, y luego se pasaron a uml
- [Modelo del Dominio Completo](images/modeloDelDominio-Mejora/): Contiene los diagramas de clases, objetos y estados que describen el sistema de transporte público, estos diagramas se realido una iteracion para mejorar el modelo del dominio.



