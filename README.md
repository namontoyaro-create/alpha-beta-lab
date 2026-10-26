
# Laboratorio: Minimax y Poda Alfa-Beta

## Descripción

Este proyecto implementa los algoritmos Minimax y Poda Alfa-Beta para resolver un árbol de decisión simplificado.

## Objetivo

Comparar el resultado y la eficiencia de Minimax frente a Poda Alfa-Beta.

## Instalación

```bash
python -m venv .venv
pip install -r requirements.txt
```

## Ejecución

```bash
python -m src.main
```

## Pruebas

```bash
python -m pytest --cov=src --cov-report=term-missing
```

## Preguntas de análisis

### 1. ¿Por qué Minimax y Alfa-Beta devuelven el mismo valor?

Porque ambos algoritmos siguen la misma estrategia de búsqueda adversarial. Alfa-Beta optimiza Minimax eliminando ramas que no pueden modificar la decisión final.

### 2. ¿Cuándo Alfa-Beta reduce más nodos?

Cuando las mejores jugadas se evalúan primero y permiten descartar otras alternativas.

### 3. ¿Qué ocurre si el árbol está mal ordenado?

La poda pierde eficiencia y puede terminar evaluando casi tantos nodos como Minimax.

### 4. ¿Cómo se aplicaría este algoritmo en ajedrez, damas o tres en raya?

Permite analizar posibles movimientos, anticipar las respuestas del adversario y seleccionar la jugada más conveniente.

## Resultados de las pruebas

- Pruebas unitarias: 5 aprobadas.
- Cobertura total: 77%.
- Cobertura de Minimax: 100%.
- Cobertura de Poda Alfa-Beta: 100%.

## Herramientas

- Python
- Visual Studio Code
- Git
- GitHub
- pytest
- GitHub Actions
- SonarCloud (opcional)
```
