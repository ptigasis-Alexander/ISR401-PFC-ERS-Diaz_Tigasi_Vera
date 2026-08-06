# ISR401-PFC-ERS-Diaz_Tigasi_Vera

Repositorio del ERS (Especificación de Requisitos de Software) del proyecto **SICM
(Sistema de Gestión Inteligente para un Centro Médico)**, correspondiente a la
**Práctica Experimental Unidad IV (PE4) — Validación, Gestión de Requisitos y
Herramientas CASE**, de la asignatura Ingeniería de Requerimientos (ISR-401),
Universidad Técnica Estatal de Quevedo (UTEQ), Facultad de Ciencias de la
Computación, Carrera de Software.

## Sistema del PFC

**SICM — Sistema de Gestión Inteligente para un Centro Médico** (también referido
como MediCita). Sistema orientado a la gestión de citas, historiales y flujos de
trabajo de distintos roles clínicos (Médico General, Odontóloga, Psicólogo,
Enfermer@, Paciente, Coordinadora, Nutricionista, Terapeuta Físico).

## Integrantes y roles en la inspección Fagan

| Integrante | Rol Fagan |
|---|---|
| Díaz Pontón Steven Santiago | Moderador / Inspector 1 |
| Vera Gómez Anthony Alfredo | Lector |
| Tigasi Sampedro Paul Alexander | Inspector 2 |

## Estructura del repositorio

```
ISR401-PFC-ERS-Diaz_Tigasi_Vera/
├── README.md                          # Este archivo
├── CHANGELOG.md                       # Historial de versiones del ERS
├── 01_ERS/
│   ├── ERS_v1.0.pdf
│   ├── ERS_v1.1.pdf
│   └── (fuentes .tex del ERS)
├── 02_Inspeccion/
│   ├── AnexoA_checklists/             # Checklist individual firmada por cada inspector
│   ├── AnexoB_registro_defectos.xlsx  # Registro consolidado de defectos
│   └── metricas.xlsx                  # Métricas de inspección (densidad, tipo, severidad)
├── 03_CCB/
│   ├── RFC-01.pdf
│   ├── RFC-02.pdf
│   ├── RFC-03.pdf
│   └── Acta_CCB.pdf
├── 04_Trazabilidad/
│   ├── matriz_trazabilidad.xlsx
│   ├── backlog_export.csv             # Anexo D — export desde Jira
│   └── capturas/
├── 05_Informe/
│   ├── PE4_U4_DIAZ_TIGASI_VERA.tex
│   ├── PE4_U4_DIAZ_TIGASI_VERA.bib
│   ├── PE4_U4_DIAZ_TIGASI_VERA.pdf
│   └── figuras/
└── 06_Evidencias/
    ├── capturas_git/                  # git log y git tag
    ├── fotos_sesion/                  # Fotos de la reunión de inspección y del CCB
    └── declaracion_IA.pdf             # Anexo F
```

## Instrucciones de compilación del informe

El informe se genera en LaTeX a partir del archivo fuente ubicado en `05_Informe/`.

**Compilador:** `pdflatex`

**Dependencias:**
- Distribución LaTeX: MiKTeX o TeX Live
- Paquetes: `babel`, `biblatex` (o `natbib`), `graphicx`, `hyperref`,
  `geometry`, `booktabs` *(ajustar a los paquetes realmente usados en el .tex)*
- Gestor de bibliografía: Biber *(o BibTeX, según corresponda)*

**Archivo principal:** `05_Informe/PE4_U4_DIAZ_TIGASI_VERA.tex`

**Orden de comandos:**

```bash
git clone https://github.com/ptigasis-Alexander/ISR401-PFC-ERS-Diaz_Tigasi_Vera.git
cd ISR401-PFC-ERS-Diaz_Tigasi_Vera/05_Informe
pdflatex PE4_U4_DIAZ_TIGASI_VERA.tex
biber PE4_U4_DIAZ_TIGASI_VERA
pdflatex PE4_U4_DIAZ_TIGASI_VERA.tex
pdflatex PE4_U4_DIAZ_TIGASI_VERA.tex
```

El PDF resultante debe ser idéntico al informe completo alojado en este repositorio,
cuya carátula referencia la misma URL que la carátula subida al SGA en la Semana 14.
Esta reproducibilidad es un criterio de piso (G2): si el PDF no se genera correctamente
a partir del LaTeX clonando este repositorio, la calificación de la práctica es CERO.

## Control de versiones y línea base

- **Commits:** mínimo 8 commits distribuidos, con autoría verificable de los tres
  integrantes y mensajes semánticos, por ejemplo:
  `docs(ers): v1.1 - aplicar cambios CCB semana 14`
- **Tag de línea base:** `baseline-v1.1`
  ```bash
  git tag -a baseline-v1.1 -m "Baseline aprobada por CCB"
  git push origin baseline-v1.1
  ```
- **Ver historial:** `git log --oneline --graph --decorate`
- **Ver tags:** `git tag -n`
- Cada entrada del `CHANGELOG.md` corresponde a un RFC aprobado, con la misma
  versión declarada en la carátula del ERS, en el historial de revisiones y en el tag.

## Herramienta CASE de gestión

Trazabilidad y backlog gestionados en **Jira**, con campos personalizados de
Prioridad (MoSCoW) y Fuente del requisito, y enlaces bidireccionales hacia el
stakeholder de origen y hacia el caso de uso, clase/módulo y caso de prueba
correspondientes.
