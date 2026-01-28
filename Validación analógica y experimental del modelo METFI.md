# METFI — Prototipos Documentados

![status](https://img.shields.io/badge/status-experimental-orange)
![license](https://img.shields.io/badge/license-CC--BY--NC--SA--4.0-blue)
![reproducibility](https://img.shields.io/badge/reproducibility-notebooks-green)
![DOI](https://img.shields.io/badge/DOI-pending-lightgrey)

> **Repositorio**: `METFI_Prototipos_Documentados`  
> **Autoría conceptual**: Javi Ciborro & colaboradores  
> **Propósito**: Validación analógica y experimental del modelo **METFI** (Sistema Tierra como sistema electromagnético toroidal de forzamiento interno)

---

## 📚 Tabla de Contenidos

* [Resumen Ejecutivo](#resumen-ejecutivo)
* [Marco Conceptual](#marco-conceptual)
* [Arquitectura de Prototipos](#arquitectura-de-prototipos)

  * [P3 · Visualizador de Dinámica de Fluidos Ferroeléctricos](#p3--visualizador-de-dinámica-de-fluidos-ferroeléctricos)
* [Diseño Experimental](#diseño-experimental)
* [Variables y Métricas](#variables-y-métricas)
* [Resultados Esperados](#resultados-esperados)
* [Notebooks Reproducibles](#notebooks-reproducibles)
* [Referencias Científicas](#referencias-científicas)
* [Roadmap](#roadmap)

---

## Resumen Ejecutivo

> **Callout — Idea central**
> El prototipo P3 introduce un **modelo analógico físico** que permite observar la **pérdida de simetría toroidal** inducida por forzamiento interno electromagnético, estableciendo un puente directo entre biofísica, dinámica de fluidos y geofísica profunda.

Este documento describe el **Visualizador de Dinámica de Fluidos Ferroeléctricos**, diseñado para emular la interacción núcleo–manto bajo el paradigma METFI. Mediante una celda de Hele‑Shaw, ferrofluidos y campos magnéticos rotatorios, el sistema permite observar transiciones de fase, rupturas de simetría y patrones no lineales comparables a los eventos ECDO.

---

## Marco Conceptual

La hipótesis METFI postula que el Sistema Tierra funciona como un **oscilador electromagnético toroidal**, donde el forzamiento interno domina sobre los forzamientos externos clásicos.

<details>
<summary><strong>🔎 Conexión teórica</strong></summary>

* El núcleo actúa como fuente de forzamiento electromagnético rotatorio
* El manto se comporta como un medio visco‑no lineal acoplado
* La pérdida de simetría toroidal precede a transiciones abruptas del sistema

</details>

Este prototipo materializa esa abstracción mediante un sistema físico observable y repetible.

---

## Arquitectura de Prototipos

### P3 · Visualizador de Dinámica de Fluidos Ferroeléctricos

<a id="p3"></a>

> **Estado**: 🧪 Prototipo experimental validable

**Objetivo principal**: demostrar cómo el **forzamiento interno** genera estructuras de campo y rupturas de simetría sin necesidad de perturbaciones externas.

---

## Diseño Experimental

### 🔧 El prototipo

* **Celda de Hele‑Shaw** (placas paralelas de vidrio/acrílico)
* **Ferrofluido** con nanopartículas magnetizables
* **Bobinas electromagnéticas** dispuestas en geometría toroidal
* **Controlador de frecuencia y fase** (Arduino / DAC)
* **Sistema de captura** (cámara + análisis óptico)

> **Admonition — Analogía clave**
> Núcleo → campo rotatorio  
> Manto → fluido visco‑no lineal  
> ECDO → transición abrupta de patrón

---

### ⚙️ Protocolo de funcionamiento

1. Inicializar campo magnético simétrico
2. Incrementar frecuencia de forzamiento interno
3. Introducir desfasaje angular controlado
4. Observar bifurcaciones y ruptura de simetría

<details>
<summary><strong>📌 Observables visuales</strong></summary>

* Vórtices toroidales
* Fracturas de patrón
* Migración espontánea de nodos
* Colapso a modos caóticos

</details>

---

## Variables y Métricas

| Categoría | Variable            | Significado METFI                 |
| --------- | ------------------- | --------------------------------- |
| Campo     | Frecuencia (Hz)     | Intensidad de forzamiento interno |
| Fluido    | Viscosidad efectiva | Estado del manto                  |
| Patrón    | Número de vórtices  | Grado de simetría                 |
| Dinámica  | Tiempo a colapso    | Umbral ECDO                       |

---

## Resultados Esperados

* Emergencia espontánea de estructuras toroidales
* Pérdida abrupta de simetría al cruzar umbrales críticos
* Histéresis y memoria del sistema
* Validación visual del desacoplamiento núcleo–manto

> **Insight metaestructural**
> El sistema revela cómo la conciencia —entendida como organización de campo— emerge y colapsa en sistemas complejos.

---

## Notebooks Reproducibles

* 📓 [`pattern_analysis.ipynb`](notebooks/pattern_analysis.ipynb) — análisis espectral
* 📓 [`symmetry_breaking.ipynb`](notebooks/symmetry_breaking.ipynb) — métricas de ruptura
* 📓 [`phase_space.ipynb`](notebooks/phase_space.ipynb) — diagramas de bifurcación

![badge](https://img.shields.io/badge/notebook-reproducible-success)

---

## Referencias Científicas

<details>
<summary><strong>📖 Click para desplegar referencias</strong></summary>

* Rosensweig, R. (1985). *Ferrohydrodynamics*. Cambridge Univ. Press. **DOI:** 10.1017/CBO9780511621062
* Cowling, T. G. (1957). Magnetohydrodynamics. *Interscience*. **DOI:** 10.1063/1.3060316
* Strogatz, S. (2018). *Nonlinear Dynamics*. **DOI:** 10.1201/9780429492563

</details>

---

## Roadmap

* [x] Diseño conceptual
* [x] Protocolo experimental
* [ ] Validación de laboratorio
* [ ] Publicación preprint
* [ ] Integración con P1/P2 (biofísica)

---
