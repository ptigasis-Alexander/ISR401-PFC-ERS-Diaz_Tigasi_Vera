# ISR401-PFC-ERS-Diaz_Tigasi_Vera

Repositorio público de la Especificación de Requisitos de Software (ERS) del proyecto **SICM — Sistema de Gestión Inteligente para un Centro Médico**, desarrollado para la **Práctica Experimental Unidad IV (PE4): Validación, Gestión de Requisitos y Herramientas CASE**, de la asignatura Ingeniería de Requerimientos (ISR-401) de la Universidad Técnica Estatal de Quevedo.

## Sistema del PFC

**SICM — Sistema de Gestión Inteligente para un Centro Médico**, también identificado como MediCita, es un sistema orientado a la gestión de citas, historiales clínicos, atención médica, enfermería, inventario, recaudación y demás procesos de un centro médico.

El sistema contempla los siguientes roles:

* Paciente.
* Médico general.
* Odontólogo.
* Psicólogo.
* Nutricionista.
* Terapeuta físico.
* Personal de enfermería.
* Personal de recepción y recaudación.
* Coordinador o administrador.

## Integrantes

| Integrante                     | Participación principal                                   |
| ------------------------------ | --------------------------------------------------------- |
| Díaz Pontón Steven Santiago    | Moderación Fagan, revisión del ERS, métricas e informe    |
| Tigasi Sampedro Paul Alexander | Inspección técnica, trazabilidad y gestión de Jira        |
| Vera Gómez Anthony Alfredo     | Lectura Fagan, revisión de calidad y documentación de RFC |

## Roles de la inspección Fagan

| Integrante                     | Rol asignado            |
| ------------------------------ | ----------------------- |
| Díaz Pontón Steven Santiago    | Moderador e Inspector 1 |
| Vera Gómez Anthony Alfredo     | Lector                  |
| Tigasi Sampedro Paul Alexander | Inspector 2             |

La asignación responde a la conformación del equipo de tres integrantes. Cada participante realizó una preparación individual documentada mediante su lista de verificación firmada.

## Change Control Board

| Integrante                     | Rol en el CCB                         |
| ------------------------------ | ------------------------------------- |
| Vera Gómez Anthony Alfredo     | Presidente del CCB                    |
| Díaz Pontón Steven Santiago    | Analista de requisitos                |
| Tigasi Sampedro Paul Alexander | Representante técnico y desarrollador |

El CCB analizó tres solicitudes formales de cambio:

* `RFC-001`: cambio de alcance.
* `RFC-002`: cambio relacionado con calidad.
* `RFC-003`: cambio de restricción y coherencia normativa.

Las decisiones, responsables, plazos y justificaciones se encuentran documentados en `03_CCB/`.

## Estructura del repositorio

```text
ISR401-PFC-ERS-Diaz_Tigasi_Vera/
├── README.md
├── CHANGELOG.md
│
├── 01_ERS/
│   ├── ERS_v1.0.pdf
│   ├── ERS_v1.0.tex
│   ├── ERS_V1.1.pdf
│   └── ERS_V1.1.tex
│
├── 02_Inspeccion/
│   ├── AnexoA_checklists/
│   │   ├── Checklist_Diaz_Steven.pdf
│   │   ├── Checklist_Tigasi-Paul.pdf
│   │   └── Checklist_Vera_Anthony.pdf
│   ├── AnexoB_registro_defectos.xlsx
│   └── metricas.xlsx
│
├── 03_CCB/
│   ├── RFC-01.pdf
│   ├── RFC-02.pdf
│   ├── RFC-03.pdf
│   ├── Acta_CCB.pdf
│   └── Acta_CCB_Firmado.pdf
│
├── 04_Trazabilidad/
│   ├── matriz_trazabilidad.xlsx
│   ├── backlog_export.csv
│   └── capturas/
│
├── 05_Informe/
│   ├── PE4_U4_DIAZ_TIGASI_VERA.tex
│   ├── PE4_U4_DIAZ_TIGASI_VERA.bib
│   ├── PE4_U4_DIAZ_TIGASI_VERA.pdf
│   └── figuras/
│
└── 06_Evidencias/
    ├── capturas_git/
    ├── fotos_sesion/
    └── Declaracion_IA.pdf
```

## Informe final PE4

El informe final se encuentra disponible en:

```text
05_Informe/PE4_U4_DIAZ_TIGASI_VERA.pdf
```

Su archivo fuente principal es:

```text
05_Informe/PE4_U4_DIAZ_TIGASI_VERA.tex
```

Y la base bibliográfica utilizada es:

```text
05_Informe/PE4_U4_DIAZ_TIGASI_VERA.bib
```

## Requisitos de compilación

Para compilar el informe se requiere:

* MiKTeX, TeX Live u otra distribución compatible con LaTeX.
* Compilador `pdflatex`.
* Procesador bibliográfico `bibtex`.
* Paquetes LaTeX utilizados por el documento:

  * `babel`
  * `lmodern`
  * `microtype`
  * `geometry`
  * `setspace`
  * `graphicx`
  * `hyperref`
  * `fancyhdr`
  * `booktabs`
  * `longtable`
  * `tabularx`
  * `array`
  * `multirow`
  * `xcolor`
  * `enumitem`
  * `amsmath`
  * `pgfplots`
  * `float`
  * `caption`
  * `subcaption`
  * `listings`
  * `csquotes`
  * `url`
  * `natbib`

