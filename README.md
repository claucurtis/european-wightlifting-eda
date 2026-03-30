# 🏋️ Análisis de los Campeonatos Europeos de Halterofilia (2019–2024)

> **Proyecto Final — Módulo 4: Análisis Exploratorio de Datos**
> Máster en Data Analysis — Nuclio Digital School
> Autora: Claudia Balseiros

---

## 📌 Contexto del proyecto

**Lift & Lead** es una startup interesada en abrir centros de entrenamiento especializados en halterofilia. Con el auge del CrossFit —que integra técnicas de este deporte—, sus fundadores creen que puede ser un buen momento para invertir en centros dedicados exclusivamente a la halterofilia en Europa.

La dirección de Lift & Lead quiere **validar la hipótesis de que la popularidad del CrossFit está impulsando el interés por la halterofilia en Europa**, y para ello encarga un análisis de los resultados de los campeonatos europeos.

---

## 🎯 Objetivos del análisis

- Explorar y limpiar los datos de los Campeonatos Europeos de Halterofilia de 2019 y 2020 (proporcionados como CSV).
- Ampliar el dataset mediante **web scraping** de Wikipedia para los años 2021–2024.
- Construir un dataset unificado y limpio listo para análisis.
- Extraer insights sobre países dominantes, categorías de peso, tendencias por género y evolución del rendimiento atlético.

---

## 📁 Estructura del repositorio

```
📁 european-weightlifting-analysis/
├── 📓 Nuclio_Modulo4_Proyecto_final_Claudia_Balseiros.ipynb   # Notebook principal
├── 📄 README.md                                               # Este archivo
├── 📄 requirements.txt                                        # Dependencias de Python
├── 📄 .gitignore
└── 📁 data/
    ├── Campeonato Europeo de Halterofilia de 2019 datos original.csv
    └── Campeonato Europeo de Halterofilia de 2020 datos original.csv
```

---

## 🔧 Tecnologías y librerías utilizadas

| Librería | Uso |
|----------|-----|
| `pandas` | Manipulación y transformación de datos |
| `numpy` | Operaciones numéricas |
| `matplotlib` / `seaborn` | Visualización estática |
| `plotly` | Visualización interactiva |
| `requests` / `BeautifulSoup` | Web scraping de Wikipedia |
| `fuzzywuzzy` | Detección de inconsistencias en texto |
| `missingno` | Visualización de valores nulos |
| `re` | Expresiones regulares para limpieza de datos |

---

## 📊 Fases del análisis

### Fase 1 — Datos disponibles (2019 y 2020)

1. Carga de los CSV originales
2. Exploración inicial del dataset
3. Corrección del año del campeonato de 2020 (pospuesto a 2021 por COVID-19)
4. Unificación en un único DataFrame con `pd.concat`
5. Transformación del formato ancho a largo con `melt`
6. Limpieza de datos: corchetes, espacios, inconsistencias
7. Extracción de columnas: `Nombre`, `Apellido`, `País`, `Categoría`, `Arrancada`, `Dos tiempos`, `Total`, `Fecha`
8. Conversión de tipos de datos

### Fase 2 — Web scraping (2021–2024)

- Scraping de las páginas de Wikipedia para cada campeonato
- Estandarización y concatenación con los datos de la Fase 1
- Construcción del dataset final completo (2019–2024)

---

## 🚀 Cómo ejecutar el proyecto

### 1. Clona el repositorio

```bash
git clone https://github.com/tu-usuario/european-weightlifting-analysis.git
cd european-weightlifting-analysis
```

### 2. Instala las dependencias

```bash
pip install -r requirements.txt
```

### 3. Abre el notebook

```bash
jupyter notebook Nuclio_Modulo4_Proyecto_final_Claudia_Balseiros.ipynb
```

> **Nota:** Los archivos de datos deben estar en la carpeta `data/` para que el notebook funcione correctamente.

---

## 📂 Fuentes de datos

- [Campeonato Europeo de Halterofilia de 2019 — Wikipedia](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2019)
- [Campeonato Europeo de Halterofilia de 2020 — Wikipedia](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2020)
- [Campeonato Europeo de Halterofilia de 2021 — Wikipedia](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2021)
- [Campeonato Europeo de Halterofilia de 2022 — Wikipedia](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2022)
- [Campeonato Europeo de Halterofilia de 2023 — Wikipedia](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2023)
- [Campeonato Europeo de Halterofilia de 2024 — Wikipedia](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2024)

---

## 👩‍💻 Autora

**Claudia Balseiros**
Máster en Data Analysis — Nuclio Digital School
[LinkedIn](https://www.linkedin.com/in/tu-perfil) · [GitHub](https://github.com/tu-usuario)
