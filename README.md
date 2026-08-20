# Detección de retinopatía diabética en imágenes del fondo del ojo

Trabajo de grado — Universidad Industrial de Santander (plantilla UIS/ICONTEC).

## Requisitos

- **Visual Studio Code**
- Extensión **[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)** (`James-Yu.latex-workshop`)
- Una distribución de **TeX Live** (recomendado, instalación completa para evitar paquetes faltantes):

  ```bash
  sudo apt install texlive-full biber
  ```

  En Windows/Mac se puede usar [TeX Live](https://tug.org/texlive/) o [MiKTeX](https://miktex.org/) (asegurando que incluya `biber`, motor requerido por `biblatex`).

## Clonar y abrir el proyecto

```bash
git clone https://github.com/oskarwest/tesis_rd.git
cd tesis_rd
code .
```

Al abrir la carpeta en VSCode, si es la primera vez, instala la extensión LaTeX Workshop cuando se sugiera (o desde la pestaña de extensiones).

## Compilar

El repo incluye `.vscode/settings.json`, que ya configura LaTeX Workshop para:

- Compilar automáticamente al guardar (`onSave`) 
- Abrir el PDF resultante en una pestaña dentro de VSCode.

De esta forma, basta unicamente con:

1. Abrir `main_file.tex`.
2. Guardar el archivo para disparar la compilación, o compilar manualmente con el botón ▶ de LaTeX Workshop / atajo `Ctrl+Alt+B`.

También se puede compilar desde terminal:

```bash
latexmk -pdf main_file.tex
```

## Estructura del proyecto

```
main_file.tex          # Documento principal (\input de cada sección)
definitions.tex         # Metadatos (autores, título, director) y comandos propios
icontec_style.sty       # Plantilla ICONTEC/UIS
chngcntr.sty            # Dependencia local de icontec_style.sty
secciones/               # Un archivo .tex por capítulo/sección
imágenes/                # Figuras usadas en el documento, organizadas por sección
references.bib          # Bibliografía (biblatex)
```


