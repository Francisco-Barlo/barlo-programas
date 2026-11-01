# Barlo · programas de los equipos

Los programas compilados de los equipos Barlo (central, pantalla y los que vengan), **firmados por Barlo**, y la **ficha** que dice cuál es el último de cada uno y con qué va.

La app Barlo lee `ficha.json` cuando el teléfono tiene internet, baja lo nuevo y, a bordo, el dueño decide si actualiza. **Cada equipo revisa la firma antes de grabar**: un programa que no esté firmado por Barlo, o al que le cambiaron un solo byte, no se instala.

- `ficha.json` — los programas publicados (tipo, versión, archivo, suma SHA-256, firma, notas).
- `ficha.json.firma` — la firma de la ficha entera.
- `programas/` — los `.bin`.

Se publica con `herramientas/firma/firmar.py` (en el repositorio del firmware, privado). El código fuente no está acá.
