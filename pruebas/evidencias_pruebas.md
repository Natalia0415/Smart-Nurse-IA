# Evidencias Simuladas de Resultados de Pruebas

## Introducción

El sistema Smart-Nurse IA se encuentra actualmente en fase de diseño y planificación dentro del proceso de Ingeniería de Software. Por esta razón, las evidencias presentadas corresponden a simulaciones basadas en los casos de prueba definidos en el plan de pruebas.

Estas simulaciones permiten demostrar cómo se validaría el comportamiento del sistema una vez implementado, verificando que las funcionalidades principales cumplan con los requisitos definidos.

---

## Resumen de ejecución de pruebas

| ID | Caso de prueba | Descripción | Resultado esperado | Resultado obtenido (simulado) | Estado |
|----|---------------|-------------|-------------------|--------------------------------|-------|

CP-01 | Registro de profesional | Registrar auxiliar o enfermero en el sistema | El sistema guarda la información correctamente | El sistema muestra mensaje "Registro exitoso" | Aprobado |
CP-02 | Asignación de turno | Asignar turno mensual a un profesional | El turno queda registrado en el sistema | El turno aparece en el calendario mensual | Aprobado |
CP-03 | Consulta de turnos | Visualizar turnos asignados | Mostrar calendario de turnos | El sistema muestra correctamente los turnos | Aprobado |
CP-04 | Solicitud de intercambio | Solicitar cambio de turno | Registrar solicitud de intercambio | El sistema registra solicitud y la envía al jefe | Aprobado |
CP-05 | Aprobación de intercambio | Jefe revisa solicitud | Aprobar o rechazar solicitud | El sistema actualiza el estado de la solicitud | Aprobado |
CP-06 | Validación de conflicto | Detectar turnos duplicados | Mostrar error de conflicto | El sistema bloquea la asignación | Aprobado |
CP-07 | Exceso de horas laborales | Asignar turnos superiores al límite mensual | Mostrar alerta de exceso de horas | Sistema genera alerta preventiva | Aprobado |
CP-08 | Acceso no autorizado | Auxiliar intenta aprobar solicitud | Denegar acceso | Sistema muestra mensaje de permisos insuficientes | Aprobado |
CP-09 | Validación de documento | Registrar documento con letras | Sistema debe rechazar registro | Sistema muestra error de formato | Aprobado |

---

## Evidencias detalladas por caso de prueba

## CP-01 Registro de profesional

Escenario: Registro de nuevo auxiliar de enfermería.

Datos ingresados:

Nombre: Laura Gómez  
Documento: 1023456789  
Tipo de profesional: Auxiliar de Enfermería  
Área: Hospitalización  

Resultado simulado del sistema:

"Registro realizado correctamente".

Estado de la prueba: Aprobado.

---

## CP-02 Asignación de turno

Escenario: Asignación de turno mensual.

Datos ingresados:

Profesional: Laura Gómez  
Fecha: 15/03/2026  
Turno: D (Diurno)  

Resultado simulado del sistema:

El sistema guarda el turno y lo muestra en el calendario mensual.

Estado de la prueba: Aprobado.

---

## CP-03 Consulta de turnos

Escenario: El profesional consulta sus turnos asignados.

Resultado simulado del sistema:

El sistema muestra un calendario con los turnos asignados para el mes correspondiente.

Estado de la prueba: Aprobado.

---

## CP-04 Solicitud de intercambio

Escenario: Un auxiliar solicita intercambiar turno con otro profesional.

Datos simulados:

Solicitante: Laura Gómez  
Receptor: Andrés Martínez  
Fecha del turno: 20/03/2026  

Resultado simulado:

El sistema registra la solicitud y la envía al jefe de enfermería para aprobación.

Estado: Aprobado.

---

## CP-05 Aprobación de intercambio

Escenario: El jefe de enfermería revisa la solicitud.

Resultado simulado:

El sistema permite aprobar o rechazar la solicitud y actualiza el estado del turno en el calendario.

Estado de la prueba: Aprobado.

---

## CP-06 Validación de conflicto de turno

Escenario: Intentar asignar dos turnos al mismo profesional en la misma fecha.

Resultado simulado del sistema:

Mensaje mostrado:

"Error: el profesional ya tiene un turno asignado en esta fecha."

Estado: Aprobado.

---

## CP-07 Validación de horas laborales

Escenario: Asignar turnos que superan el límite mensual de horas laborales.

Resultado simulado:

El sistema muestra advertencia:

"Se ha superado el número máximo de horas laborales permitidas para este mes."

Estado: Aprobado.

---

## CP-08 Acceso no autorizado

Escenario: Un auxiliar intenta acceder al módulo de aprobación de solicitudes.

Resultado simulado:

Mensaje del sistema:

"Acceso denegado. No cuenta con permisos para realizar esta acción."

Estado: Aprobado.

---

## CP-09 Validación de documento

Escenario: Intentar registrar documento con caracteres alfanuméricos.

Datos ingresados:

Documento: 1023ABC45

Resultado simulado:

El sistema bloquea el registro y muestra mensaje:

"El documento debe contener únicamente valores numéricos."

Estado: Aprobado.

---

## Conclusión

Los resultados simulados de las pruebas indican que las funcionalidades principales del sistema Smart-Nurse IA cumplen con los requisitos definidos en el análisis del sistema. Las pruebas permiten validar que la lógica propuesta para la gestión de turnos, intercambio de horarios y control de permisos funcionaría correctamente una vez implementado el sistema.
