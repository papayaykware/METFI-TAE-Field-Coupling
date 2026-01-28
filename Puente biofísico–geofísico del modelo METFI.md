# METFI-BioLink — Acoplamiento Bioelectromagnético y Transiciones Sistémicas

![Status](https://img.shields.io/badge/status-prototipo%20conceptual--experimental-orange)
![License](https://img.shields.io/badge/license-CC--BY--NC--SA%204.0-green)
![Python](https://img.shields.io/badge/python-3.10%2B-yellow)
![Reproducible](https://img.shields.io/badge/reproducible-pipelines-success)
![BioEM](https://img.shields.io/badge/focus-bioelectromagnetismo-blueviolet)

> **Repositorio:** `METFI_Prototipos_Documentados`  
> **Documento:** `METFI-BioLink_whitepaper.md`  
> **Rol:** Prototipo — puente biofísico–geofísico del modelo METFI

---

## 📌 Abstract

**METFI-BioLink** formaliza el acoplamiento entre el **campo electromagnético toroidal interno del Sistema Tierra** y los **sistemas biológicos sensibles a coherencia electromagnética** (cerebro, corazón, sistema neuroentérico, microbiota). El prototipo propone que la **pérdida de simetría toroidal** induce firmas bioelectromagnéticas detectables, funcionando los sistemas vivos como **sensores distribuidos de transición sistémica**. El objetivo es cerrar la brecha entre geofísica no lineal y biofísica de la coherencia, aportando métricas observables y rutas de validación experimental.

---

## 🧭 Table of Contents

* [1. Hipótesis BioLink](#1-hipótesis-biolink)
* [2. Marco Biofísico](#2-marco-biofísico)
* [3. Arquitectura del Prototipo](#3-arquitectura-del-prototipo)
* [4. Variables y Señales](#4-variables-y-señales)
* [5. Métrica de Coherencia Toroidal (MCT)](#5-métrica-de-coherencia-toroidal-mct)
* [6. Integración con METFI-Sim](#6-integración-con-metfi-sim)
* [7. Pipeline Computacional](#7-pipeline-computacional)
* [8. Notebooks y Reproducibilidad](#8-notebooks-y-reproducibilidad)
* [9. Casos de Uso](#9-casos-de-uso)
* [10. Limitaciones y Falsabilidad](#10-limitaciones-y-falsabilidad)
* [11. Roadmap Experimental](#11-roadmap-experimental)
* [12. Referencias Comentadas](#12-referencias-comentadas)

---

## 1. Hipótesis BioLink

La biosfera no se modela como pasajera del sistema Tierra, sino como **capa resonante activa**, capaz de reflejar transiciones internas del campo global.

---

## 2. Marco Biofísico

<details>
<summary><strong>Sistemas considerados</strong></summary>

* Eje cerebro–corazón (EEG–HRV)
* Sistema nervioso entérico
* Microbiota como red oscilatoria
* Comunicación intercelular (exosomas)

</details>

Estos sistemas comparten propiedades de **coherencia, no linealidad y sensibilidad a campos débiles**.

---

## 3. Arquitectura del Prototipo

```text
METFI-BioLink/
├── sensors/
│   ├── eeg_proxy.py
│   ├── hrv_proxy.py
│   └── schumann_link.py
├── metrics/
│   ├── coherence_index.py
│   └── mct.py
├── pipelines/
│   ├── biolink_pipeline.py
│   └── anomaly_fusion.py
├── notebooks/
│   ├── 01_bio_coherence.ipynb
│   ├── 02_geo_bio_sync.ipynb
│   └── 03_transition_signatures.ipynb
└── data/
```

---

## 4. Variables y Señales

* EEG (bandas delta–gamma)
* HRV (RMSSD, LF/HF)
* Ritmos Schumann
* Índices de entropía fisiológica

---

## 5. Métrica de Coherencia Toroidal (MCT)

La **MCT** cuantifica el grado de alineación entre señales biológicas y el estado toroidal simulado:

[
\text{MCT}(t) = \langle C_{bio}(t), C_{toroide}(t) \rangle - \lambda \cdot \nabla S
]

Donde $S$ es la entropía fisiológica agregada.

---

## 6. Integración con METFI-Sim

Los eventos de ruptura simulados se proyectan sobre el espacio biofísico para buscar correlatos.

---

## 7. Pipeline Computacional

```python
signals = load_bio_signals()
toroidal_state = load_metfi_sim()

mct = compute_mct(signals, toroidal_state)
if mct < threshold:
    flag_transition()
```

---

## 8. Notebooks y Reproducibilidad

📓 **Notebooks:**

* `01_bio_coherence.ipynb`
* `02_geo_bio_sync.ipynb`
* `03_transition_signatures.ipynb`

---

## 9. Casos de Uso

* Detección temprana de transiciones sistémicas
* Estudios de sensibilidad biosférica
* Validación cruzada METFI–TAE

---

## 10. Limitaciones y Falsabilidad

La ausencia de correlación sostenida refutaría la hipótesis BioLink.

---

## 11. Roadmap Experimental

* [ ] Integración con datasets EEG/HRV abiertos
* [ ] Estudios longitudinales
* [ ] Validación cruzada con eventos geofísicos

---

## 12. Referencias Comentadas

<details>
<summary><strong>Literatura clave (con DOI)</strong></summary>

* Pikovsky et al. *Synchronization*. **DOI:** 10.1017/CBO9780511755743  
  *Marco de sincronización no lineal.*

* McCraty et al. *Heart–brain interactions*. **DOI:** 10.3389/fpsyg.2014.01090  
  *Coherencia cardíaca y campos.*

</details>

---

### ✅ Conclusión

**METFI-BioLink** convierte la biosfera en un **instrumento distribuido**, capaz de reflejar la dinámica profunda del sistema Tierra bajo el marco METFI y la lógica de aprendizaje por excepción.
