# REPORTES PREDEFINIDOS Y AD HOC PARA UNA FARMACIA ONLINE MINORISTA
<p align="left">
El repositorio contiene consultas SQL con diferentes niveles de complejidad. El punto de almacenamiento de los datos de la empresa es en un datalake en buckets de Amazon S3. A través a Amazon Athena 
realizaba las consultas utilizando el motor de consultas de Trino/Presto. 
	
</p>

## 🔍 Breve síntesis de algunas consultas y reportes realizados:
<p>

1️⃣ **Reporte de Comisiones a Pagar - Área Convenios**: 

Obtiene un resumen de ventas y comisiones de productos en función de las facturas emitidas, excluyendo ciertos productos y filtrando por instituciones específicas. Calcula las ventas brutas y netas, y la comisión correspondiente a pagar para cada institución y producto, agrupado por fecha y otros detalles.

2️⃣ **Reporte Mensual para envío a Proveedores(laboratorios) - Área Comercial**

Información de ventas de productos específicos que pertenecen a un laboratorio durante julio de 2024. Para cada producto, lote y mes, calcula el precio promedio de venta, las unidades totales vendidas y la utilidad generada por las ventas, y presenta estos resultados agrupados y ordenados por SKU, nombre del producto, lote y mes.


3️⃣ **Información de correos electrónicos de clientes en listado de productos requeridos - 'Area Marketing'**

Realización de una consulta que permite obtener información de correos electrónicos de personas que hayan solicitado productos sin disponibilidad para la venta. 


4️⃣ **Información sobre control de ventas y stock para el canal de venta B2B - Área Operaciones** 

La razón detrás de esta consulta era analizar el flujo de ventas de uno de los canales de venta que maneja la empresa para promover acciones tendientes al aumento de las mismas. 
La consulta permitió obtener un resumen de las ventas realizadas en el canal B2B en el último mes. Para cada transacción, muestra la fecha de compra, el canal, el número de la orden, una lista de los productos comprados junto con su SKU, una lista de los productos con su stock disponible y el total de las ventas.


5️⃣  **Información sobre compras realizadas por clientes durante un período de tiempo determinado - 'Area Marketing** 

Se obtiene un resumen de las transacciones realizadas a través del canal Ecommerce en los últimos tres meses. Filtra las transacciones de acuerdo a determinado estado de una orden y también omite las transacciones asociadas a clientes reservados. 

6️⃣ **Información de ventas generadas con la utilización de cupones de descuentos de determinados profesionales médicos - Área Convenios**

Se obtiene información detallada sobre cada transacción, como las fechas de creación y facturación, el número de orden, el estado de la transacción, el SKU y descripción del producto, las unidades vendidas, el precio unitario y total de la venta, la institución asociada y el cupón utilizado.

7️⃣ **Reporte sobre un Programa de descuentos por unidades de compra sobre un producto - Área Comercial**

Informe de las transacciones más recientes para el producto específico que formaba parte del programa de descuentos, con detalles sobre las unidades vendidas y los cupones aplicados.

8️⃣ **Información de ventas de productos de la subcategoría control de peso - Área Marketing**

Obtención de todas las órdenes de la subcategoría "Control de Peso" que fueron entregadas a partir del 1 de enero de 2024, en las que no se requiere receta médica, y en las que no se aplicaron descuentos. Los resultados incluyen información como la fecha de la orden, el correo del cliente, el estado de la orden, y los tipos de descuentos aplicados en caso de existir. 

9️⃣ **Reporte SLA (Service Level Agreement) - 'Area Operaciones'**: 

El reporte permitió que la persona encargada del área de operaciones de la empresa pueda reconocer el tiempo de entrega de las órdenes de compra. El enfoque parte de analizar en particular, algunas de las etapas del proceso de una orden de compra y el tiempo transcurrido entre etapas.
El énfasis era determinar a su vez, cúanto tiempo se demoraba una orden cuando ingresaba en la fase de observación. Ha sido uno de los reportes con mayor nivel de complejidad por las transformaciones que debieron hacerse a los datos en la propia consulta. 

🔟 **Reporte s/ Institución médica y reconocimiento de recargos UF - Área Experiencia de Compra y Operaciones**

 La finalidad del reporte era analizar el comportamiento de ventas y el foco central era tomar conocimiento del día de la emisión de la facturación para verificar los recargos aplicados o no en función de los tiempos de ingreso.

*️⃣...

</p>

## 👾 Razón de lo realizado: 

#### Por mi cargo de Analista de Datos y Negocios para la empresa.  
