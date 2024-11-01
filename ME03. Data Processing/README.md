# Estimación del riesgo de deserción de los beneficiarios en Sapiencia

## ¿Qué es Sapiencia?

Sapiencia es una entidad adscrita al distrito de Medellín cuya misión es otorgar créditos condonables o becas a los nacidos o residentes por al menos 3 años en el municipio de Medellín (Medellín, 2023), esto con el fin de garantizar el acceso y permanencia a la educación superior. Uno de los principales dilemas que ha tenido la entidad, es el predecir el costo que puede suponer un beneficiario durante sus estudios postsecundarios, dado la gran variedad de universidades y programas que existen en el Valle de Aburrá. Por ello, se desarrolló un modelo predictivo con el objetivo de mejorar la gestión del recurso al estimar la proyección financiera para cada estudiante en su ciclo académico.

## Objetivo del Proyecto

Mejorar la gestión del recurso económico al estimar la proyección financiera para cada estudiante en su ciclo académico e identificar qué beneficiarios pueden ser susceptibles de abandonar sus estudios postsecundarios y por ende su crédito o beca en Sapiencia.


## Base Datos

La base de datos fue extraída del registro histórico de los beneficiarios del fondo línea pregrado de Sapiencia desde el semestre 2014-1 hasta el semestre 2024-2. La base de datos inicial llamada _Data_Sapiencia_ la cual cuenta con  677060  filas y 65 columnas.

\begin{table}[h!]
\centering
\begin{tabular}{|l|r|}
\hline
\textbf{Nombre de la Columna} & \textbf{Cantidad de Valores} \\
\hline
ID USUARIO (TI) & 677060 \\
CONVOCATORIA & 677060 \\
FONDO SAPIENCIA & 677060 \\
GÉNERO & 677055 \\
FECHA DE NACIMIENTO & 662136 \\
ESTRATO & 676464 \\
COMUNA DE RESIDENCIA & 677052 \\
MUNICIPIO DE RESIDENCIA & 677060 \\
VICTIMA DEL CONFLICTO ARMADO & 676464 \\
HECHO VICTIMIZANTE & 676464 \\
SITUACIÓN DE DISCAPACIDAD & 676464 \\
TIPO DE DISCAPACIDAD & 676464 \\
PUNTAJE SISBEN & 665366 \\
LGTBI & 666951 \\
MODALIDAD & 677059 \\
MONTO MATRÍCULA & 677060 \\
MONTO SOSTENIMIENTO & 677060 \\
MONTO TOTAL & 677060 \\
IES & 677060 \\
PROGRAMA & 677060 \\
DURACIÓN DEL PROGRAMA & 676476 \\
TOTAL CRÉDITOS DE LA CARRERA & 669348 \\
ESTADO GENERAL & 676477 \\
PERIODO RENOVADO & 677060 \\
ESTADO SEMESTRAL & 677060 \\
MOTIVO ESTADO & 676469 \\
SEMESTRES A FINANCIAR & 677060 \\
SEMESTRE DE INGRESO & 676476 \\
GIROS REALIZADOS & 677060 \\
GIROS PENDIENTES & 677060 \\
\hline
\end{tabular}
\caption{Tabla de Columnas y Cantidad de Valores}
\label{tab:columnas_valores}
\end{table}



