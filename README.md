# 🚚 Análisis Operativo y Formulación de Problemas - Logística Express

Proyecto desarrollado como **Actividad Core** para el módulo de **"Pensamiento Analítico y Toma de Decisiones Basada en Datos"**.

El objetivo de este proyecto es evaluar la operación de entregas de última milla de **Logística Express**, traduciendo una duda de negocio cualitativa a métricas cuantitativas exactas mediante estadística descriptiva para identificar la causa real de las demoras.

---

## 🎯 Caso de Negocio y Pregunta de Origen
El Gerente de Operaciones manifestó preocupación por posibles demoras en entregas:
> *"¡Hola! Los clientes se están quejando de que tardamos demasiado. Siento que los conductores están atrapados en el tráfico o llevando paquetes muy pesados, pero no tengo claridad... ¿cuánto tiempo nos estamos tardando realmente en entregar un paquete típico?"*

### Traducción al idioma de datos:
* **Métricas:** Volumen total de envíos (conteo), peso total movilizado (suma KG) y tiempos de entrega (Mínimo, Máximo, Promedio y Mediana en minutos).
* **Dimensión:** Análisis global de la operación.
* **Filtro temporal:** Periodo del 29/03/2026 al 30/03/2026.

---

## 🛠️ Mapeo de Variables
* `ID_Envio`: Categórica (Identificador único).
* `Peso_Paquete_KG`: Numérica (Peso del paquete).
* `Tiempo_Entrega_Minutos`: Numérica (Tiempo del recorrido).

---

## 📊 Tablero de Resultados (Estadística Descriptiva)

| Métrica | Valor Calculado | Fórmula Utilizada |
| :--- | :---: | :--- |
| **Volumen Total de Envíos** | **10** | `=CONTAR(A2:A11)` |
| **Peso Total Movilizado** | **43.9 KG** | `=SUMA(F2:F11)` |
| **Tiempo Mínimo** | **12 min** | `=MIN(G2:G11)` |
| **Tiempo Máximo** | **140 min** | `=MAX(G2:G11)` |
| **Tiempo Promedio** | **32.2 min** | `=PROMEDIO(G2:G11)` |
| **Mediana del Tiempo** | **21.0 min** | `=MEDIANA(G2:G11)` |

---

## 💡 Conclusión Estratégica e Insights de Negocio

* **Explicación de la diferencia entre Promedio (32.2 min) y Mediana (21 min):**  
  Existe una distorsión sustancial provocada por un único valor atípico (*outlier*): el **envío #5009** realizado por Carlos Ruiz en la zona Norte, el cual registró **140 minutos**. Este caso aislado infla el promedio general de la flota.

* **Métrica más representativa:**  
  La **Mediana (21 minutos)** representa fielmente lo que tarda un *"envío típico"* en Logística Express, ya que es una métrica robusta e inmune a valores extremos. Evaluar la operación únicamente con el promedio llevaría a diagnosticar erróneamente un problema generalizado en la flota.

---

## 🛠️ Herramientas Utilizadas
* Google Sheets / Excel (Estadística Descriptiva y Fórmulas)
* Análisis de Tendencia Central (Media vs. Mediana)

---
✉️ **Contacto**: Matías Gómez

---

## 🛠️ Herramientas Utilizadas
* Google Sheets (Estadística Descriptiva, Filtros y Tablas)
* Análisis de Tendencia Central (Media vs. Mediana)

---✉️ **Contacto**: [Tu LinkedIn] | Matías Gómez
