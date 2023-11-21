---
layout: default
tema: Rosa
tema_oscuro: RosaOscuro
title: Ejemplos
description: "Ejemplos"
last_modified_date: 2020-08-17T09:00:00+0000
parent: Inducción Matemática
nav_order: 1
---

# Ejemplos
{:.fs-9}

¡A demostrar infinitas proposiciones!
{:.fs-6 .fw-300}

---

El principio de inducción matemática ahora puede utilizarse para demostrar infinitas propiedades relacionadas, cada una, a un número natural.

Para ello veamos un ejemplo

<div class="marco-16-9 no-imprimir"><iframe  class="adaptable" src="https://www.youtube.com/embed/5HuMMTTfAGs?si=VXoy9EC2BYKQwJR7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>
<div class="no-mostrar">Escanea el siguiente código QR para ver el video <div id="VideoInduccionEdu" style="width: 5cm; height: 5cm;"></div></div>

## Demostraciones <span class="deg-sitio deg-sitio-texto">paso a paso </span>

En esta sección, te mostraremos una serie de demostraciones sencillas que utilizan el <span class="deg-sitio deg-sitio-texto">Principio de inducción matemática</span>.

### Ejemplo&nbsp;<span class="deg-sitio deg-sitio-texto">1 </span>

Para todo \\(n\in\mathbb{N}\\), se cumple que

$$\sum_{j=1}^n j=\frac{n(n+1)}{2}$$
{:.math }

<div class="salto"></div>

#### Demostración

<div class="marco-16-9 no-imprimir">
    <iframe class="adaptable" src="{{'/00-Archivos/Suma1-n.html'| relative_url}}">
    </iframe>
</div>

Para cada \\(n\in\mathbb{N}\\), sea \\(p(n)\\) el enunciado abierto dado por 
{:.no-mostrar}

$$p(n)\iff \displaystyle\sum_{k=1}^n k=\frac{n(n+1)}{2}$$
{:.math .no-mostrar}

Como
{: .no-mostrar}

$$\displaystyle\sum_{j=1}^1 j=1\land 1=\frac{1(1+1)}{2}$$
{:.math .no-mostrar}

\\(p(1)\\) es verdadero. Sea \\(k\in\mathbb{N}\\). Si \\(p(k)\\) es verdadero, entonces 
{: .no-mostrar}

$$\sum_{j=1}^k j=\frac{k(k+1)}{2}$$
{:.math .no-mostrar}

Luego
{: .no-mostrar}

$$
\begin{align*}
\sum_{j=1}^{k+1} j&=(k+1)+\sum_{j=1}^k j\\
&=(k+1)+\frac{k(k+1)}{2}\\
&=\frac{k(k+1)+2(k+1)}{2}\\
&=\frac{(k+1)(k+2)}{2}
\end{align*}
$$
{:.math .no-mostrar}

Por lo tanto, \\(p(k+1)\\) es verdadero. Finalmente, por el **Principio de Inducción matemática**,
{:.no-mostrar}

$$\forall n\in\mathbb{N}:\sum_{k=1}^n k=\frac{n(n+1)}{2}$$
{:.math .no-mostrar}

### Ejemplo&nbsp;<span class="deg-sitio deg-sitio-texto">2 </span>

Todo número natural diferente de 1 se puede escribir como la suma de 1 más algún número natural.

#### Demostración

<div class="marco-16-9 no-imprimir">
    <iframe class="adaptable" src="{{'/00-Archivos/1-o-Sucesor.html'| relative_url}}">
    </iframe>
</div>

Sea \\(A=\\{n\in\mathbb{N}\|n=1\lor \exists m\in\mathbb{N}:1+m=n\\}\\).
{:.no-mostrar}

$$
\begin{align*}
(n=1\lor \exists m\in\mathbb{N}:1+m=n)&\iff n\in A\\
\hline
1\in A
\end{align*}
$$
{:.math .no-mostrar}

Lo anterior indica que \\(1\in A\\).
{:.no-mostrar}

Ahora supóngase que \\(n\in A\\). Entonces \\(\exists m\in\mathbb{N}:1+m=n\\). Dado que \\(m,n\in\mathbb{N}\\), \\(m+1,n+1\in \mathbb{N}\\).
{:.no-mostrar}

$$
\begin{align*}
\forall n\in\mathbb{R}:&&n\in A&\iff (\exists m\in\mathbb{N}:1+m=n)\lor 1=n&\\
\forall n\in\mathbb{R}:&&&\iff (\exists m\in\mathbb{N}:1+m+1=n+1)\lor 1+1=n+1\\
\forall n\in\mathbb{R}:&&&\iff (\exists m\in\mathbb{N}:1+(m+1)=n+1)\lor 1+1=n+1\\
\forall n\in\mathbb{R}:&&&\implies n+1\in A\\
\hline
\forall n\in\mathbb{R}:&&n\in A&\implies n+1\in A
\end{align*}
$$
{:.math .no-mostrar}

Por tanto, \\(A\\) es inductivo. Por el **Principio de Inducción Matemática**, \\(A=\mathbb{N}\\)
{:.no-mostrar}

<script type="text/javascript">
new QRCode(document.getElementById("VideoInduccionEdu"), "https://www.youtube.com/watch?v=5HuMMTTfAGs");
</script>