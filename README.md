# Simulador de Jornada Única · IEB María de los Milagros

Simulador de procesos para el caso de la asignatura Políticas Públicas Educativas. Permite ver el colegio en 3D antes y después de unificar la jornada, comparar los escenarios A, B y C, y cargar la propuesta de un grupo (PDF, DOCX o PPTX) para simularla y evaluarla.

Todo funciona en el navegador. Los archivos que se cargan no se suben a ningún servidor.

## Publicar en GitHub Pages

1. Crea un repositorio público, por ejemplo `simulador-jornada-unica`.
2. Sube `index.html` (y este `README.md`) a la raíz del repositorio.
3. En el repositorio, ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
5. En uno o dos minutos la página queda en `https://TU-USUARIO.github.io/simulador-jornada-unica/`.

## Análisis de propuestas

- **Sin configuración:** el simulador lee el archivo, lo simula y hace un análisis básico por palabras clave.
- **Con Claude:** en la pestaña *Evaluar propuesta*, abre «Analizar con Claude usando una clave de API» y pega una clave de API de Anthropic (se crea en console.anthropic.com). Claude lee la propuesta completa, incluidas las páginas que son solo imagen, y genera el informe detallado.

Sobre la clave:

- Se envía solo a la API de Anthropic, desde el navegador de quien la escribe.
- Queda guardada en ese navegador solo si se marca «Recordar en este navegador».
- Cada análisis se cobra a la cuenta dueña de la clave. No la escribas en computadores compartidos ni la pongas dentro del código del repositorio.

Las propuestas cargadas se guardan solo en el navegador de quien las carga.

## Requisitos técnicos

La página carga Three.js (jsDelivr), pdf.js y JSZip (cdnjs) y las fuentes de Google Fonts, así que necesita conexión a internet.
