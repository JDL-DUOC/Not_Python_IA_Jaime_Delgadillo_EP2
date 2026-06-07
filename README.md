#  Agente Académico – Reglamento Duoc UC

Agente conversacional desarrollado como proyecto académico para responder consultas relacionadas con el **Reglamento Académico de Duoc UC**. El sistema utiliza técnicas de búsqueda semántica e inteligencia artificial para localizar información relevante dentro del reglamento y entregar respuestas contextualizadas en lenguaje natural.

Además, incorpora memoria conversacional, permitiendo recordar preguntas anteriores y mantener la coherencia durante la interacción con el usuario.

---

##  Objetivo del Proyecto

El propósito de este proyecto es aplicar conceptos de:

- Inteligencia Artificial Generativa.
- Procesamiento de lenguaje natural (NLP).
- Búsqueda semántica mediante embeddings.
- Bases vectoriales con FAISS.
- Diseño de agentes conversacionales.
- Memoria conversacional en sistemas de IA.

El agente permite consultar el Reglamento Académico de forma más rápida y amigable que una búsqueda manual dentro del documento PDF.

---

##  Tecnologías Utilizadas

- Python
- LangChain
- LangChain Core
- LangChain OpenAI
- Sentence Transformers
- FAISS
- PDFPlumber
- GitHub Models

---

##  Estructura del Proyecto

```text
Agente_Academico_Duoc/
│
├── README.md
├── Not_Python_IA_Jaime_Delgadillo_2.ipynb
├── RES-VRA-03-2024-NUEVO-REGLAMENTO-ACADEMICO63-1.pdf
```

---

##  Instalación

Instala las dependencias necesarias ejecutando el siguiente comando:

```bash
pip install langchain langchain-core langchain-openai langchain-classic sentence-transformers faiss-cpu pdfplumber
```

---

##  Configuración

Antes de ejecutar el notebook, debes configurar tu token de GitHub.

En la **Celda 2**, reemplaza el siguiente valor:

```python
import os

os.environ["GITHUB_TOKEN"] = "INGRESE SU TOKEN ACA" #por seguridad no puedo subir mi token al repositorio publico.
```

Puedes generar el token en:

**GitHub → Settings → Developer Settings → Personal Access Tokens**

---

##  Reglamento Académico

El proyecto utiliza como fuente de conocimiento el documento:

```text
RES-VRA-03-2024-NUEVO-REGLAMENTO-ACADEMICO63-1.pdf
```

Este archivo debe permanecer en la misma carpeta que el notebook para que pueda ser procesado correctamente.

---

##  Ejecución

Abrir el archivo:

```text
Not_Python_IA_Jaime_Delgadillo_2.ipynb
```

y ejecutar las celdas en orden.

| Celda | Descripción |
|---------|-------------|
| 1 | Instalación de librerías |
| 2 | Configuración y conexión del modelo |
| 3 | Lectura y procesamiento del reglamento |
| 4 | Configuración de herramientas |
| 5 | Creación del agente |
| 6 | Activación de memoria conversacional |
| 7 - 10 | Pruebas automáticas |
| 11 | Visualización del estado de la memoria |
| 12 | Inicio del chat interactivo |

---

##  Uso del Agente

Una vez ejecutada la última celda, el usuario puede realizar consultas directamente sobre el Reglamento Académico.

### Ejemplos de preguntas

```text
¿Cuántas veces puedo reprobar una asignatura?

¿Qué ocurre si abandono una asignatura?

¿Cuál es el porcentaje mínimo de asistencia?

¿Existen causales de eliminación académica?
```

---

##  Comandos Especiales

Durante la conversación se encuentran disponibles los siguientes comandos:

| Comando | Función |
|----------|----------|
| memoria | Muestra el historial almacenado |
| limpiar | Borra la memoria conversacional |
| salir | Finaliza la sesión |

---

##  Funcionamiento General

El sistema realiza las siguientes etapas:

1. Lectura del Reglamento Académico en formato PDF.
2. Extracción y limpieza del texto.
3. División del contenido por artículos.
4. Generación de embeddings semánticos.
5. Creación de una base vectorial mediante FAISS.
6. Recuperación de artículos relevantes.
7. Generación de respuestas mediante IA.
8. Gestión de memoria conversacional para mantener contexto.

---

##  Resultados Esperados

El agente permite:

- Consultar información académica de manera rápida.
- Reducir el tiempo de búsqueda dentro del reglamento.
- Obtener respuestas contextualizadas.
- Mantener continuidad en la conversación gracias a la memoria.

---

##  Autor

**Jaime Delgadillo López**

**ISY0101 – Ingeniería de Soluciones con IA**

**Duoc UC – 2026**
