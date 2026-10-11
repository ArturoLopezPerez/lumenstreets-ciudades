# Lumenstreets · ciudades

Zonas de la maqueta 3D de [Lumenstreets](https://github.com/ArturoLopezPerez/App-de-viajes) para Fráncfort del Meno. La app descarga solo las zonas que necesita cada paseo y las guarda en el móvil.

Este repositorio no contiene código: solo los datos procesados, publicados como archivos de una *release*.

- `zonas.json`: índice (versión, ciudad y tamaño de cada zona).
- `frankfurt-<E>_<N>.bin`: una zona de 1 km × 1 km (cuadrícula UTM 32N; `E` y `N` son los kilómetros de su esquina suroeste) con todo el detalle. Formato propio LMQ2 (comprimido con LZ4): edificios con tejados reales, relieve, calles según su acceso, agua, parques, árboles y rótulos.
- `frankfurt-<E>_<N>-m.bin`: la misma zona en nivel medio (edificios simplificados, suelo a 20 m), para verla a entre 0,45 y 1,8 km.
- `frankfurt-lejos.bin`: la ciudad entera en la capa lejana (suelo a 100 m con el plano de clases a 10 m por píxel y los edificios altos o grandes), para verla siempre.

## Procedencia y licencias

**Edificios y relieve.** Datenquelle: Hessische Verwaltung für Bodenmanagement und Geoinformation (HVBG), 3D-Gebäudemodell LoD2 und Digitales Geländemodell DGM1, Datenlizenz Deutschland – Namensnennung – Version 2.0 ([dl-de/by-2-0](https://www.govdata.de/dl-de/by-2-0)), bearbeitet. Los datos están modificados: simplificados, reproyectados, recortados por zonas y convertidos al formato de la app.

**Calles, parques, agua y nombres.** © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors, Open Database License ([ODbL](https://opendatacommons.org/licenses/odbl/)), a través de las teselas de [OpenFreeMap](https://openfreemap.org/). Los datos están modificados: recortados por zonas y convertidos al formato de la app.

Los archivos derivados de este repositorio se distribuyen con esas mismas condiciones: hay que mantener estas atribuciones.
