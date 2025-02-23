# ALU_SigmaBits_Version1
ALU (Unidad Aritmético-Lógica) - Primera Versión Simple
Este proyecto implementa una Unidad Aritmético-Lógica (ALU) básica que realiza operaciones sobre dos números de 4 bits. Esta es la primera versión simple de la ALU, que soporta las siguientes operaciones, seleccionadas mediante un interruptor de control (SWITCH_MODE):

Suma: Realiza la suma de los dos números de entrada.
Resta: Realiza la resta de los dos números de entrada.
AND: Realiza una operación lógica AND bit a bit entre los dos números.
OR: Realiza una operación lógica OR bit a bit entre los dos números.
La ALU genera como salida dos displays de 7 segmentos que muestran el resultado de las operaciones en formato BCD, y un conjunto de LEDs que indican los resultados de las operaciones lógicas AND/OR. Además, incluye un LED indicador de desbordamiento (overflow) para las operaciones de suma y resta, que se enciende cuando ocurre un overflow.

Componentes utilizados
SUMADOR_RESTADOR: Componente encargado de realizar las operaciones de suma y resta.
AND_OR_UNIT: Componente que realiza las operaciones lógicas AND y OR.
bin2bcd: Componente que convierte el resultado binario en formato BCD para ser mostrado en los displays de 7 segmentos.
BCD_CASE_A01412388: Componente que controla los displays de 7 segmentos y mapea los valores BCD a las salidas correspondientes.
Esta versión del proyecto está diseñada como un modelo simple para la realización de operaciones aritméticas y lógicas, con visualización en displays de 7 segmentos y control de LEDs para representar resultados lógicos y de aritmética. Está pensada como una base para futuras mejoras y expansiones.

Instrucciones de uso
Conectar las señales de entrada: Los valores de entrada deben ser proporcionados en el formato de vectores de 4 bits (NUM_1 y NUM_2).
Seleccionar la operación: A través del puerto SWITCH_MODE, puedes seleccionar la operación a realizar:
00: Suma
01: Resta
10: AND
11: OR
Visualización de resultados: El resultado se mostrará en dos displays de 7 segmentos (D_RESULTADO_SR1 y D_RESULTADO_SR2), y los resultados de AND/OR en los LEDs (LED_RESULTADO).
Indicador de overflow: El LED LED_COUT_SIGN se enciende si ocurre un desbordamiento en las operaciones de suma o resta.
