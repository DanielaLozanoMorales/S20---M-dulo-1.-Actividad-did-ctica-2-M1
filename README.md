# Simulación de Yahtzee - Método de Montecarlo

Este proyecto consiste en un programa desarrollado en Python que simula el juego clásico de **Yahtzee** para dos jugadores.  
El objetivo principal es aplicar el **Método de Montecarlo** para analizar cómo influye una estrategia de decisión en un entorno dominado por el azar.

---

## Descripción del juego

- **Jugadores:** 2 compitiendo por turnos  
- **Lanzamientos:** Hasta 3 por turno  
- **Dados:** 5 dados convencionales de 6 caras  
- **Estrategia:**  
  El programa identifica qué dados conviene conservar y los "congela" para mejorar la jugada en los siguientes lanzamientos del turno.

---

## Metodología (Montecarlo)

Para lograr una simulación realista, se aplican los siguientes principios:

- **Generación de azar:**  
  Cada cara del dado tiene una probabilidad uniforme de `1/6`.

- **Lógica de decisión:**  
  No todo se deja al azar. Una función analiza la frecuencia de los valores obtenidos y decide cuáles conservar para maximizar el puntaje.

- **Repetición:**  
  Se ejecutan múltiples partidas para observar la probabilidad de obtener combinaciones como:
  - Póker
  - Full House
  - Yahtzee

---

## Estructura del código

El programa está organizado en funciones clave:

- `lanzar_dados`  
  Completa el conjunto de 5 dados respetando los dados retenidos.

- `evaluar_jugada`  
  Actúa como "juez", asignando categorías como:
  - Trío
  - Full House
  - Escaleras

- `simular_estrategia`  
  Decide qué dados mantener según la frecuencia más alta.

- `jugar`  
  Controla el flujo del juego, los turnos y el conteo final de puntos.

---

## Para ejecutarlo:

1. Copiar el código en un archivo `.py`
2. Ejecutar en la terminal:

```bash
python nombre_del_archivo.py

```bash
python nombre_del_archivo.py