## Instrucciones de compilación

Clonar el repositorio público:

```bash
git clone https://github.com/ptigasis-Alexander/ISR401-PFC-ERS-Diaz_Tigasi_Vera.git
```

Entrar en la carpeta del informe:

```bash
cd ISR401-PFC-ERS-Diaz_Tigasi_Vera/05_Informe
```

Compilar el documento siguiendo este orden:

```bash
pdflatex PE4_U4_DIAZ_TIGASI_VERA.tex
bibtex PE4_U4_DIAZ_TIGASI_VERA
pdflatex PE4_U4_DIAZ_TIGASI_VERA.tex
pdflatex PE4_U4_DIAZ_TIGASI_VERA.tex
```

El archivo generado será:

```text
PE4_U4_DIAZ_TIGASI_VERA.pdf
```

Las imágenes utilizadas por el informe se almacenan en:

```text
05_Informe/figuras/
```

Por tanto, el archivo principal utiliza la siguiente ruta gráfica:

```latex
\graphicspath{{figuras/}}
```

## Inspección formal Fagan

La inspección formal fue aplicada sobre el ERS real del proyecto. Las evidencias incluyen:

* Listas de verificación individuales.
* Registro consolidado de defectos.
* Clasificación por tipo y severidad.
* Métricas de inspección.
* Correcciones aplicadas.
* Evidencias de la sesión.
* Fotografías de participación del equipo.

Los artefactos correspondientes se encuentran en:

```text
02_Inspeccion/
```

## Gestión del cambio y CCB

Las tres solicitudes de cambio y el acta del Change Control Board se encuentran en:

```text
03_CCB/
```

La versión resultante del ERS es:

```text
v1.1
```

La misma versión debe coincidir en:

* Portada del ERS.
* Historial de revisiones.
* `CHANGELOG.md`.
* Informe PE4.
* Tag de línea base de Git.

## Trazabilidad en Jira

La gestión de requisitos y trazabilidad fue realizada en Jira. El repositorio contiene:

* Exportación del backlog en CSV.
* Matriz de trazabilidad bidireccional.
* Capturas del tablero.
* Capturas de issues.
* Evidencias de campos y relaciones.

Los archivos se encuentran en:

```text
04_Trazabilidad/
```

La matriz establece relaciones entre:

```text
Stakeholder → Requisito → Caso de uso → Módulo o clase → Caso de prueba
```

## Control de versiones y línea base

La línea base aprobada del ERS utiliza el tag:

```text
baseline-v1.1
```

El mensaje correspondiente es:

```text
Baseline aprobada por CCB
```

Para crear el tag anotado mediante Git CLI:

```bash
git tag -a baseline-v1.1 -m "Baseline aprobada por CCB"
git push origin baseline-v1.1
```

También puede crearse mediante un Release de GitHub con los siguientes datos:

```text
Tag: baseline-v1.1
Título: Baseline v1.1
Descripción: Baseline del ERS v1.1 aprobada por el Change Control Board (CCB).
```

Para descargar y comprobar los tags publicados:

```bash
git fetch --tags
git tag -n
```

Para mostrar el historial gráfico:

```bash
git log --oneline --graph --decorate --all
```

Para revisar el contenido de la línea base:

```bash
git show baseline-v1.1
```

Las capturas correspondientes deben almacenarse en:

```text
06_Evidencias/capturas_git/
```

## Historial de cambios

El archivo `CHANGELOG.md` documenta los cambios incorporados en cada versión del ERS.

La versión `1.1` contiene una entrada identificable para cada RFC aprobado:

* RFC-001.
* RFC-002.
* RFC-003.

## Evidencias

Las evidencias del proyecto se encuentran organizadas en:

```text
06_Evidencias/
```

Esta carpeta contiene:

* Capturas del historial Git.
* Capturas del tag de línea base.
* Evidencia del Release de GitHub.
* Fotografías de la inspección Fagan.
* Fotografías de la reunión del CCB.
* Declaración de uso de inteligencia artificial.

## Declaración de uso de inteligencia artificial

El uso de herramientas de inteligencia artificial se encuentra declarado en:

```text
06_Evidencias/Declaracion_IA.pdf
```

La declaración identifica la herramienta utilizada, versión, tareas asistidas, fragmentos afectados y procedimiento de verificación crítica realizado por el equipo.

## Enlace público del repositorio

```text
https://github.com/ptigasis-Alexander/ISR401-PFC-ERS-Diaz_Tigasi_Vera
```

## Licencia y uso académico

Este repositorio contiene documentación académica desarrollada para la asignatura Ingeniería de Requerimientos de la Universidad Técnica Estatal de Quevedo. Su contenido debe utilizarse respetando la autoría del equipo y las normas institucionales de integridad académica.
