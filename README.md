# Airbnb Scraper

## Descripción

Este proyecto realiza un web scraping básico de listados de Airbnb para obtener información como títulos, precios y enlaces a las propiedades disponibles en una ubicación específica.

El proyecto incluye un script principal para realizar el scraping, así como herramientas para procesar los datos extraídos y analizarlos en un notebook.

## Estructura del Proyecto

```bash
    airbnb_scraper/
    │
    ├── data/                   # Carpeta para almacenar datos extraídos
    │   ├── raw/                # Datos en bruto (raw)
    │   ├── processed/          # Datos procesados
    │
    ├── logs/                   # Carpeta para guardar logs
    │   └── scrape.log          # Log del scraping
    │
    ├── notebooks/              # Notebooks para exploración y análisis
    │   └── analysis.ipynb
    │
    ├── scripts/                # Scripts de scraping y procesamiento
    │   ├── scrape_airbnb.py    # Script principal de scraping
    │   └── process_data.py     # Script para procesamiento de datos
    │
    ├── requirements.txt        # Librerías requeridas
    ├── .gitignore              # Ignorar datos sensibles y binarios
    └── README.md               # Documentación del proyecto
```


---

## Requisitos Previos

1. **Python 3.8 o superior**: Asegúrate de tener Python instalado en tu sistema.
   - [Descargar Python](https://www.python.org/downloads/)

2. **Git**: Para clonar el repositorio.
   - [Descargar Git](https://git-scm.com/)

3. **pip**: Administrador de paquetes de Python (viene incluido con Python).

---

## Instalación

Sigue estos pasos para configurar el proyecto localmente:

1. Clona este repositorio desde GitHub:
   ```bash
   git clone https://github.com/usuario/airbnb_scraper.git
   cd airbnb_scraper
   ```


2. Crea un entorno virtual para instalar las dependencias (opcional pero recomendado):
    ```bash
    python -m venv venv
    source venv/bin/activate    # En Linux/Mac
    venv\Scripts\activate       # En Windows
    ```

3. Instala las dependencias listadas en requirements.txt:
    ```bash
    pip install -r requirements.txt
    ```

## Uso
1. Ejecuta el script principal para realizar el scraping:

```bash
python scripts/scrape_airbnb.py
```

2. Los datos extraídos se guardarán en la carpeta data/raw con un archivo CSV que incluye un timestamp.

3. Los logs se almacenan en logs/scrape.log.