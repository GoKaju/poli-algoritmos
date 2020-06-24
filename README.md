# Trabajo colaborativo Analisis y verificación de algoritmos

## Deiby Julián Gómez Calderón - 1911020219

## Marlen Amézquita Casafús - 1911980319

## Santiago Cuervo Ramírez - 1911980303

### ¿Cuál es el problema abordado en el articulo?

Aunque en el articulo se plantea como un caso hipotético, a hoy es una realidad del día a día para muchas personas que acudieron a entidades haciendo uso de un producto en particular, los prestamos a través de hipotecas.

El riesgo de incumplimiento o pagos no oportunos durante la duración del contrato del préstamo hipotecario lleva a tomar por opción el refinanciamiento sin un respectivo análisis de las consecuencias que conlleva este nuevo contrato el cual puede terminar convirtiéndose en una deuda interminable o incluso la perdida del bien en medio.


### ¿En que contexto(s) existe el problema descrito?

Al ser un tema especifico, el problema existe al acceder a un préstamo por hipoteca, el cual está definido como un préstamo garantizado por bienes raíces, este se puede dar en dos condiciones, hipotecas de tipo fijo y tipo variable, las cuales consisten en calcular los intereses de la cuota dada una tasa porcentual inicial y calcular la tasa con la cual se generarán los intereses respectivamente.

El objetivo que se busca es encontrar una política óptima de refinanciación para el deudor, describiendo de forma algorítmica una solución para realizar refinanciamientos de la deuda a beneficio del deudor, de esta manera intentando disminuir considerablemente los gastos en pagos a intereses, para esto se deberá contemplar desde el inicio la cantidad de posibles refinanciamientos a los cuales el deudor podra acceder, la cual deberá ser estrictamente menor al número de cuotas pactadas, tambien se contemplan comisiones y costos de transacciones para garantizar una politica optima en todos los posibles escenarios para el deudor teniendo en cuenta que las mejores condiciones de mercado siempre estarán a favor del prestamista.


### ¿Grosso modo, en que consiste la solución de programación dinámica propuesta en el articulo?

En cuanto a la decisión de refinanciación de la hipoteca, ésta puede ser descrita por un proceso 𝛼, especificando en cada momento t = 0,..., T – 1 si el deudor hipotecario continúa con su posición en las condiciones normales 𝛼 = 0 o, si es posible, refinanciar su deuda 𝛼 = 1. 
La política de control elegida afecta a la dinámica de las variables de estado que caracterizan la posición del prestatario en el tiempo, estas variables son: el número de oportunidades de refinanciación disponibles dejadas para ejercitar en el futuro, el tipo de interés corriente, el flujo de efectivo a plazos para el periodo corriente, el resultado del saldo pendiente.
El prestamista desea seleccionar una política de control que minimice el coste asociado con el sistema de amortización con el propósito de ilustrar esta cuestión, consideramos la suma de todos estos pagos como una medida de este coste.
Para dicha solución cada que se presenta una posible opción de refinanciación se realiza un calculo de costos a mediano plazo continuando con el contrato actual contra los valores ofrecidos actuales del mercado teniendo en cuenta las tarifas de comisiones base, la decisión óptima es refinanciar la hipoteca, siempre que la nueva tasa de mercado sea inferior a la tasa de deuda pendiente.

### ¿Cuáles son los resultados de la solución, de acuerdo con lo reportado en el articulo?

Con la implantación de la solución propuesta por medio de la programación dinámica se logró optimizar los costos de las tasas de 3,5% a 1,4% a través de políticas de control optimo con reglas capaces de decidir en tiempos oportunos si se continúa la hipoteca con las condiciones actuales o validando con los datos actuales del mercado si es favorable realizar una refinanciación, sin embargo se evidenció que en la simulación los tiempos de refinanciación se usaron en un periodo de tiempo corto comparado con el tiempo completo del horizonte de amortización lo que para el ejemplo provocó no poder tomar decisiones más favorables en la optimización de los costos.

