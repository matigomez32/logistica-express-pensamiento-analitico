# 🚚 Análisis Operativo y Formulación de Problemas - Logística Express

Proyecto desarrollado como trabajo final del curso **"Pensamiento Analítico y Toma de Decisiones Basada en Datos"**. 

El objetivo principal de este trabajo es traducir una necesidad/duda operativa del área de operaciones de una empresa de logística de última milla a un marco de análisis cuantitativo, aplicando estadística descriptiva para identificar cuellos de botella y sesgos en las métricas clave.

---

## 🎯 Caso de Negocio y Pregunta de Origen
El Gerente de Operaciones de **Logística Express** manifestó preocupación por demoras en entregas, planteando la duda inicial:  
> *"¿Cuánto tiempo nos estamos tardando realmente en entregar un paquete típico?"*

### Traducción al idioma de datos:
* **Métricas a calcular:** Volumen total de envíos, peso total movilizado (KG) y tiempo de entrega (minutos).
* **Dimensiones de agrupación:** Conductor y Zona_Ciudad (para identificar concentraciones de demoras).
* **Filtro de análisis:** Periodo del 29/03/2026 al 30/03/2026.

---

## 🛠️ Mapeo de Variables y Datos
* `ID_Envio`: Categórica (identificador único del paquete).
* `Peso_Paquete_KG`: Numérica (peso del envío).
* `Tiempo_Entrega_Minutos`: Numérica (tiempo total del trayecto).

---

## 📊 Tablero de Resultados (Estadística Descriptiva)

| Métrica | Valor Calculado |
| :--- | :--- |
| **Volumen Total de Envíos** | 10 envíos |
| **Peso Total Movilizado** | 43.9 KG |
| **Tiempo Mínimo** | 12 minutos |
| **Tiempo Máximo** | 140 minutos |
| **Tiempo Promedio** | 32.2 minutos |
| **Mediana del Tiempo** | 21.0 minutos |

---

## 💡 Hallazgo Clave e Insight de Negocio

Existe una diferencia sustancial entre la **Media (32.2 min)** y la **Mediana (21.0 min)**[cite: 6]:

* **Detección de Outlier:** La distorsión es ocasionada por un único envío anómalo (**ID #5009** realizado por Carlos Ruiz en la zona Norte, el cual registró un tiempo de **140 minutos**)[cite: 6]. Este dato atípico infla el promedio general de la operación[cite: 6].
* **Conclusión y Recomendación:** La **Mediana (21 min)** representa con mayor precisión el tiempo de un *"envío típico"* en Logística Express, ya que es resistente a valores extremos[cite: 6]. Evaluar la operación únicamente por el promedio llevaría a decisiones erróneas sobre el rendimiento general de la flota[cite: 6].

---

## 🛠️ Herramientas Utilizadas
* Google Sheets (Estadística Descriptiva, Filtros y Tablas)
* Análisis de Tendencia Central (Media vs. Mediana)

---
✉️ **Contacto**: [Tu LinkedIn] | Matías Gómez
