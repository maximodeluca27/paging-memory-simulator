# paging-memory-simulator
Simulador didáctico de paginación con FIFO para la cátedra de Arquitectura de Computadores (UTN FRBA)

# Simulador de Paginación – FIFO

Este proyecto implementa un simulador didáctico de **paginación por demanda**
utilizando el algoritmo de reemplazo **FIFO**, pensado para la materia
**Arquitectura de Computadores / Sistemas Operativos**.

## 📄 Archivo de accesos a memoria

El archivo `memory_accesses.csv` representa una traza realista de accesos a
memoria virtual.

Cada fila indica:
- `time`: instante del acceso
- `pid`: proceso que ejecuta
- `virtual_page`: página virtual accedida por el proceso

Cada proceso posee su propio espacio de direcciones virtuales.

## 🧠 Simulación

La simulación:
- utiliza una cantidad configurable de **frames físicos**
- detecta **page faults**
- aplica reemplazo FIFO cuando la memoria está llena
- registra cada acceso en una base SQLite

## 📊 Métricas

El simulador calcula:
- total de accesos a memoria
- cantidad de page faults
- tasa de page faults global
- métricas separadas por proceso

## 🎓 Objetivo didáctico

El objetivo es visualizar:
- la diferencia entre páginas y frames
- el impacto de la cantidad de frames
- la interferencia entre procesos
- el funcionamiento de FIFO en memoria virtual

## 🛠️ Tecnologías utilizadas

- **Python 3**
- **Pandas** – procesamiento de accesos a memoria
- **SQLite** – persistencia del log y consultas SQL
- **Google Colab** – entorno de ejecución
- **Git & GitHub** – control de versiones


