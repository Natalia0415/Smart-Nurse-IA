# Arquitectura del Sistema – Smart-Nurse IA

El sistema Smart-Nurse IA está diseñado utilizando una arquitectura en capas que permite mantener el sistema organizado, escalable y fácil de mantener.

---

## Capa de Presentación

La capa de presentación corresponde a la interfaz con la que interactúan los usuarios.

Funciones principales:

* registro de personal
* visualización del calendario de turnos
* solicitud de intercambio de turnos
* aprobación de intercambios

Esta capa está orientada a facilitar la interacción del personal de enfermería con el sistema.

---

## Capa de Lógica de Negocio

La capa de lógica de negocio se encarga de procesar las reglas del sistema.

Funciones principales:

* validar registro del personal
* controlar horas laborales mensuales
* verificar conflictos de turnos
* gestionar solicitudes de intercambio
* validar permisos de usuarios
* autorizar aprobaciones por jefe de enfermería

Esta capa garantiza que todas las operaciones cumplan con las reglas definidas por la institución.

---

## Capa de Persistencia de Datos

Esta capa gestiona el almacenamiento de la información en la base de datos.

Funciones principales:

* almacenar información del personal
* registrar turnos asignados
* guardar solicitudes de intercambio
* registrar aprobaciones

El uso de una base de datos relacional permite mantener integridad y consistencia en los datos.

---

## Beneficios de la arquitectura

La arquitectura en capas permite:

* mantener el sistema organizado
* facilitar futuras mejoras
* mejorar la seguridad del sistema
* separar responsabilidades dentro del software
