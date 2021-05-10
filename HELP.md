# HELP

## Crear el ambiente
conda create -n pycon_ar

# Instalar librerías
Desde requirements:
source activate pycon_ar
conda install --file requirements.txt

Uno a uno:
pip install rise
pip install pandas
(rise instala jupyter notebook & all, pandas instala numpy y matplotlib)

## Generar un pdf con las slides
Ejecutar
jupyter nbconvert --to slides pycon_ar.ipynb --post serve

Abrir
http://127.0.0.1:8000/pycon_ar.slides.html

Agregar "?print-pdf" al enlace
http://127.0.0.1:8000/pycon_ar.slides.html?print-pdf

Guardar/Imprimir como PDF

## Borrar el ambiente
conda deactivate
conda env remove -n pycon_ar

## Mostrar todos los ambientes
conda env list

## Actualizar index.html
Reemplazar REPOSITORY por el nombre del repositorio.
Recordar activar github pages en la rama principal y directorio principal.
