# Diagrama de Casos de Uso – Smart Nurse IA

## Actores del sistema

1. Auxiliar de Enfermería
2. Enfermero Profesional
3. Jefe de Enfermería
4. Sistema

---

## Casos de Uso

### Gestión de Usuarios

- Registrar enfermero o auxiliar
- Consultar información del profesional

### Gestión de Turnos

- Registrar turnos mensuales
- Visualizar calendario de turnos
- Validar horas mensuales

### Intercambio de Turnos

- Solicitar intercambio de turno
- Firmar solicitud por ambas partes
- Enviar solicitud al jefe de enfermería

### Aprobación

- Revisar solicitud
- Aprobar intercambio
- Rechazar intercambio

## Control del Sistema

- Validar conflictos de horario
- Control de permisos por rol
- Registro de historial

---

## Representación Simplificada

Auxiliar / Enfermero
        │
        ├── Consultar turnos
        ├── Solicitar intercambio
        └── Firmar solicitud

Jefe de Enfermería
        │
        ├── Revisar solicitud
        ├── Aprobar intercambio
        └── Rechazar intercambio

Sistema
        │
        ├── Validar horas mensuales
        ├── Validar conflictos
        └── Guardar registro
