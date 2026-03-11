# Casos de Prueba – Smart-Nurse IA

## Casos de prueba funcionales

### CP-01 Registro de personal

Descripción
Verificar que el sistema permita registrar un auxiliar o enfermero correctamente.

Datos de prueba

Nombre: Laura Gómez
Tipo: Auxiliar
Documento: 1023456789

Resultado esperado

El sistema registra correctamente al profesional.

---

### CP-02 Registro de turnos

Descripción
Verificar que el sistema permita registrar turnos mediante códigos.

Datos de prueba

Profesional: Laura Gómez
Turno: D
Fecha: 10 marzo

Resultado esperado

El sistema registra correctamente el turno.

---

### CP-03 Control de horas laborales

Descripción
Verificar que el sistema calcule las horas trabajadas durante el mes.

Resultado esperado

El sistema muestra correctamente el total de horas acumuladas.

---

### CP-04 Solicitud de intercambio

Descripción
Verificar que un profesional pueda solicitar intercambio de turno.

Resultado esperado

El sistema registra la solicitud correctamente.

---

### CP-05 Confirmación de intercambio

Descripción
Verificar que ambos profesionales confirmen el intercambio.

Resultado esperado

El sistema registra la confirmación de ambos usuarios.

---

### CP-06 Aprobación de jefe de enfermería

Descripción
Verificar que el jefe de enfermería pueda aprobar el intercambio.

Resultado esperado

El sistema actualiza el calendario de turnos.

---

## Casos de prueba de validación y excepción

### CP-07 Conflicto de turnos

Descripción
Verificar que el sistema no permita asignar dos turnos simultáneos al mismo profesional.

Precondición

Laura Gómez ya tiene turno diurno el 15 de marzo.

Pasos

1. ingresar al módulo de asignación de turnos
2. intentar asignar turno nocturno el mismo día

Resultado esperado

El sistema muestra el mensaje:

"El profesional ya cuenta con turno asignado en esta fecha".

---

### CP-08 Acceso no autorizado

Descripción

Verificar que un auxiliar no pueda aprobar intercambios.

Pasos

1. iniciar sesión como auxiliar
2. intentar acceder al módulo de aprobación

Resultado esperado

El sistema bloquea el acceso y muestra el mensaje:

"Permisos insuficientes para realizar esta acción".

---

### CP-09 Validación de documento

Descripción

Intentar registrar un documento con caracteres no numéricos.

Datos de prueba

Documento: 10234ABC

Resultado esperado

El sistema no permite guardar el registro y solicita ingresar solo números.

---

### CP-10 Validación de horas máximas

Descripción

Verificar que el sistema no permita superar el límite de horas laborales mensuales.

Resultado esperado

El sistema muestra el mensaje:

"Exceso de horas laborales permitidas".
