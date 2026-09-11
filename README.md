# Manual Metodológico y Estadístico

Libro en español para investigación en ciencias de la salud, construido con Quarto. Pixi administra Quarto, Python y las dependencias de la galería de gráficos.

## Preparación

Instala Pixi y ejecuta desde la raíz del proyecto:

```sh
pixi install --locked
```

El entorno está definido para Linux y Windows. Conserva `pixi.toml` y `pixi.lock` en el repositorio para reproducir las dependencias.

## Construcción y vista previa

```sh
pixi run --locked build
```

Genera el libro HTML en `_book/`, ejecutando de nuevo las celdas del notebook. Abre `_book/index.html` para consultar el resultado.

```sh
pixi run --locked preview
```

Inicia la vista previa local con actualización al guardar cambios. Detén el servidor con `Ctrl+C`. Después de modificar el código de la galería, ejecuta `build` para verificarlo desde un kernel nuevo.

## Archivos principales

- `_quarto.yml`: configuración, formato y orden de capítulos.
- `index.qmd` y `libro/*.qmd`: contenido del libro.
- `libro/galeria_graficos.ipynb`: ejemplos y gráficos en Python.
- `references.bib`: bibliografía.
- `pixi.toml` y `pixi.lock`: entorno y tareas.

Los entornos locales, la salida HTML, la caché de Quarto y los checkpoints de Jupyter se excluyen mediante `.gitignore`.

## Licencia

El contenido original del libro se distribuye bajo [Creative Commons Atribución-NoComercial-SinDerivadas 4.0 Internacional (CC BY-NC-ND 4.0)](https://creativecommons.org/licenses/by-nc-nd/4.0/deed.es). Se permite compartirlo con atribución, únicamente con fines no comerciales; la licencia no permite distribuir versiones adaptadas. Consulta [LICENSE.md](LICENSE.md) para conocer el alcance, la atribución y las exclusiones de material de terceros y código.
