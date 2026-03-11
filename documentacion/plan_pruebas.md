# Plan de Pruebas – Smart-Nurse IA

## 1. Introducción

El presente plan de pruebas define la estrategia utilizada para validar el correcto funcionamiento del sistema **Smart-Nurse IA**, el cual permite gestionar los turnos del personal de enfermería dentro de una institución de salud.

El sistema permite registrar auxiliares y enfermeros, controlar horas laborales mensuales, gestionar calendarios de turnos mediante códigos y administrar solicitudes de intercambio de turnos que deben ser confirmadas por los profesionales involucrados y aprobadas por el jefe de enfermería del área.

El objetivo de este documento es garantizar que el sistema cumpla con los requerimientos funcionales, técnicos y de seguridad definidos para el proyecto.

---

## 2. Objetivos de las pruebas

## Objetivo general

Validar el funcionamiento del sistema Smart-Nurse IA mediante la ejecución de pruebas que aseguren la calidad, estabilidad y seguridad del sistema.

## Objetivos específicos

* verificar el registro correcto del personal de enfermería
* validar el control de horas laborales mensuales
* comprobar la correcta asignación de turnos mediante códigos
* validar el proceso de intercambio de turnos entre profesionales
* garantizar que solo el jefe de enfermería pueda aprobar intercambios
* identificar posibles errores o defectos antes de la entrega del sistema

---

## 3. Alcance de las pruebas

Las pruebas se aplicarán a los siguientes módulos del sistema:

* registro del personal de enfermería
* control de horas laborales mensuales
* gestión de calendario de turnos
* solicitud de intercambio de turnos
* aprobación de intercambios por jefe de enfermería

---

## 4. Estrategia de Pruebas

Para garantizar la calidad del sistema se implementa una estrategia de pruebas basada en distintos niveles de validación.

## 4.1 Pruebas Funcionales

Las pruebas funcionales verifican que cada funcionalidad del sistema opere correctamente según los requerimientos definidos.

Se validan procesos como:

* registro de auxiliares y enfermeros
* asignación de turnos mensuales
* registro de horas laborales
* solicitud de intercambio de turnos
* aprobación de intercambios por jefe de enfermería

---

## 4.2 Pruebas de Integración

Estas pruebas verifican la correcta comunicación entre los distintos componentes del sistema.

Ejemplos de validación:

* verificar que al presionar el botón **"Enviar solicitud de intercambio"** el sistema registre correctamente la solicitud en la base de datos
* validar que cuando el jefe de enfermería aprueba un intercambio, el cambio se refleje en el calendario de turnos
* comprobar que los datos registrados en el formulario se almacenen correctamente en el sistema

---

## 4.3 Pruebas de Seguridad

El sistema implementa un modelo de control de acceso basado en roles.

Se validan escenarios como:

* un auxiliar de enfermería no puede aprobar intercambios de turnos
* solo el jefe de enfermería del área puede autorizar cambios
* los usuarios solo pueden modificar sus propias solicitudes

Estas pruebas garantizan que el sistema proteja adecuadamente la información y los permisos de los usuarios.

---

## 4.4 Pruebas de Interfaz de Usuario (UI)

Estas pruebas evalúan la usabilidad y accesibilidad del sistema.

Se verifica que:

* la interfaz sea clara para el personal de enfermería
* los formularios validen correctamente los datos ingresados
* el sistema sea responsivo y funcione correctamente en dispositivos móviles
* los mensajes de error sean claros para el usuario

---

## 5. Entorno de Pruebas

Las pruebas del sistema se ejecutan en un entorno controlado que simula las condiciones reales de uso.

## Hardware

Procesador: 4 CPU
Memoria RAM: 8 GB

## Sistema operativo

Ubuntu 22.04

## Navegadores utilizados

Google Chrome
Mozilla Firefox

## Herramientas de prueba

Las pruebas se ejecutan mediante:

* ejecución manual paso a paso
* validación funcional del sistema
* simulación de flujos de usuario

## Base de datos

El sistema utiliza una base de datos relacional para almacenar:

* información del personal de enfermería
* turnos mensuales
* solicitudes de intercambio
* aprobaciones de jefes de enfermería

---

## 6. Criterios de Aceptación

El sistema Smart-Nurse IA se considerará validado cuando se cumplan los siguientes criterios:

* 100% de las funcionalidades críticas aprobadas (registro de personal, asignación de turnos y aprobación de intercambios)
* 0 defectos de severidad crítica o alta abiertos al momento de la entrega del sistema
* al menos el 95% de los casos de prueba ejecutados con resultado exitoso
* validación correcta de roles y permisos dentro del sistema

---

## 7. Gestión de Defectos

Durante la ejecución de las pruebas pueden identificarse errores o fallos en el sistema.

Para gestionar estos incidentes se utilizará el sistema de seguimiento de incidencias de GitHub.

## Registro de errores

Cada defecto identificado será registrado en **GitHub Issues** incluyendo:

* descripción del problema
* pasos para reproducir el error
* severidad del defecto
* responsable asignado

## Clasificación de severidad

Alta
Errores que impiden el funcionamiento del sistema.

Media
Errores que afectan parcialmente la funcionalidad.

Baja
Errores menores o relacionados con la interfaz.

## Ciclo de vida del defecto

1. identificación del error durante pruebas
2. registro del error en GitHub Issues
3. corrección del error por parte del desarrollador
4. verificación nuevamente por el equipo de pruebas
5. cierre del incidente

Una vez que el defecto ha sido corregido y validado exitosamente por el equipo de pruebas, el incidente será cerrado en el sistema de seguimiento de incidencias. Este cierre indica que el problema ha sido resuelto y no requiere más acciones.
