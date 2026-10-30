# Hospital San Gabriel — Base de Datos Clínica

## Objetivo

El objetivo de este proyecto es transformar los registros clínicos ficticios y no estructurados del caso **Hospital San Gabriel** en una base de datos organizada, normalizada y adecuada para realizar análisis básicos mediante Excel.

La información corresponde a **20 pacientes ficticios** y fue utilizada exclusivamente con fines académicos.

---

## Diccionario de datos

| Campo | Descripción | Tipo de dato |
|---|---|---|
| Código | Identificador único del paciente | Texto |
| Edad | Edad del paciente en años | Numérico |
| Sexo | Sexo registrado del paciente (F/M) | Texto |
| Fecha de consulta | Fecha en la que se realizó la consulta | Fecha |
| Motivo | Motivo principal de consulta | Texto |
| Temperatura (°C) | Temperatura corporal registrada | Numérico |
| Frecuencia cardíaca (lpm) | Frecuencia cardíaca en latidos por minuto | Numérico |
| Saturación de oxígeno (%) | Saturación periférica de oxígeno | Numérico |
| Diagnóstico simulado | Diagnóstico indicado en el caso clínico | Texto |
| Estado de atención | Estado actual de la atención | Texto |

---

## Proceso de limpieza y organización

Para construir la base de datos se realizaron los siguientes pasos:

1. Se identificaron los campos presentes en los registros clínicos.
2. Se estructuraron los datos de los 20 pacientes en filas individuales.
3. Se utilizaron nombres de columnas claros y uniformes.
4. Las fechas fueron normalizadas al formato `YYYY-MM-DD`.
5. El sexo fue estandarizado utilizando las categorías `F` y `M`.
6. El estado de atención fue estandarizado en:
   - `Pendiente`
   - `En atención`
   - `Finalizada`
7. Las variables numéricas se almacenaron como valores numéricos para permitir cálculos en Excel.
8. El registro de saturación de oxígeno del paciente **P016** se dejó vacío debido a que este dato no estaba registrado en el caso clínico. No se realizó ninguna estimación o sustitución.
9. Se activaron filtros en la hoja de pacientes para facilitar la consulta de los registros.
10. Se calcularon indicadores básicos como número total de pacientes, edad promedio, temperatura promedio, distribución por sexo, estado de atención, saturación mínima y registros incompletos.
11. Se incorporaron gráficos para representar la distribución por sexo y por estado de atención.

---

## Archivos del proyecto

- **`Base_Datos_Hospital.xlsx`**: base de datos principal con las hojas `Pacientes` y `Análisis`.
- **`pacientes.csv`**: exportación de la hoja de pacientes en formato CSV UTF-8.
- **`analisis.md`**: interpretación de los indicadores y documentación de inconsistencias.
- **`README.md`**: descripción del proyecto, diccionario de datos y proceso de limpieza.

---

## Declaración sobre los datos

Todos los pacientes y datos incluidos en este proyecto son **completamente ficticios** y fueron proporcionados como parte de un caso académico del Hospital San Gabriel.

No corresponden a historias clínicas reales ni contienen información de pacientes reales. Por esta razón, la base de datos no debe utilizarse para diagnóstico, tratamiento o toma de decisiones clínicas.

El proyecto tiene exclusivamente fines **académicos y educativos** relacionados con la organización, limpieza y análisis básico de datos clínicos.
