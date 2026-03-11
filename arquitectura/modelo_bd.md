# Modelo de Base de Datos – Smart-Nurse IA

El sistema utiliza una base de datos relacional para gestionar la información del personal de enfermería, los turnos asignados y las solicitudes de intercambio.

---

## Entidades principales

## Personal

Almacena la información del personal de enfermería.

Campos:

* id_personal
* nombre
* tipo_personal (auxiliar / enfermero)
* documento
* area
* horas_mensuales

---

## Turnos

Almacena la asignación de turnos del personal.

Campos:

* id_turno
* id_personal
* fecha
* codigo_turno
* horas_turno

---

## Intercambios

Registra las solicitudes de intercambio de turno entre profesionales.

Campos:

* id_intercambio
* id_personal_solicita
* id_personal_destino
* fecha_turno
* estado_intercambio

Estados posibles:

* pendiente
* aprobado
* rechazado

---

## Aprobaciones

Registra la aprobación del jefe de enfermería.

Campos:

* id_aprobacion
* id_intercambio
* id_jefe_enfermeria
* fecha_aprobacion
* estado

---

## Relaciones

Personal 1 → N Turnos

Un profesional puede tener múltiples turnos asignados.

Personal 1 → N Intercambios

Un profesional puede solicitar múltiples intercambios.

Intercambios 1 → 1 Aprobaciones

Cada intercambio debe ser aprobado o rechazado por el jefe de enfermería.
