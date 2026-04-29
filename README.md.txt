🚀 AI Business Manager: IA Privada y RAG
Este proyecto busca implementar una solución de Inteligencia Artificial Privada para entornos corporativos, utilizando Ollama y técnicas de RAG (Retrieval-Augmented Generation). El objetivo es permitir que los empleados consulten documentos internos (Excel, Word, PDF) de forma segura, rápida y sin que los datos salgan de la infraestructura de la empresa.

🛡️ Propuesta de Valor: Soberanía de Datos
A diferencia de ChatGPT o Claude, esta solución corre 100% local. Ningún presupuesto contable, contrato legal o dato de RRHH es enviado a servidores externos.

🛠️ Tecnologías Principales
Motor de IA: Ollama (Llama 3 / Mistral).

Orquestación: Docker & Docker Compose.

Backend: Python 3.12+ (FastAPI).

Framework de RAG: LangChain & LlamaIndex.

Base de Datos Vectorial: ChromaDB.

Análisis de Datos: Pandas & OpenPyXL.

📂 Estructura del Proyecto
Plaintext
rag-gestion/
├── backend/                # Lógica de procesamiento de IA y API
│   ├── main.py             # Punto de entrada de la aplicación
│   ├── requirements.txt    # Dependencias de Python
│   └── venv/               # Entorno virtual (local)
├── data/                   # Carpeta para archivos de oficina (Excel, Docs)
├── docker-compose.yml      # Configuración de contenedores
├── .gitignore              # Archivos excluidos de Git
└── README.md               # Este archivo
⚙️ Configuración del Entorno (Guía para Desarrolladores)
Sigue estos pasos para replicar el entorno de desarrollo en tu máquina:

1. Requisitos Previos
Tener instalado Docker Desktop.

Tener instalado Python 3.12+.

2. Clonar el Repositorio
Bash
git clone https://github.com/TU_USUARIO/TU_REPO.git
cd rag-gestion
3. Levantar Infraestructura (Docker)
Este comando descargará e iniciará Ollama automáticamente:

Bash
docker-compose up -d
4. Configurar el Backend (Python)
Entra en la carpeta de backend, crea el entorno virtual e instala las librerías:

Bash
cd backend
python -m venv venv
# Activar en Windows:
.\venv\Scripts\activate
# Activar en Mac/Linux:
source venv/bin/activate

pip install -r requirements.txt
5. Descargar el Modelo de Lenguaje
Para que el sistema funcione, debemos bajar el modelo llama3 dentro del contenedor de Ollama:

Bash
docker exec -it ollama-container-name ollama run llama3
(Cuando se cree el contenedor, sustituir ollama-container-name por el nombre real que Docker le asigne al contenedor).