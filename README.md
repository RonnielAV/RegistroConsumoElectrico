# RegistroConsumoElectrico 
# Calculadora y Registro de Consumo Eléctrico Residencial (República Dominicana)

Aplicación web simple para rastrear, calcular y visualizar tu consumo eléctrico residencial basado en la tarifa dominicana por tramos.

## 💡 Sobre el Proyecto

Este proyecto es una herramienta práctica desarrollada en HTML, CSS y JavaScript que se ejecuta completamente en tu navegador web. Permite llevar un registro de las lecturas de tu contador eléctrico en cada período de corte, calcular el consumo real entre fechas y estimar el costo asociado basándose en la estructura de la tarifa residencial por tramos (Tarifa No. 1) aplicada en la República Dominicana.

Es ideal para tener una idea clara de cómo tu consumo impacta en las diferentes bandas tarifarias y monitorear tus hábitos a lo largo del tiempo.

## ✨ Características

-   **Registro de Lecturas:** Ingresa fácilmente la fecha de corte y el valor del contador (kWh) en esa fecha.
-   **Cálculo por Período:** Calcula automáticamente el consumo de kWh entre cada lectura registrada.
-   **Estimación de Costo:** Proporciona un cálculo estimado del costo por período basado en los tramos de tarifa residencial (Nota importante abajo ⚠️).
-   **Tabla Detallada:** Muestra los registros, el consumo por período, el costo estimado y un desglose del cálculo por cada tramo tarifario.
-   **Resumen General:** Calcula y muestra el consumo total acumulado y el promedio de consumo por período.
-   **Visualización Gráfica:** Incluye un gráfico de barras interactivo (gracias a Chart.js) que muestra el consumo de kWh en cada período para identificar tendencias y picos.
-   **Edición y Eliminación:** Permite modificar o eliminar registros individuales si cometes un error o necesitas corregir datos.
-   **Persistencia de Datos:** Guarda automáticamente tus datos en el almacenamiento local del navegador (`localStorage`) para que no los pierdas al cerrar la página.
-   **Importar/Exportar:** Opción para guardar tus datos en un archivo JSON (`.json`) o cargar datos previamente guardados desde un archivo.

## 🛠️ Tecnologías Utilizadas

-   HTML5
-   CSS3
-   JavaScript (Vanilla JS)
-   [Chart.js](https://www.chartjs.org/) (para los gráficos)

## 🚀 Cómo Usar

1.  Clona el repositorio o descarga los archivos.
2.  Abre el archivo `Registro de Consumo Electrico.html` (o como lo hayas nombrado) directamente en tu navegador web. ¡No necesitas un servidor!
3.  Comienza a agregar tus lecturas de contador (Fecha de Corte y kWh al Corte).
4.  La tabla, el resumen y el gráfico se actualizarán automáticamente.
5.  Usa los botones de "Editar" y "Eliminar" en cada fila para gestionar tus registros.
6.  Los botones "Guardar Datos" y "Cargar Datos" te permiten exportar e importar tu historial.

## ⚠️ Nota Importante sobre la Estimación de Costo

El cálculo del costo en esta aplicación se basa estrictamente en la tarifa por kWh por tramos (Tarifa No. 1 residencial) tal como se define comúnmente para el servicio eléctrico en la República Dominicana (ej. por Edeeste, Edenorte, Edesur).

**Esta estimación es una referencia útil, pero NO representa el total de tu factura real.** Las facturas oficiales de las distribuidoras incluyen **cargos adicionales** que no están considerados aquí, tales como:

-   Cargo Fijo por Servicio
-   Ajuste por Combustible
-   Ajuste por Energía Comprada
-   ITBIS (Impuesto sobre Transferencias de Bienes Industrializados y Servicios)
-   Posibles Subsidios o Cargos Especiales

Además, las tarifas por tramo y otros cargos pueden ser revisados y modificados por las autoridades (como la SIE y la CNE). Si notas una discrepancia significativa con tu factura real, verifica si las tarifas programadas en la función `calcularDetalleCosto` (`tramos` array) necesitan ser actualizadas según la información más reciente de tu distribuidora o la Superintendencia de Electricidad (SIE).

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si encuentras errores, tienes sugerencias para mejorar el código o la funcionalidad (por ejemplo, añadir la posibilidad de configurar las tarifas o incluir otros cargos de la factura), siéntete libre de abrir un "Issue" o enviar un "Pull Request".

