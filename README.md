# Modelos de datos de alta frecuencia financiera

Trabajo de Fin de Grado del **Grado en Matemáticas** de la Universidad de Cádiz (junio de 2025), tutorizado por Miguel Ángel Sordo.

## De qué trata

Los mercados financieros generan órdenes de compra y venta en fracciones de segundo. Las **series temporales de alta frecuencia** permiten estudiar ese comportamiento con mucho detalle, pero tienen problemas propios: las operaciones no ocurren a intervalos regulares, los precios rebotan entre oferta y demanda y el ruido de microestructura sesga las estimaciones.

El trabajo construye el marco matemático para modelizar estos datos y lo aplica a **datos reales tick a tick de las acciones de Caterpillar** (base de datos NYSE TAQ, enero de 2010; 155.267 transacciones solo entre el 4 y el 8 de enero).

## Contenido

1. **Fundamentos matemáticos:** máxima verosimilitud, mínimos cuadrados y los teoremas de Wold, Cramér, Donsker, Engle, Glosten-Milgrom y Kyle, además del lema de Itô.
2. **Negociación no sincrónica:** cómo la falta de sincronía entre operaciones distorsiona las conclusiones sobre la rentabilidad.
3. **Diferencial bid-ask:** modelo de Roll, test de Dickey-Fuller, análisis ACF/PACF y ajuste de un **ARIMA(4,1,2)** a los rendimientos logarítmicos intradía.
4. **Modelos de variación de precios:** **probit ordenado** y modelo de descomposición (Bernoulli y geométrica), estimados por máxima verosimilitud.
5. **Modelos duracionales:** modelos **ACD** de Engle y Russell, con ajustes **EACD(1,1)** y **WACD(1,2)** tras eliminar el patrón diurno con splines; procesos de Wiener e Itô y movimiento browniano.
6. **Volatilidad realizada:** estimación con rendimientos intradía y efecto del intervalo de muestreo (enero a mayo de 2010).
7. **Ruido de microestructura:** estimador de dos escalas, estimador kernel realizado, pre-promediado y modelo de Roll (1984) para el spread efectivo.

## Tecnologías

R / RStudio (`ggplot2`, `gridExtra`, `dplyr`, `tidyr`, `readxl`, `MASS`, `auto.arima`) · LaTeX

## Documento

[`TFGFINAL.pdf`](TFGFINAL.pdf): memoria completa, con el código R de cada análisis.

## Autor

**Josué Hormiga Benítez**

- LinkedIn: [Josué Juan Hormiga Benítez](https://www.linkedin.com/in/josu%C3%A9-juan-hormiga-ben%C3%ADtez-098499334/)
- GitHub: [@josuehormigabenitez22-cmd](https://github.com/josuehormigabenitez22-cmd)
