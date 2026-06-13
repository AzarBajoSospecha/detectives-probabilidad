# Diagrama de árbol — Experimento A (guiado)

**Urna:** 5 bolas rojas (R), 3 azules (A), 2 verdes (V) · Total: 10 bolas  
**Extracción:** dos bolas **sin reemplazamiento**

> **Cómo usarlo:** la rama de la primera roja está completa y sirve de modelo.
> Las ramas de azul y verde tienen huecos `___` que debéis completar.
> Recordad: al sacar la primera bola, el total pasa de 10 a 9.

---

```mermaid
graph TD
    U["Urna (10 bolas)"]

    U -->|"5/10"| R["1.ª Roja (R)"]
    U -->|"3/10"| A["1.ª Azul (A)"]
    U -->|"2/10"| V["1.ª Verde (V)"]

    R -->|"4/9"| RR["2.ª Roja · P = 5/10 × 4/9 = 20/90"]
    R -->|"3/9"| RA["2.ª Azul · P = 5/10 × 3/9 = 15/90"]
    R -->|"2/9"| RV["2.ª Verde · P = 5/10 × 2/9 = 10/90"]

    A -->|"___/9"| AR["2.ª Roja · P = 3/10 × ___/9 = ___/90"]
    A -->|"___/9"| AA["2.ª Azul · P = 3/10 × ___/9 = ___/90"]
    A -->|"___/9"| AV["2.ª Verde · P = 3/10 × ___/9 = ___/90"]

    V -->|"___/9"| VR["2.ª ___ · P = 2/10 × ___/9 = ___/90"]
    V -->|"___/9"| VA["2.ª ___ · P = 2/10 × ___/9 = ___/90"]
    V -->|"___/9"| VV["2.ª ___ · P = 2/10 × ___/9 = ___/90"]
```

---

## Preguntas del expediente

Completad el árbol y responded:

| Pregunta | Desarrollo | Resultado |
|---|---|---|
| P (dos bolas rojas) | 5/10 × ___/9 = | ___ |
| P (una roja y una azul, en cualquier orden) | 5/10 × ___/9 + ___/10 × ___/9 = | ___ |
| ¿Cambia el resultado con reemplazamiento? ¿Por qué? | | |

---

## Pista

> Con reemplazamiento, antes de la segunda extracción la bola vuelve a la urna.
> ¿Cuántas bolas habría entonces? ¿Cambian las probabilidades de la segunda rama?

---

## Comprobación final

Cuando hayáis completado todas las ramas, sumad todas las probabilidades.  
Si está bien hecho, el resultado debe ser:

$$\text{Suma de todas las ramas} = \frac{\_\_\_}{90} = 1$$
