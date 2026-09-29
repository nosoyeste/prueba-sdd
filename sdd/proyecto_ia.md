---
title: "Proyecto basado en SDD (Spec Driven Development): Despliegue de una pila de IA local en Docker sobre ubuntu "
author: "Mnarrieta"
date: "2026-09-29"
category: "Despliegue IA"
tags: [markdown,ia,prompt,local,SDD]
---

# Proyecto basado en SDD (Spec Driven Development): Despliegue de una pila de IA local en Docker sobre ubuntu 
- **Versión:** 1.0
- **Rol del creadaor:** Administrador de sistemas
- **Propçosito:** Definir un manual técnico de requisitos y definiendo una arquitectura para la generación de un manual técnico detallado con la instalación, configuración, tests y mantenimiento en formato markdown (.md)

## 1. Visión general del proyecto (Objetivo)
El objetivo del proyecto es desplegar una insfraestructura de inteligencia artificial local usando contenedores docker en un sistema operativo ubuntu server. Cada servicio residirá en su propio contenedor docker. El sistema dispone de tarjeta gráfica NVIDIA (GPU) 

## 2. Servicios, especificaciones y aplicaciones 
Los serivicios a desplegar son los siguientes 

| Servicio | nombre de contenedor | Puerto interno | Puerto externo | Proposito principal| Dependencias | 
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Ollama** | ollama | 11434 | 11434 | Motor de LLMs locales y servidor de API | GPU NVIDIA y driver (Cuda) |
| **OpenWebUI** | openwebui | 8080 | 3000 | Interfaz web tipo ChatGPT para interactuar con LLMs | Ollama, SearXNG, ComfyUI |
| **Hermes Agent** | hermes-agent | 8000 | 8000 | Arnés parael motor LLMs, Agente autónomo para realizar tareas complejas | Ollama, SearXNG, ComfyUI |
| **Opencode** | opencode | 8080 | 8443 |  |  |
| **ComfyUI** | comfyui | 8188 | 8188 |  |  |
| **YOLO** | yolo | 5000 | 5000 |  |  |
| **SearXNG** | searxng | 8080 | 8080 |  |  |

## 3. Arquitectura de red y datos

### 3.1 Redes Docker
### 3.2 Volúmenes de datos 


## 4. Requisitos de sistema y hardware

## 5. Instrucciones para generar el manual técnico 

## 6. Criterios de aceptación
