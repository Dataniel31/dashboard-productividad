# 📊 Dashboard de Productividad – Power BI

![Dashboard de Productividad](https://raw.githubusercontent.com/Dataniel31/dashboard-productividad/refs/heads/main/dashboard.png)

Este proyecto es un **dashboard interactivo** desarrollado en **Power BI** para analizar la **productividad en la producción de piezas** en diferentes ubicaciones. El objetivo principal es proporcionar una visión clara y concisa para la **toma de decisiones** basadas en la calidad, productividad y rendimiento por operador.

## 🔍 Descripción General

El dashboard incluye las siguientes visualizaciones y cálculos:

### 1. 🛠 **Piezas Buenas Producidas**
   - **Medida DAX:** `Total Piezas Buenas producidas = SUM('Producción'[Piezas producidas])`
   - Esta tarjeta muestra el número total de piezas que cumplen con los estándares de calidad.

### 2. 🚫 **Piezas Rechazadas**
   - **Medida DAX:** `Total Piezas Rechazadas = SUM('Producción'[Piezas rechazadas])`
   - Visualiza el total de piezas rechazadas debido a defectos u otros problemas.

### 3. 🔢 **Total de Piezas Producidas**
   - **Medida DAX:** `Total Piezas Producidas = [Total Piezas Buenas producidas] + [Total Piezas Rechazadas]`
   - Representa el total de piezas producidas, sumando las buenas y las rechazadas.

### 4. ⏱️ **Total Horas Productivas**
   - **Medida DAX:** `Total Horas Productivas = CALCULATE(SUM('Producción'[Total Horas]), 'Producción'[Obstáculos]=BLANK())`
   - Muestra las horas efectivas trabajadas sin obstáculos que interfirieran en la producción.

### 5. 🌍 **Horas Productivas vs Horas No Productivas por Ubicación**
   - **Medida Horas No Productivas DAX:** `Total Horas No Productivas = CALCULATE(SUM('Producción'[Total Horas]), 'Producción'[Obstáculos]<>BLANK())`
   - Gráfico de barras que compara las horas productivas y no productivas en distintas ubicaciones (Japón, Canadá, China, etc.).

### 6. 📈 **Piezas Buenas Producidas por Mes**
   - Utiliza la medida `Total Piezas Buenas Producidas` para visualizar la tendencia mensual de piezas de calidad producidas.

### 7. ✅ **% de Calidad**
   - **Medida DAX:** `% Calidad = [Total Piezas Buenas producidas] / [Total Piezas Producidas]`
   - Mide el porcentaje de piezas que pasan el control de calidad.

### 8. ⚙️ **% de Productividad**
   - **Medida DAX:** `% Productividad = [Total Horas Productivas] / SUM('Producción'[Total Horas])`
   - Indica la relación entre las horas productivas y el total de horas trabajadas.

### 9. 👷 **Productividad por Operador**
   - Filtro interactivo que permite analizar la productividad segmentando por operador.

### 10. 📅 **Filtro por Mes**
   - Filtro que permite ajustar los datos para analizar la productividad y los resultados por mes específico.

## 📌 Tecnologías Utilizadas

- **Power BI**: Herramienta principal para la visualización y análisis de datos.
- **DAX (Data Analysis Expressions)**: Para la creación de medidas personalizadas que permiten realizar cálculos avanzados.
- **Power Query**: Para la transformación y modelado de los datos.

## 🎯 Resultados Clave

- **Análisis detallado de más de 3 millones de piezas producidas**.
- **Monitorización de más de 30 mil horas productivas** en diferentes ubicaciones.
- **Incremento de calidad al 99.32%**, optimizando la productividad en cada etapa de la producción.

## 🏆 Conclusiones

Este dashboard proporciona una visión clara y completa del rendimiento de la producción, permitiendo identificar áreas de mejora en la eficiencia operativa y tomar decisiones más informadas. Las visualizaciones y los cálculos avanzados en Power BI permiten realizar un seguimiento detallado de los resultados clave como la calidad y productividad por operador y ubicación.

## 🔗 Contacto

Para más información sobre este proyecto o posibles colaboraciones:

- **Daniel Alex Suclle Luque**
- **Email:** [tu.email@ejemplo.com](mailto:alexdspe02@gmail.com)
- **LinkedIn:** [TuPerfilLinkedIn](https://www.linkedin.com/in/alexsuclle/)

---

⌨️ con ❤️ por [Daniel Alex Suclle Luque](https://github.com/Dataniel31)
