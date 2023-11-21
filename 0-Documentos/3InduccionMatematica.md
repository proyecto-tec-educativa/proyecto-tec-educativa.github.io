---
layout: default
tema: Rosa
tema_oscuro: RosaOscuro
title: Inducción Matemática
description: "Una herramienta fundamental"
last_modified_date: 2023-11-01T09:00:00+0000
has_children: true
nav_order: 3
---

# El Principio de Inducción Matemática
{:.fs-9}

Una herramienta fundamental
{:.fs-6 .fw-300}

---

A continuación, enunciaremos y demostraremos de dos maneras distintas una de las propiedades más importantes relacionadas con los números naturales.

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">1 </span> Principio de Inducción matemática
Para cada número natural \\(n\\), sea \\(p(n)\\) una frase abierta en \\(\mathbb{N}\\). Si

1. \\(p(1)\\) es un enunciado verdadero, y
2. Para cada \\(k\in\mathbb{N}\\), si \\(p(k)\\) es un enunciado verdadero, \\(p(k+1)\\) también es un enunciado verdadero.

Entonces \\(p(n)\\) es un enunciado verdadero para cada \\(n\in\mathbb{N}\\).

#### Nota

*A la primera propiedad se le suele llamar* **Base de inducción***, y a la segunda* **Paso inductivo***. Sin embargo, dada la diversidad de proposiciones equivalentes al Principio de Inducción matemática, estas propiedades cambian ligeramente entre una y otra.*

#### Demostración 1 (Por el Principio del Buen orden)
Sea \\(S\\) un subconjunto de \\(\mathbb{N}\\) que consiste en aquellos naturales \\(j\\) para los cuales \\(p(j)\\) es falso, *i.e.*
    
$$S=\left\{j\in\mathbb{N}\;|\;p(j) \text{ es falso}\right\}$$
{:.math}

Veamos que \\(S=\varnothing\\).
    
Procedamos por contradicción. Supóngase que \\(S\ne\varnothing\\). Por el **Principio del buen orden**, \\(S\\) tiene un mínimo, digamos \\(d\\). Como \\(d\in S\\), \\(p(d)\\) es falsa, pero \\(p(1)\\) es verdadera por <span class="deg-sitio deg-sitio-texto">1</span>, de ahí que \\(d\ne 1\\). Luego, \\(d\ge 2\\) pues \\(d\\) es un entero no negativo, así \\(d-1\ge 1\\), por lo que \\(d\in\mathbb{N}\\). Como \\(d-1< d\\), se tiene que \\(d-1\notin S\\), ya que \\(d\\) es el elemento más pequeño de \\(S\\), de ahí que \\(p(d-1)\\) sea verdadera. La hipótesis <span class="deg-sitio deg-sitio-texto">2</span> implica que \\(p\Big((d-1)+1\Big)\\) es verdadera, es decir, \\(p(d)\\) es verdadera, lo cual no es posible, dado que \\(d\in S\\) y por tanto \\(p(d)\\) es falsa. Contradicción

Luego \\(S=\varnothing\\) y

$$\forall n \in\mathbb{N}:p(n) \text{ es verdadera}$$
{:.math}

#### Demostración 2 (Por conjuntos inductivos)

Sea

$$A=\left\{j\in\mathbb{N}\;|\;p(j) \text{ es verdadero}\right\}$$
{:.math}

Es fácil notar que

1. \\(1\in A\\) pues \\(p(1)\\) es verdadera
2. Para cada \\(r\in\mathbb{R}\\), si \\(r\in A\\), entonces \\(p(r)\\) es verdadera, luego \\(p(r+1)\\) es verdadera y así \\(r+1\in A\\).

En consecuencia \\(A\\) es inductivo. Luego \\(\mathbb{N}\subseteq A\\). Pero por construcción \\(A\subseteq \mathbb{N}\\). Luego \\(A=\mathbb{N}\\), y así se concluye que

$$\forall n \in\mathbb{N}:p(n) \text{ es verdadera}$$
{:.math}

## ¿Y todo para qué?

Puedes averiguarlo navegando por la sección.