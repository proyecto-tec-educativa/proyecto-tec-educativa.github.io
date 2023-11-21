---
layout: default
search_exclude: true
tema: Especial
tema_oscuro: EspecialOscuro
title: Conjuntos Inductivos
description: "Entrenamiento del 14 de marzo de 2020"
last_modified_date: 2023-11-01T09:00:00+0000
parent: Preliminares
---

# Conjuntos&nbsp;<span class="deg-sitio deg-sitio-texto">Inductivos</span>&nbsp;<i class="jpa-all-default-rel-face_with_magnifying_glass jpa-2em"></i>
{:.fs-9}

Una forma de construir el conjunto \\(\mathbb{N}\\)
{:.fs-6 .fw-300}

### Definición&nbsp;<span class="deg-sitio deg-sitio-texto">1</span>

Un subconjunto \\(A\\) del conjunto \\(\mathbb{R}\\) se dice **Inductivo** si se satisfacen las siguientes proposiciones:

1. \\(1\in A\\)
2. Para cada \\(r\in\mathbb{R}\\), si \\(r\in A\\), entonces \\(r+1\in A\\).

### Definición&nbsp;<span class="deg-sitio deg-sitio-texto">2</span>

La intersección de todos los subconjuntos inductivos de \\(R\\) será el conjunto de los números naturales, y se denotará por \\(\mathbb{N}\\).

## Un teorema&nbsp;<span class="deg-sitio deg-sitio-texto">fundamental</span>

Esta es la propiedad que nos interesará de los conjuntos inductivos, y de \\(\mathbb{N}\\) en particular

### Teorema&nbsp;<span class="deg-sitio deg-sitio-texto">3</span>

1. \\(\mathbb{N}\\) es inductivo.
2. Si \\(A\\) es inductivo,  \\(\mathbb{N}\subseteq A\\).

#### Demostración 1

La expresión \\(\left(\forall x\in U:p(x)\implies q(x)\right)\implies \left(\forall x\in U:p(x)\implies\forall x\in U: q(x)\right)\\) es tautología.

Sea \\(I\\) el conjunto de todos los conjuntos inductivos. El siguiente razonamiento es válido, tomando como premisas la tautología anterior y, que para todo número real \\(x\\), si \\(x\\) es elemento de un conjunto inductivo, \\(x+1\\) también es un elemento de dicho conjunto inductivo:

$$
\begin{align*}
\forall x\in \mathbb{R}:&\left(\forall A\in I:x\in A\implies x+1\in A\right)\\
\forall x\in \mathbb{R}:&\left(\forall A\in I:x\in A\implies x+1\in A\right)\\
&\implies \left(\forall A\in I:x\in A\implies\forall A\in I: x+1\in A\right)\\
\hline
\forall x\in \mathbb{R}:&\:\forall A\in I:x\in A\implies\forall A\in I: x+1\in A
\end{align*}
$$
{:.math}

La conclusión nos dice que para todo número real \\(x\\), si \\(x\\) pertenece a cualquier conjunto inductivo, entonces \\(x+1\\) pertenece a cualquier conjunto inductivo.

Sea \\(\mathbb{N}\\) la intersección de todos los conjuntos inductivos. Por definición, \\(\mathbb{N}=\\{x\in R\|\forall A\in I: x\in A\\}\\).

En el siguiente razonamiento, si tomamos como premisas la definición del conjunto \\(\mathbb{N}\\) y que el número 1 pertenece a cualquier conjunto inductivo, concluimos que 1 pertenece al conjunto \\(\mathbb{N}\\): 

$$
\begin{align*}
\forall x\in \mathbb{R}:&\forall A\in I:x\in A\iff x\in \mathbb{N} \\
\forall A\in I:&\:1\in A\\
\hline
1\in \mathbb{N}
\end{align*}
$$
{:.math}

Finalmente, dado que hemos demostrado que \\(\forall x\in \mathbb{R}:\forall A\in I:x\in A\implies\forall A\in I: x+1\in A\\), entonces podemos utilizar esta proposición como premisa, junto a la definición del conjunto \\(\mathbb{N}\\):

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\iff \forall A\in I:x\in A\\
\forall x\in \mathbb{R}:&&\forall A\in I:x\in A&\implies\forall A\in I: x+1\in A\\
\forall x\in \mathbb{R}:&&\forall A\in I:x+1\in A&\iff x+1\in \mathbb{N}\\
\hline
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\implies x+1\in \mathbb{N}
\end{align*}
$$
{:.math}

Todo lo anterior demuestra que \\(\mathbb{N}\\) es un conjunto inductivo.

Nota: *Dado que \\(\mathbb{N}\\) es inductivo, tenemos que \\(n\in\mathbb{N}\implies n+1\in\mathbb{N}\\). Por lo tanto, si en algún momento se tiene que la proposición \\(n\in\mathbb{N}\\) es verdadera, entonces la proposición \\(n+1\in\mathbb{N}\\) es verdadera. Es decir:*

$$
\begin{align*}
n\in\mathbb{N}&\\
n\in\mathbb{N}&\implies n+1\in\mathbb{N}\\
\hline
n+1\in\mathbb{N}
\end{align*}
$$
{:.math}

#### Demostración 2

En el siguiente razonamiento, la primera premisa es la definición del conjunto de los números naturales, la segunda premisa indica que si el la expresión del cuantificador es verdadera, entonces lo es para cualquier elemento.

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\iff \forall A\in I:x\in A\\
\forall x\in \mathbb{R}:&&(\forall A\in I:x\in A)&\implies x\in A\\
\hline
\forall x\in \mathbb{R}:&&x\in\mathbb{N}&\implies x\in A
\end{align*}
$$
{:.math}

Dado que \\(\forall x\in \mathbb{R}: \\: x\in\mathbb{N}\implies x\in A\\) \\(\equiv \mathbb{N}\subseteq A\\), concluimos la demostración.



### Corolario&nbsp;<span class="deg-sitio deg-sitio-texto">4</span>

\\(\forall n\in \mathbb{N}: n\ge1\\).

#### Demostración

Sea \\(A=\\{x\in \mathbb{R}\|x\ge 1\\}\\).

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in &\iff x\ge1 \\
1\ge 1\\
\hline
1\in A&&
\end{align*}
$$
{:.math}

Además:

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in A&\iff x\ge 1 \\
\forall x\in \mathbb{R}:&&x\ge 1&\implies x\ge 1 \land 1>0\\
\forall x\in \mathbb{R}:&&x\ge 1\land 1>0&\implies x>0\\
\forall x\in \mathbb{R}:&&x>0&\implies x+1>0+1\\
\forall x\in \mathbb{R}:&&x+1>0+1&\implies x+1>1\\
\forall x\in \mathbb{R}:&&x+1>1&\implies x+1 \in A\\
\hline
\forall x\in \mathbb{R}:&&x\in A&\implies x+1\in A
\end{align*}
$$
{:.math}

Es decir, \\(A\\) es inductivo, por lo que \\(\mathbb{N}\subseteq A\\).

Finalmente:

$$
\begin{align*}
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\implies x\in A \\
\forall x\in \mathbb{R}:&&x\in A&\implies x\ge1\\
\hline
\forall x\in \mathbb{R}:&&x\in \mathbb{N}&\implies x\ge 1
\end{align*}
$$
{:.math}