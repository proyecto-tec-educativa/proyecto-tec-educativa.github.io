---
layout: default
tema: Rosa
tema_oscuro: RosaOscuro
title: Equivalencias
description: "Proposiciones equivalentes"
last_modified_date: 2023-11-01T09:00:00+0000
parent: Inducción Matemática
nav_order: 1
---

# Equivalencias
{:.fs-9}

Extendiendo lo aprendido
{:.fs-6 .fw-300}

---

Ya habíamos dicho que el Principio de Inducción Matemática tiene variantes en su enunciado, pero su función es la misma. Por ello, las presentaremos a continuación

### Proposición&nbsp;<span class="deg-sitio deg-sitio-texto">1 </span> Principio de Inducción fuerte

Para cada número natural \\(n\\), sea \\(p(n)\\) una frase abierta en \\(\mathbb{N}\\). Si

1. \\(p(1)\\) es un enunciado verdadero, y
2. Para cada \\(k\in\mathbb{N}\\), si \\(\displaystyle\bigwedge\limits_{j=1}^k p(j)\\) es un enunciado verdadero, \\(p(k+1)\\) también es un enunciado verdadero.

Entonces \\(p(n)\\) es un enunciado verdadero para cada \\(n\in\mathbb{N}\\).

#### Nota

*En este caso, a la primera propiedad se le suele llamar* **Base de inducción***, y a la segunda* **Paso inductivo***.

### Proposición&nbsp;<span class="deg-sitio deg-sitio-texto">2 </span> Principio de Inducción a la Cauchy

Para cada número natural \\(n\\), sea \\(p(n)\\) una frase abierta en \\(\mathbb{N}\\). Si

1. \\(p(2)\\) es un enunciado verdadero,
2. Para cada \\(k\in\mathbb{N}\\), si \\(p(k)\\) es un enunciado verdadero, \\(p(2k)\\) también es un enunciado verdadero.
3. Para cada \\(k\in\mathbb{N}\\), si \\(p(k)\\) es un enunciado verdadero y \\(k>1\\), entonces \\(p(k-1)\\) también es un enunciado verdadero.

Entonces \\(p(n)\\) es un enunciado verdadero para cada \\(n\in\mathbb{N}\\).

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">3 </span> Equivalencias del Principio de Inducción

Cada variante del **Principio de Inducción matemática**, y el **Principio del Buen Orden** son equivalentes entre sí.