# Estimación del riesgo de deserción de los beneficiarios en Sapiencia

## ¿Qué es Sapiencia?

Sapiencia es una entidad adscrita al distrito de Medellín cuya misión es otorgar créditos condonables o becas a los nacidos o residentes por al menos 3 años en el municipio de Medellín (Medellín, 2023), esto con el fin de garantizar el acceso y permanencia a la educación superior. Uno de los principales dilemas que ha tenido la entidad, es el predecir el costo que puede suponer un beneficiario durante sus estudios postsecundarios, dado la gran variedad de universidades y programas que existen en el Valle de Aburrá. Por ello, se desarrolló un modelo predictivo con el objetivo de mejorar la gestión del recurso al estimar la proyección financiera para cada estudiante en su ciclo académico.

## Objetivo del Proyecto

Mejorar la gestión del recurso económico al estimar la proyección financiera para cada estudiante en su ciclo académico e identificar qué beneficiarios pueden ser susceptibles de abandonar sus estudios postsecundarios y por ende su crédito o beca en Sapiencia.


## Base Datos

La base de datos fue extraída del registro histórico de los beneficiarios del fondo línea pregrado de Sapiencia desde el semestre 2014-1 hasta el semestre 2024-2. La base de datos inicial llamada __Data_Sapiencia__ la cual cuenta con  677060  filas y 65 columnas. Posteriormente, dado que se trata de información sensible, se anonimizó los datos excluyendo esas columnas que contenían información personal del beneficiario, donde se obtuvo finalmente las siguientes 30 variables:

| Nombre de la Columna           | Cantidad de Valores |
|--------------------------------|----------------------|
| ID USUARIO (TI)                | 677060              |
| CONVOCATORIA                   | 677060              |
| FONDO SAPIENCIA                | 677060              |
| GÉNERO                         | 677055              |
| FECHA DE NACIMIENTO            | 662136              |
| ESTRATO                        | 676464              |
| COMUNA DE RESIDENCIA           | 677052              |
| MUNICIPIO DE RESIDENCIA        | 677060              |
| VICTIMA DEL CONFLICTO ARMADO   | 676464              |
| HECHO VICTIMIZANTE             | 676464              |
| SITUACIÓN DE DISCAPACIDAD      | 676464              |
| TIPO DE DISCAPACIDAD           | 676464              |
| PUNTAJE SISBEN                 | 665366              |
| LGTBI                          | 666951              |
| MODALIDAD                      | 677059              |
| MONTO MATRÍCULA                | 677060              |
| MONTO SOSTENIMIENTO            | 677060              |
| MONTO TOTAL                    | 677060              |
| IES                            | 677060              |
| PROGRAMA                       | 677060              |
| DURACIÓN DEL PROGRAMA          | 676476              |
| TOTAL CRÉDITOS DE LA CARRERA   | 669348              |
| ESTADO GENERAL                 | 676477              |
| PERIODO RENOVADO               | 677060              |
| ESTADO SEMESTRAL               | 677060              |
| MOTIVO ESTADO                  | 676469              |
| SEMESTRES A FINANCIAR          | 677060              |
| SEMESTRE DE INGRESO            | 676476              |
| GIROS REALIZADOS               | 677060              |
| GIROS PENDIENTES               | 677060              |

## Limpieza de datos

Se realizo inicialmente el análisis de los valores nulos de las variavbles donde se obtuvieron los siguientes resultados:

| Nombre de la Columna           | Cantidad de Valores Nulos |
|--------------------------------|---------------------------|
| ID USUARIO (TI)                | 0                         |
| CONVOCATORIA                   | 0                         |
| FONDO SAPIENCIA                | 0                         |
| GÉNERO                         | 5                         |
| FECHA DE NACIMIENTO            | 14924                     |
| ESTRATO                        | 596                       |
| COMUNA DE RESIDENCIA           | 8                         |
| MUNICIPIO DE RESIDENCIA        | 0                         |
| VICTIMA DEL CONFLICTO ARMADO   | 596                       |
| HECHO VICTIMIZANTE             | 596                       |
| SITUACIÓN DE DISCAPACIDAD      | 596                       |
| TIPO DE DISCAPACIDAD           | 596                       |
| PUNTAJE SISBEN                 | 11694                     |
| LGTBI                          | 10109                     |
| MODALIDAD                      | 1                         |
| MONTO MATRÍCULA                | 0                         |
| MONTO SOSTENIMIENTO            | 0                         |
| MONTO TOTAL                    | 0                         |
| IES                            | 0                         |
| PROGRAMA                       | 0                         |
| DURACIÓN DEL PROGRAMA          | 584                       |
| TOTAL CRÉDITOS DE LA CARRERA   | 7712                      |
| ESTADO GENERAL                 | 583                       |
| PERIODO RENOVADO               | 0                         |
| ESTADO SEMESTRAL               | 0                         |
| MOTIVO ESTADO                  | 591                       |
| SEMESTRES A FINANCIAR          | 0                         |
| SEMESTRE DE INGRESO            | 584                       |
| GIROS REALIZADOS               | 0                         |
| GIROS PENDIENTES               | 0                         |

Se contó inicialmente con 677059 registros, de los cuales por su imposibilidad de imputar información se concretó con una base que cuenta con 643896. 

## Análisis descriptivo

