# 🧠 Calculadora VMC Mundoclima con IA Comercial

![Proyecto](https://img.shields.io/badge/proyecto-VMC%20Calculator-blue)
![Normativa](https://img.shields.io/badge/Normativa-CTE%20HS3-green)
![Tecnología](https://img.shields.io/badge/Tecnología-HTML%20%7C%20JS%20%7C%20Tailwind-orange)
![IA](https://img.shields.io/badge/IA-Chatbot%20RAG-purple)
![Estado](https://img.shields.io/badge/Estado-Operativo-success)

Primera **calculadora de ventilación mecánica controlada (VMC)** con **asistente de inteligencia artificial comercial integrado**.

Esta herramienta permite calcular automáticamente sistemas de ventilación residencial según la normativa **CTE HS3**, generar la **lista de materiales**, y producir un **informe técnico en PDF** listo para entregar al cliente.

Incluye además un **asistente IA llamado Lucía** que ayuda al usuario a interpretar los cálculos y entender la configuración del sistema.

---

# 🎯 Objetivo del proyecto

En muchas empresas del sector HVAC los cálculos de ventilación se realizan mediante hojas Excel poco intuitivas y propensas a errores.

Este proyecto nace con el objetivo de:

- Automatizar cálculos técnicos de ventilación
- Facilitar el trabajo de comerciales
- Reducir errores de dimensionamiento
- Generar documentación técnica automática
- Introducir **IA aplicada al soporte técnico comercial**

---

# ⚙️ Funcionamiento general

El proceso de cálculo sigue el siguiente flujo:

Usuario / Comercial  
↓  
Introducción de datos de vivienda  
↓  
Motor de cálculo (CTE HS3)  
↓  
Cálculo de caudales de ventilación  
↓  
Lista de materiales + Informe PDF  
↓  
Asistente IA Lucía

---

# 📐 Normativa aplicada

La herramienta utiliza el **Documento Básico HS3 del Código Técnico de la Edificación (CTE)**.

Esta normativa establece los **caudales mínimos de ventilación en viviendas**.

Se distinguen dos tipos de estancias.

### Locales secos
- dormitorios  
- salones  
- despachos  

### Locales húmedos
- baños  
- cocinas  
- lavaderos  

La calculadora determina automáticamente:

- caudal por estancia  
- caudal total de ventilación  

---

# 🔧 Selección automática del sistema

Según el caudal total calculado se selecciona automáticamente el sistema de distribución.

### Sistema 125 mm

Para caudales:

0 – 150 m³/h

### Sistema 160 mm

Para caudales:

151 – 300 m³/h

Esto garantiza velocidades adecuadas de aire dentro de los conductos evitando:

- ruido  
- pérdidas de carga  
- sobredimensionamiento  

---

# 🧮 Cálculo de conductos

Para simplificar el dimensionamiento inicial se utiliza una regla práctica basada en la superficie de la vivienda.

**1 rollo de conducto cada 50 m²**

Ejemplo:

150 m² vivienda → 3 rollos de conducto

---

# 🔩 Componentes calculados automáticamente

La herramienta genera automáticamente una **lista de materiales (BOM)** incluyendo:

### Conductos
- rollos semiflexibles

### Clips
- clips rojos  
- clips grises  

### Cajas de distribución
Calculadas según número de estancias.

### Plenums
1 plenum por estancia.

### Conducto aislado
Si el usuario no introduce valores se asignan:

20 metros totales  
10 impulsión  
10 retorno  

### Codos
Si no se especifica:

2 codos por defecto

### Silenciadores
Por defecto:

1 impulsión  
1 retorno

---

# 🎚 Regulación del caudal

La herramienta permite dos sistemas de regulación.

### Bocas autoregulables

Seleccionadas automáticamente según caudal:

- 15 m³/h  
- 30 m³/h  
- 45 m³/h  
- 60 m³/h  
- 90 m³/h  
- 120 m³/h  

### Reguladores de caudal constante (MVF)

En este modo se añade:

- regulador MVF  
- boca decorativa  

Opciones disponibles:

- SlimValve  
- Rondo  
- Kvadro  
- SR  

---

# 📄 Generación de informe técnico

La herramienta genera automáticamente un **informe técnico PDF DIN A4** que incluye:

- datos del proyecto  
- cálculo de ventilación  
- lista de materiales  
- precios  
- descuento aplicado  
- subtotal  

El informe incluye la nota:

"Los precios pueden variar y no constituyen una oferta vinculante."

---

# 🤖 Asistente IA — Lucía

Lucía es un asistente conversacional integrado que permite:

- explicar cómo funciona la calculadora  
- interpretar los resultados  
- resolver dudas sobre ventilación  
- explicar la normativa HS3  

El asistente utiliza un sistema **RAG (Retrieval Augmented Generation)** basado en documentación técnica.

---

# 🧱 Arquitectura del sistema

Usuario / Comercial  
↓  
Interfaz Web (HTML + JavaScript)  
↓  
Motor de cálculo HS3  
↓  
Lista de materiales + Informe PDF  
↓  
Chatbot IA Lucía  
↓  
Base de conocimiento (RAG + documentación técnica)

---

# 🖥 Tecnologías utilizadas

- HTML  
- CSS  
- JavaScript  
- TailwindCSS  
- jsPDF  
- NotebookLM (RAG)  
- IA generativa  

---

# ▶️ Cómo ejecutar la herramienta

La aplicación **no requiere instalación**.

1️⃣ Descargar el archivo:

calculadora_vmc_mundoclima.html

2️⃣ Colocar en la misma carpeta:

logo_mundoclima.png  
lucia.png  
tecnicos.png  

3️⃣ Abrir el archivo en el navegador.

---

# 📈 Impacto del proyecto

Esta herramienta permite:

- acelerar la preparación de ofertas  
- reducir errores de cálculo  
- facilitar el trabajo comercial  
- introducir inteligencia artificial en procesos HVAC  

---

# 👨‍💻 Autor

**Jordi Salvador Noya**

Jefe de Producto  
División de Ventilación  
Salvador Escoda S.A.

Proyecto desarrollado dentro del:

**Master Online en IA e Innovación 2026 – Founderz**
