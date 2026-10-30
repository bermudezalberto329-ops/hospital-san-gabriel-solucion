Análisis y documentación

## 1. Total de pacientes

La base de datos contiene **20 pacientes**. Este valor corresponde a los 20 registros ficticios incluidos en el caso clínico.

## 2. Edad promedio

La edad promedio es de **44,50 años**. Esto representa la edad media de los 20 pacientes registrados.

## 3. Temperatura promedio

La temperatura promedio registrada es de **37,12 °C**. El cálculo incluye las temperaturas disponibles en los 20 registros, ya que no existen valores faltantes para este campo.

## 4. Pacientes por sexo

La distribución por sexo es equilibrada:

- **F: 10 pacientes**
- **M: 10 pacientes**

Por lo tanto, cada sexo representa el 50 % de los pacientes de la base.

## 5. Pacientes por estado de atención

Los estados de atención se distribuyen de la siguiente manera:

- **Pendiente: 4 pacientes**
- **En atención: 6 pacientes**
- **Finalizada: 10 pacientes**

La categoría con mayor frecuencia es **Finalizada**, que corresponde a la mitad de los registros.

## 6. Saturación mínima de oxígeno

La saturación mínima registrada es de **91 %**. Este valor corresponde al paciente P009, cuyo registro presenta dificultad respiratoria y una saturación de 91 %.

## 7. Registros incompletos

Se identificó **1 registro incompleto** respecto a la saturación de oxígeno. Corresponde al paciente **P016**, para quien el caso clínico indica explícitamente que no se registró la saturación. La celda se dejó vacía, siguiendo la instrucción de no inventar información faltante.

## Inconsistencias y datos faltantes

La principal inconsistencia encontrada en los datos originales fue la **variación en los formatos de fecha, sexo y presentación de las variables clínicas**. Por ejemplo, las fechas aparecían como `20/10/2026`, `2026/10/23`, `24-10-2026` y `2026-10-25`; además, el sexo estaba expresado mediante términos como “mujer”, “masculino”, “F” y “M”.

Para facilitar el análisis, estos valores fueron normalizados a un único formato: fechas **AAAA-MM-DD**, sexo **F/M** y estados **Pendiente/En atención/Finalizada**. También se conservaron las variables numéricas como valores numéricos.

El único dato clínico faltante explícito es la saturación de oxígeno del paciente P016. No se realizó ninguna estimación o sustitución de este valor.

## Reflexión sobre privacidad clínica

Aunque los datos utilizados en este ejercicio son completamente ficticios, la información clínica requiere un manejo responsable porque puede contener datos capaces de identificar directa o indirectamente a una persona. En un entorno real, una base de datos hospitalaria debe limitar el acceso a la información según las funciones del personal autorizado y aplicar medidas de seguridad para evitar accesos, modificaciones o divulgaciones no permitidas. También es importante utilizar únicamente los datos necesarios para cada propósito y evitar compartir información clínica en repositorios públicos sin las medidas de protección correspondientes. La anonimización o seudonimización puede reducir riesgos, pero debe aplicarse de manera adecuada. La privacidad clínica protege la confidencialidad del paciente y contribuye a mantener la confianza entre las personas y las instituciones de salud.
