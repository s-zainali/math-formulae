## Question 1: Direct Proof
Prove the following using a **Direct Proof**.

**Theorem:** For any real number, if $(6n+4)/(8n+5)$ is rational, then $n$ is rational.  
_Hint: $6/8\neq (6n+4)/(8n+5)$_
### Proof
Let $n$ be an unspecified real number.
Assume $(6n+4)/(8n+5)\in \mathbb{Q}$ .
Then $(6n+4)/(8n+5) = p/q$ for some $p\in \mathbb{Z}$ and some $q\in \mathbb{Z}$ where $q\neq 0$ by definition of rational number.
$6n+4=p\cdot c$ for some $c\in\mathbb{R}$
$8n+5=q\cdot c$
$\implies 6n=p\cdot c-4\implies n = (p\cdot c-4)/6=(p\cdot c+(-4))/6$
Since $p\cdot c$ is an integer and $-4$ is an integer, $p\cdot c+(-4)=a$ for some $a\in \mathbb{Z}$
So, $n=a/6$
Thus, $n\in \mathbb{Q}$ since $a$ is an integer and $6$ is an integer by definition of rational number.
Hence, $\forall n\in \mathbb{R},((6n+4)/(8n+5))\in\mathbb{Q}\rightarrow n\in\mathbb{Q}$
QED
## Question 2: Indirect Proof
Prove the following using a **Contradiction Proof**.

**Theorem:** For any real number, $x$ and $y\neq 3$, if $(2x^2+6x+2)/(y-3)$ is irrational, then either $x$ or $y$ is irrational.  
### Proof
We will prove by contradiction.
Consider $x$ to be an unspecified real number.
Consider $y$ to be an unspecified real number where $y\neq 3$.
Assume $(2x^2+6x+2)/(y-3)$ is irrational.
Assume $x\in\mathbb{Q}\implies x=p/q$ for some $p\in\mathbb{Z}$ and $q\in\mathbb{Z}\land q\neq 0$
Assume $y\in\mathbb{Q}\implies y=r/s$ for some $r\in\mathbb{Z}$ and $s\in\mathbb{Z}\land q\neq 0$
Thus, $(2x^2+6x+2)/(y-3)=((2(p/q))^2+6(p/q)+2)/(r/s)-3$
$=((2p/q)^2+6(p/q)+2)/(r/s)-3$
$=((2p/q)^2+(6p/q)+2)/(r/s)-3$
$=((2p/q)^2+(6p/q)+2)/(r/s)-(3s/s)$
$=(((2p)^2/q^2)+(6p/q)+2)/(r/s)-(3s/s)$
$=((4p^2/q^2)+(6p/q)+2)/(r/s)-(3s/s)$
$=((4p^2/q^2)+(6p/q)+2)/(r-3s/s)$
$= ((4p^2/q^2)+(6p/q)+2)/(r-3s/s)$
$= ((4p^2/q^2)+((6p)^2/q^2)+2)/(r-3s/s)$
$= ((4p^2/q^2)+((6p)^2/q^2)+2q^2/q^2)/(r-3s/s)$
$= ((4p^2/q^2)+(36p^2/q^2)+2q^2/q^2)/(r-3s/s)$
$= ((4p^2+36p^2+2q^2)/q^2)/(r-3s/s)$
$= ((4p^2+36p^2+2q^2)/q^2)/(r+(-3s)/s)$

Since the sum and product of integers is an integer, and $p\in\mathbb{Z}$ , and $q\in\mathbb{Z}$, and, and $r\in\mathbb{Z}$ $s\in\mathbb{Z}$
	$\exists a\in\mathbb{Z}, a=(4p^2+36p^2+2q^2)$
	$\exists b\in\mathbb{Z}, b= q\cdot q=q^2$
	$\exists c\in\mathbb{Z}, c = r+(-3)$ 

$\implies ((4p^2+36p^2+2q^2)/q^2)/(r+(-3s)/s) = (a/b)/(c/d)$
$=(a/b)\cdot (d/c)$
$=ad/bc$

Since the product of integers is an integer, $\exists e\in\mathbb{Z}, e = ad$
Since the product of integers is an integer, $\exists f\in\mathbb{Z}, f = bc$

$\implies ad/bc = e/f$
$\implies (2x^2+6x+2)/(y-3)=(e/f) \in\mathbb{Z}$ by definition of rational numbers

We had assumed $(2x^2+6x+2)/(y-3)$ is irrational.
Thus, we have a contradiction.
Hence, For any real number, $x$ and $y\neq 3$, if $(2x^2+6x+2)/(y-3)$ is irrational, then either $x$ or $y$ is irrational.  
QED
## Question 3: Induction Proof
Prove the following using a **Weak Induction Proof**.

**Theorem:** For any positive integer $x$, $(6^x+4)|5$.
### Proof
#### Base:
Let $x=1\implies 6^1+4=10$, $10|5$ since $5\cdot 2=10$.
#### Induction Hypothesis
Assume $\left(6^{(x-1)}+4\right)|5$.
#### Induction Step
Consider an unspecified positive integer $x$.
$\left(6^{(x-1)}+4\right)|5 \implies 6^{(x-1)}+4=5n$ where $n$ is some integer. **By IH**
$\implies 6\left(6^{x-1}+4\right)= 6\cdot 5n$
$\implies 6^x+24=30n$
$\implies 6^x+4=30n-20$
$\implies 6^x+4=5\cdot 6n-5\cdot4$
$\implies 6^x+4=5(6n-4)$
$\implies 6^x+4=5(6n+(-4))$
$6n$ is an integer since the product of integers is an integer
$-4$ is an integer
Since the sum of integers is an integer, $6n+(-4)$ is an integer $m$.
Thus, $6^x+4=5m$ where $m$ is an integer.
$\therefore (6^x+4)|5$
Hence, for any positive integer $x$, $6^x+4$ is divisible by 5.
QED
## Question 4
Prove the following using a **Strong Induction Proof**.

**Theorem:** Consider the following sequence, for integers $x$ and $n\geq 0$:  
$x_0=-2$  
$x_1=-14$  
$x_n=6\cdot x_{n-1}-8\cdot x_{n-2}$  
Prove that $x_n=3\cdot 2^n-5\cdot 4^n$
### Proof
#### Base:
#### Inductive Hypothesis:
#### Inductive Step:
## Question 5