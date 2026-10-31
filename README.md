# FORM-MC-01 - Mapa conceptual colaborativo

**Universidad Técnica Estatal de Quevedo (UTEQ)**  
**Facultad de Ciencias de la Computación — Carrera de Software**  
**Asignatura:** Aplicaciones Distribuidas 
**Docente:** Dr. Gleiston Cicerón Guerrero Ulloa, PhD  
**Paralelo:** Séptimo Nivel "A"  

## Integrantes 
LOOR SUAREZ STEFFANNY DEL ROCIO
MUÑOZ VERA MELANIE MICHELLE
RIVAS PILOSO DAYVER YAHIR

---

## Estructura del Repositorio
* `main.tex`: Archivo fuente principal del informe técnico en LaTeX.
* `referencias.bib`: Base de datos bibliográfica en formato BibLaTeX (Estilo IEEE).
* `src/`: Código fuente, scripts y archivos de configuración implementados.
* `data/`: Datos crudos, registros (logs) y mediciones obtenidas en las pruebas.
* `figs/`: Diagramas de arquitectura, gráficas y capturas de evidencia verificable.
* `docs/`: Documentación adicional o el PDF compilado requerido por la guía.

---

## Instrucciones de Compilación del Informe 

Para regenerar el documento PDF a partir del código fuente LaTeX clonando este repositorio, asegúrese de cumplir con los siguientes requisitos:

### 1. Compilador y Dependencias
* **Distribución LaTeX:** TeX Live (2023 o superior) o MiKTeX actualizado.
* **Compilador principal:** `pdflatex`
* **Motor de bibliografía:** `biber` (requerido por `biblatex` con estilo `ieee`).
* **Paquetes principales requeridos:** `babel` (spanish), `inputenc`, `fontenc`, `biblatex`, `csquotes`, `graphicx`, `booktabs`, `hyperref`, `listings`, `amsmath`, `geometry`.

### 2. Archivo Principal
* Archivo de entrada: `main.tex`
* Archivo de referencias: `referencias.bib`

### 3. Orden Exacto de Comandos
Ejecute la siguiente secuencia desde la raíz del repositorio en su terminal:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

*(Alternativamente, si utiliza `latexmk`, puede ejecutar: `latexmk -pdf main.tex`)*
