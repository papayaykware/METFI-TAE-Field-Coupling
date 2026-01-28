# METFI-Sim — Simulador Computacional de Topología No Lineal

![Status](https://img.shields.io/badge/status-prototipo%20activo-blue)
![License](https://img.shields.io/badge/license-CC--BY--NC--SA%204.0-green)
![Python](https://img.shields.io/badge/python-3.10%2B-yellow)
![Julia](https://img.shields.io/badge/julia-1.9%2B-purple)
![Reproducible](https://img.shields.io/badge/reproducible-notebooks-success)

> **Repositorio:** `METFI_Prototipos_Documentados`  
> **Documento:** `whitepaper.md`  
> **Propósito:** cerrar la brecha entre teoría biofísica y geofísica mediante simulación toroidal no lineal

---

## 📌 Abstract

Este whitepaper presenta **METFI-Sim**, un simulador computacional diseñado para modelar el Sistema Tierra como un **nodo de interferencia electromagnética toroidal de forzamiento interno**, incorporando **pérdida de simetría**, **no linealidades** y **aprendizaje por excepción (TAE)**. El objetivo es traducir hipótesis teóricas del marco METFI en **predicciones computables**, identificando regiones críticas donde emergerían efectos no lineales con impacto geofísico y biofísico.

---

## 🧭 Table of Contents

* [1. Motivación y Alcance](#1-motivación-y-alcance)
* [2. Marco Conceptual](#2-marco-conceptual)
* [3. Arquitectura del Simulador](#3-arquitectura-del-simulador)
* [4. Formulación Matemática](#4-formulación-matemática)
* [5. Pérdida de Simetría Toroidal](#5-pérdida-de-simetría-toroidal)
* [6. Integración de TAE](#6-integración-de-tae)
* [7. Implementación Computacional](#7-implementación-computacional)
* [8. Notebooks Reproducibles](#8-notebooks-reproducibles)
* [9. Casos de Uso y Predicciones](#9-casos-de-uso-y-predicciones)
* [10. Limitaciones y Falsabilidad](#10-limitaciones-y-falsabilidad)
* [11. Roadmap](#11-roadmap)
* [12. Referencias Comentadas](#12-referencias-comentadas)

---

## 1. Motivación y Alcance

Los modelos geofísicos clásicos asumen geometrías esencialmente esféricas y dinámicas mayormente lineales. METFI-Sim introduce una **geometría toroidal activa**, donde pequeñas perturbaciones internas pueden amplificarse mediante **acoplamientos no lineales**.

---

## 2. Marco Conceptual

<details>
<summary><strong>Conceptos clave</strong></summary>

* Campo electromagnético toroidal interno
* Nodo de interferencia planetaria
* No linealidad y bifurcaciones
* Conciencia metaestructural como marco interpretativo

</details>

El sistema se concibe como un **oscilador toroidal acoplado**, sensible a rupturas locales de simetría que actúan como semillas de transición.

---

## 3. Arquitectura del Simulador

```text
METFI-Sim/
├── core/
│   ├── torus_field.py
│   ├── symmetry.py
│   └── nonlinear_dynamics.py
├── tae/
│   ├── exception_learning.py
│   └── collapse_predictor.py
├── notebooks/
│   ├── 01_base_torus.ipynb
│   ├── 02_symmetry_break.ipynb
│   └── 03_tae_events.ipynb
└── data/
```

---

## 4. Formulación Matemática

La topología toroidal se describe mediante coordenadas $(\theta, \phi)$ y un potencial electromagnético $A_T$:

[
\nabla \times A_T = B_T + \delta B(\theta, \phi, t)
]

Donde $\delta B$ representa perturbaciones internas no lineales.

---

## 5. Pérdida de Simetría Toroidal

El simulador permite introducir **puntos de ruptura** (defectos topológicos) y observar la redistribución energética.

---

## 6. Integración de TAE

TAE se implementa como un **mecanismo de aprendizaje inverso**, donde los eventos raros (excepciones) ajustan los parámetros globales:

```python
if event.is_exception():
    model.update_weights(event.signature)
```

Este enfoque permite anticipar **eventos de colapso/transición**.

---

## 7. Implementación Computacional

* **Lenguajes:** Python / Julia
* **Métodos:** ecuaciones diferenciales no lineales, autómatas topológicos
* **Visualización:** mapas toroidales interactivos

---

## 8. Notebooks Reproducibles

📓 **Acceso directo:**

* [`01_base_torus.ipynb`](./notebooks/01_base_torus.ipynb)
* [`02_symmetry_break.ipynb`](./notebooks/02_symmetry_break.ipynb)
* [`03_tae_events.ipynb`](./notebooks/03_tae_events.ipynb)

---

## 9. Casos de Uso y Predicciones

* Identificación de zonas biosféricas sensibles
* Simulación de transiciones abruptas
* Correlación con eventos históricos

---

## 10. Limitaciones y Falsabilidad

Las predicciones deben contrastarse con datos independientes.

---

## 11. Roadmap

* [x] Prototipo base
* [ ] Integración con datos geofísicos reales
* [ ] Validación cruzada biofísica

---

## 12. Referencias Comentadas

<details>
<summary><strong>Artículos clave (con DOI)</strong></summary>

* Bullard, E. C. *The stability of a homopolar dynamo*. **DOI:** 10.1098/rspa.1955.0066  
  *Fundamentos de dinamos planetarias.*

* Fröhlich, H. *Long-range coherence and energy storage in biological systems*. **DOI:** 10.1007/BF01808471  
  *Puente biofísico relevante para METFI.*

</details>

---

### ✅ Conclusión

**METFI-Sim** constituye un puente operativo entre teoría y simulación, aportando una herramienta concreta para explorar la **pérdida de simetría toroidal** y su traducción en eventos críticos dentro del marco METFI.
