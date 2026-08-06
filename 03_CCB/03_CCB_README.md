# 03_CCB — Gestión del Cambio y Change Control Board

Esta carpeta contiene el **Paso 2** de la Práctica Experimental Unidad IV (PE4) — Ingeniería de Requisitos (ISR-401), UTEQ — correspondiente al Sistema de Gestión para un Centro Médico.

## Contenido

| Archivo | Descripción |
|---|---|
| `RFC-01.pdf` | Solicitud de cambio de **alcance** (nuevo requisito): incorporación de un asistente virtual con IA para preguntas frecuentes y agendamiento de citas, retomando RC-24 (originalmente clasificado "Won't" en el MoSCoW del PE2). |
| `RFC-02.pdf` | Solicitud de cambio de **calidad** (modificación de NFR): actualización de RNF-02 (disponibilidad) de 99% en horario laboral a 99% las 24 horas, los 7 días de la semana. |
| `RFC-03.pdf` | Solicitud de cambio de **restricción/normativa**: corrección de la colisión de identificadores detectada en la inspección del PE2 entre "RNF-06" (citado en el Acta de Negociación N.°1) y RNF-08 (control de acceso al historial clínico), con implicación directa en el cumplimiento de la LOPDP. |
| `Acta_CCB.pdf` | Acta de la reunión simulada del Change Control Board: asistentes, agenda, deliberación y votación por cada RFC (roles: Presidente, Representante del cliente, Analista, Desarrollador), decisión motivada, acciones, responsables, plazos y línea base resultante (ERS v1.0 → v1.1). |

## Resultado de las decisiones

| RFC | Tipo | Decisión |
|---|---|---|
| RFC-01 | Alcance | Aprobado con condiciones (diferido a Fase 2, tras el cierre del MVP) |
| RFC-02 | Calidad | Aprobado con condiciones (sujeto a validación de presupuesto de infraestructura) |
| RFC-03 | Restricción/normativa | Aprobado (corrección documental inmediata) |

## Trazabilidad

Los cambios aprobados en esta carpeta se reflejan en:
- `01_ERS/ERS_v1.1.pdf` (versión actualizada del ERS)
- `CHANGELOG.md` (raíz del repositorio), entrada `[1.1.0] - 2026-07-22`
- Tag de Git `v1.1.0` (ver `06_Evidencias/` para el historial de commits y tags)

## Equipo

Diaz Pontón Steven Santiago · Tigasi Sampedro Paúl Alexander · Vera Gómez Anthony Alfredo
UTEQ — Ingeniería de Requisitos (ISR-401) — 4to Software "A"
