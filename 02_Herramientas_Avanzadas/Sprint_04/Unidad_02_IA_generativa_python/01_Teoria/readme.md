![Cabecera](../../assets/cabecera_thebridge.png)

# IA generativa con Python — Teoría

Índice de **esta carpeta de teoría**.

Hay **dos formas** de abrir cada notebook en Colab:

1. **Launcher** (GitHub Pages): `template_workout` — misma convención que el resto del bootcamp.
2. **Colab** (enlace al `.ipynb` en GitHub): `https://colab.research.google.com/github/<org>/<repo>/blob/<rama>/<ruta>.ipynb`

**Parámetros fijos:** `repo=aie-online-tb/material_bootcamp_AI_Engineering`, rama `main`.

Leyenda:

- **[README]** — documento Markdown (`.md`)
- **[Notebook]** — Jupyter (`.ipynb`)

---

## Ficheros en esta carpeta

| Fichero | Tipo |
|---------|------|
| [01_Entornos_virtuales_y_dependencias.md](01_Entornos_virtuales_y_dependencias.md) | Markdown — teoría + tutorial del proyecto ejemplo |
| [02_Introducción_IA_Generativa.md](02_Introducción_IA_Generativa.md) | Markdown |
| [03_IA_Generativa_con_python.md](03_IA_Generativa_con_python.md) | Markdown |
| [04_Ejemplos_Gemini_API_con_Python.ipynb](04_Ejemplos_Gemini_API_con_Python.ipynb) | Notebook — ejemplos ampliados (opcional) |
| [ejemplo_proyecto_entornos_virtuales/](ejemplo_proyecto_entornos_virtuales/) | Proyecto sesión entornos + Gemini ([README](ejemplo_proyecto_entornos_virtuales/README.md)) |
| [readme.md](readme.md) | Markdown |

---

## Proyecto ejemplo: entorno virtual + Gemini

**Carpeta del proyecto (abrid aquí):** [ejemplo_proyecto_entornos_virtuales/](ejemplo_proyecto_entornos_virtuales/)

**Guía paso a paso (vídeo / local):** [ejemplo_proyecto_entornos_virtuales/README.md](ejemplo_proyecto_entornos_virtuales/README.md)

```text
ejemplo_proyecto_entornos_virtuales/
├── README.md
├── .venv/                      ← python -m venv .venv
├── requirements.txt            ← google-genai, python-dotenv
├── .gitignore                  ← incluye .env
├── .env.example                ← plantilla (subir a git)
├── .env                        ← tu API key (no subir a git)
├── gemini_hola_mundo.py
└── gemini_hola_mundo.ipynb
```

**Tutorial completo (teoría):** [01_Entornos_virtuales_y_dependencias.md](01_Entornos_virtuales_y_dependencias.md)

**Resumen rápido:**

```bash
cd ejemplo_proyecto_entornos_virtuales
cp .env.example .env   # editar .env con tu GEMINI_API_KEY
python -m venv .venv
# activar .venv (ver 01_Entornos_virtuales_y_dependencias.md)
python -m pip install -r requirements.txt
python gemini_hola_mundo.py
# o abrir gemini_hola_mundo.ipynb (kernel = .venv de esta carpeta)
```

---

## Notebooks — Colab y launcher

### [gemini_hola_mundo.ipynb](ejemplo_proyecto_entornos_virtuales/gemini_hola_mundo.ipynb) — proyecto de la sesión

- **Colab:** https://colab.research.google.com/github/aie-online-tb/material_bootcamp_AI_Engineering/blob/main/02_Herramientas_Avanzadas/Sprint_04/Unidad_02_IA_generativa_python/01_Teoria/ejemplo_proyecto_entornos_virtuales/gemini_hola_mundo.ipynb
- **Launcher:** https://aie-online-tb.github.io/template_workout/?mode=colab&repo=aie-online-tb/material_bootcamp_AI_Engineering&ref=main&path=02_Herramientas_Avanzadas/Sprint_04/Unidad_02_IA_generativa_python/01_Teoria/ejemplo_proyecto_entornos_virtuales/gemini_hola_mundo.ipynb

En Colab: `pip install google-genai python-dotenv` y configurar `GEMINI_API_KEY` (secretos de Colab o `getpass` en la celda 1 del notebook).

### [04_Ejemplos_Gemini_API_con_Python.ipynb](04_Ejemplos_Gemini_API_con_Python.ipynb) — ejemplos ampliados (opcional)

- **Colab:** https://colab.research.google.com/github/aie-online-tb/material_bootcamp_AI_Engineering/blob/main/02_Herramientas_Avanzadas/Sprint_04/Unidad_02_IA_generativa_python/01_Teoria/04_Ejemplos_Gemini_API_con_Python.ipynb
- **Launcher:** https://aie-online-tb.github.io/template_workout/?mode=colab&repo=aie-online-tb/material_bootcamp_AI_Engineering&ref=main&path=02_Herramientas_Avanzadas/Sprint_04/Unidad_02_IA_generativa_python/01_Teoria/04_Ejemplos_Gemini_API_con_Python.ipynb

JSON estructurado, streaming, chat, etc. Misma API key y convención de kernel si usáis un `.venv` local.

---

## Documentos Markdown

- [01_Entornos_virtuales_y_dependencias.md](01_Entornos_virtuales_y_dependencias.md)
- [02_Introducción_IA_Generativa.md](02_Introducción_IA_Generativa.md)
- [03_IA_Generativa_con_python.md](03_IA_Generativa_con_python.md)
- [readme.md](readme.md)

---

## Nota sobre Colab y GitHub

Si al abrir desde Colab aparece una ventana de autorización de GitHub **en blanco** y aun así se carga el cuaderno, podéis cerrarla. Con repos **privados**, el enlace Colab también exige acceso a GitHub y OAuth aprobado para la organización.
