# 🤖 AI Business Manager | RAG Enterprise Solution

![Status](https://img.shields.io/badge/Status-Development-orange)
![Tech](https://img.shields.io/badge/Tech-Ollama%20%7C%20FastAPI%20%7C%20Docker-blue)

Solución de **Inteligencia Artificial Local** para la gestión eficiente de documentos de oficina. Orientado a sectores contables, legales y administrativos que requieren **privacidad absoluta** de sus datos.

---

## 🎯 Objetivo del Proyecto
Transformar archivos estáticos (Excel, Word, PDF) en una base de conocimientos dinámica donde los empleados puedan:
* 📊 **Generar estadísticas** instantáneas de archivos contables.
* 🔍 **Ubicar información** en segundos dentro de miles de documentos.
* 📉 **Realizar cálculos** complejos mediante lenguaje natural.

---

## 🏗️ Arquitectura del Sistema
El proyecto utiliza una arquitectura de **microservicios** para garantizar escalabilidad y orden:

| Componente | Tecnología | Rol |
| :--- | :--- | :--- |
| **IA Engine** | Ollama (Llama 3) | Procesamiento de lenguaje natural local. |
| **Backend** | FastAPI / Python | Orquestación de lógica y API. |
| **Vector DB** | ChromaDB | Almacenamiento inteligente de documentos. |
| **Infra** | Docker | Aislamiento por áreas (Contabilidad, RRHH). |

---

## 🚀 Guía de Inicio Rápido

### 1️⃣ Clonar y Preparar
```bash
git clone [https://github.com/franIribarren/rag-gestion-v1.git](https://github.com/franIribarren/rag-gestion-v1.git)
cd rag-gestion-v1
