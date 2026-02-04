# 📊 Análisis Comercial y Eficiencia Operativa: Marketplace Olist (Brasil)

## 🎯 Contexto del Negocio
Olist opera como un integrador logístico y comercial que conecta a miles de vendedores con los principales e-commerce de Brasil. En un ecosistema de marketplace de gran escala, el éxito no depende solo del volumen transaccional, sino de la **mezcla de categorías** y la **eficiencia logística**. La empresa enfrenta el reto de identificar qué productos realmente generan valor y cuáles están siendo erosionados por costos de envío elevados, impactando la sostenibilidad del modelo de negocio a largo plazo.

## 🚀 Objetivo del Proyecto
* **Evaluar el desempeño comercial** identificando las categorías que actúan como motores de ingresos.
* **Analizar la estructura de precios** para determinar si el crecimiento es impulsado por volumen o por ticket promedio.
* **Auditar el impacto logístico** calculando la relación costo de envío vs. precio de venta.
* **Priorizar esfuerzos comerciales** mediante la identificación de segmentos estratégicos bajo el principio de Pareto.

## 📊 Alcance del Análisis
* **Nivel de análisis:** Transaccional por orden, producto y categoría.
* **Datos incluidos:** +110,000 órdenes procesadas entre 2016 y 2018.
* **Supuestos:** Se asume que el costo logístico registrado es el factor principal de fricción en la conversión de categorías de bajo ticket promedio.

## 💡 Principales Insights (EDA)
* **Concentración de Ingresos (Pareto):** Se confirmó que el **20% de las categorías genera aproximadamente el 80% del ingreso total**, destacando *health_beauty*, *watches_gifts* y *bed_bath_table* como pilares financieros.
* **Driver de Crecimiento:** El modelo de ingresos actual está apalancado en el **alto volumen de ventas** de productos de ticket medio, más que en la venta de artículos de lujo o high-end.
* **Fuga de Rentabilidad:** Se detectaron categorías donde el costo logístico representa una proporción crítica del precio de venta, sugiriendo ineficiencias en la distribución geográfica o en el embalaje.
* **Oportunidad de Portafolio:** Existe una alta dispersión de precios en categorías clave, lo que indica espacio para una estrategia de *upselling* dirigida.

## 🛠️ Enfoque Analítico y Modelo
* **Análisis de Concentración:** Aplicación del Principio de Pareto para segmentar categorías "A" (estratégicas) de las "C" (marginales).
* **Análisis de Dispersión:** Correlación entre volumen de pedidos y precio unitario para entender la elasticidad visual del catálogo.
* **Métricas de Fricción Logística:** Creación de un ratio de costo de envío/precio para identificar categorías con márgenes en riesgo.

## 📈 Métricas y Resultados
* **GMV (Gross Merchandise Volume):** Identificación total del valor transaccionado por periodo.
* **Average Ticket:** Cálculo de la media transaccional por categoría para definir el perfil del consumidor.
* **Freight Ratio:** Identificación de las 5 categorías con mayor costo logístico relativo, permitiendo focalizar renegociaciones con transportistas.

## 🧠 Impacto en Decisiones de Negocio
* **Optimización de Marketing:** Redirección del presupuesto publicitario hacia las categorías del "Top 20%" que aseguran el flujo de caja.
* **Estrategia Logística:** Base de datos lista para que el equipo de Operaciones negocie tarifas planas o subsidios en categorías con *Freight Ratio* crítico.
* **Gestión de Sellers:** Identificación de categorías subexplotadas donde se requieren captar nuevos vendedores para diversificar la oferta.

## 💻 Tecnologías y Herramientas
* **Lenguaje:** Python
* **Librerías principales:** Pandas (Manipulación), NumPy (Cálculo), Matplotlib & Seaborn (Visualización).
* **Entorno de trabajo:** Jupyter Notebook / VS Code.

## 📂 Estructura del Repositorio
```text
├── data/
│   ├── olist_orders_dataset.csv     # Datos transaccionales
│   ├── olist_products_dataset.csv   # Catálogo de productos
│   └── category_name_translation.csv # Diccionario de categorías
├── notebooks/
```

## 📝 Conclusiones
El análisis revela un marketplace saludable pero con una dependencia marcada de categorías **core**. La rentabilidad no está solo en vender más, sino en equilibrar el costo logístico. Este proyecto demuestra que una visión orientada a datos permite separar el "ruido" del volumen transaccional de la "señal" de la rentabilidad real, permitiendo a Olist tomar decisiones de escalabilidad informadas.

## 🔮 Próximos Pasos / Mejoras Futuras
* **Segmentación de Vendedores:** Implementar un modelo de clustering (K-Means) para clasificar a los vendedores por su nivel de cumplimiento y volumen.
* **Análisis Geográfico:** Integrar datos de geolocalización para optimizar las rutas logísticas y reducir el *Freight Ratio*.
* **Predicción de Ventas:** Desarrollar un modelo de series temporales para anticipar picos de demanda en categorías estacionales.
