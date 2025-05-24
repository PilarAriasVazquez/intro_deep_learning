
# 🧠 Pokédex Similarity App

Este proyecto permite encontrar el Pokémon más parecido a una imagen proporcionada a través de diferentes interfaces:

- ✔️ Línea de comandos (CLI)
- 🌐 API REST con FastAPI
- 🖼️ Interfaz gráfica con Streamlit

---

## 📦 Requisitos

Asegúrate de tener instalado:

- Python 3.8 o superior
- Las dependencias listadas en `requirements.txt`
- Opcional: Docker (para despliegue)

Instalación recomendada:

```bash
pip install -r requirements.txt
```

---

## 🖥️ 1. Ejecutar desde la línea de comandos (CLI)

### 📌 Ruta de trabajo

Ubícate en el directorio:

```
../solutions/scripts
```

### ▶️ Comando

Ejecuta el siguiente comando, pasando como argumento la URL de la imagen:

```bash
python cli_template.py --img-url "https://theriagames.com/wp-content/uploads/2025/04/POKEMON-GO-charmander-1020x1024.png"
```

Esto imprimirá por consola el nombre del Pokémon más parecido.

---

## 🚀 2. Ejecutar la API con FastAPI

### 📌 Ruta de trabajo

Ubícate en el directorio:

```
../solutions/pokedex
```

### ▶️ Comando

Ejecuta la API con:

```bash
uvicorn main:app --reload
```

> Nota: asegúrate de que `main.py` contiene la definición de la app FastAPI como `app`.

### 🔍 Documentación interactiva

Abre en tu navegador:

```
http://localhost:8000/docs
```

Aquí podrás probar el endpoint `POST /predict` enviando la URL de la imagen.

---

## 🖼️ 3. Ejecutar la interfaz gráfica con Streamlit

### 📌 Ruta de trabajo

Ubícate en el directorio:

```
../solutions/pokedex
```

### ▶️ Comando

Ejecuta el frontend con:

```bash
streamlit run streamlit.py
```

Esto abrirá una interfaz web donde podrás introducir la URL de una imagen y visualizar el resultado del Pokémon más parecido.

---

## 📂 Estructura del proyecto (simplificada)

```
solutions/
├── scripts/
│   └── cli_template.py
│   └── similarity_template.py
│
├── pokedex/
│   └── main.py           # API FastAPI
│   └── streamlit.py      # Interfaz gráfica
│   └── requirements.txt
```

---

## ✨ Autores

Proyecto desarrollado como ejercicio práctico de Deep Learning.  
Autores Álvaro, Pablo, Juan Francisco, Pilar
