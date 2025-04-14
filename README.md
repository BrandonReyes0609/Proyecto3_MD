# Proyecto3_MD

# 📦 Proyecto 3 - Minería de Datos UVG

**Semana 1: Preparación de Datos y Análisis Inicial**

Este repositorio contiene el desarrollo de la Semana 1 del Proyecto 3 del curso de Minería de Datos (CC3074) en la Universidad del Valle de Guatemala. El proyecto se basa en el análisis del conjunto de datos de Olist, una empresa de comercio electrónico en Brasil.

---

## 📌 Objetivos de la Semana 1

- Realizar la propuesta inicial del proyecto.
- Explorar y entender los datos con un análisis exploratorio (EDA).
- Preprocesar el dataset principal (`olist_orders_dataset.csv`) y generar un archivo limpio y transformado.
- Documentar los resultados obtenidos.

---

## 📂 Estructura del proyecto

📁 Proyecto3_MD/
├── csv/                                                               # Archivos originales de datos
│   ├── olist_customers_dataset.csv
│   ├── olist_geolocation_dataset.csv
│   ├── olist_order_items_dataset.csv
│   ├── olist_order_payments_dataset.csv
│   ├── olist_order_reviews_dataset.csv
│   ├── olist_orders_dataset.csv
│   ├── olist_products_dataset.csv
│   ├── olist_sellers_dataset.csv
│   └── product_category_name_translation.csv
│
├── data_limpia/                                                   # Dataset limpio exportado
│   └── olist_orders_preprocesado.csv
│
├── main.ipynb                                                    # Notebook principal con todo el código de la Semana 1
└── README.md                                                # Este archivo


## 📊 Detalle de archivos `.csv` (carpeta `csv/`)

| Archivo                                   | Descripción                                                        |
| ----------------------------------------- | ------------------------------------------------------------------- |
| `olist_orders_dataset.csv`              | Dataset principal de pedidos. Contiene fechas y estados de entrega. |
| `olist_order_reviews_dataset.csv`       | Calificaciones y comentarios de los clientes.                       |
| `olist_customers_dataset.csv`           | Información del cliente y ubicación.                              |
| `olist_order_items_dataset.csv`         | Detalles por ítem del pedido: productos, precios y vendedores.     |
| `olist_products_dataset.csv`            | Características de los productos vendidos.                         |
| `olist_sellers_dataset.csv`             | Información de los vendedores.                                     |
| `olist_order_payments_dataset.csv`      | Información sobre métodos de pago y montos.                       |
| `olist_geolocation_dataset.csv`         | Datos de ubicación por código postal.                             |
| `product_category_name_translation.csv` | Traducción de las categorías de productos al inglés.             |

---

## 🧹 Dataset limpio generado (carpeta `data_limpia/`)

**Archivo:** `olist_orders_preprocesado.csv`

Este archivo fue generado tras aplicar limpieza y transformación al dataset de pedidos. Contiene:

- Columnas originales necesarias (`order_id`, `customer_id`, etc.)
- Variables nuevas:
  - `delivery_time_days`: días entre compra y entrega
  - `delay_vs_estimate`: diferencia entre entrega real y estimada
  - `estimated_days`: días prometidos desde la compra
  - `purchase_year`, `purchase_month`, `purchase_day`: descomposición temporal

Este dataset será utilizado en las próximas semanas para modelos de regresión y clasificación.

---

## 📓 Notebook (`main.ipynb`)

Contiene todo el código de la Semana 1:

- Propuesta del proyecto (Markdown)
- Carga y exploración de los datos
- Análisis exploratorio visual
- Estadísticas y correlaciones
- Limpieza de valores nulos
- Creación de nuevas variables
- Exportación del dataset limpio

---

## 👨‍💻 Integrantes del equipo

- Gabriela Mazariegos - 22513
- Giovanni Santos - 22523
- Santiago Pereira - 22318
- Brandon Reyes - 22992

---

## 🔗 Créditos

Datos proporcionados por [Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).
