# Diagrama de Clases – Smart Nurse IA

## Clase Usuario

Atributos:

- id_usuario
- nombre
- documento
- rol
- area

Métodos:

- iniciarSesion()
- consultarTurnos()

---

## Clase Enfermero

Atributos:

- horas_mensuales
- tipo (Auxiliar / Enfermero)

Métodos:

- solicitarIntercambio()
- firmarSolicitud()

Hereda de: Usuario

---

## Clase Turno

Atributos:

- id_turno
- fecha
- codigo_turno
- horas
- estado

Métodos:

- asignarTurno()
- validarConflicto()

---

## Clase IntercambioTurno

Atributos:

- id_intercambio
- turno_original
- turno_destino
- enfermero_solicitante
- enfermero_receptor
- estado
- firma_solicitante
- firma_receptor

Métodos:

- registrarSolicitud()
- enviarAprobacion()

---

## Clase JefeEnfermeria

Atributos:

- area_responsable

Métodos:

- aprobarIntercambio()
- rechazarIntercambio()

Hereda de: Usuario

---

## Clase Sistema

Métodos:

- validarHorasMensuales()
- validarConflictoTurnos()
- registrarHistorial()
