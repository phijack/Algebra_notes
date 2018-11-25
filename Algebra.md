# Algebra

## chapter 2 Groups

### Basic definitions

**Group** : group is a set of elements with a law of composition and they should satisfy the following properties:

- the law of composition should be associative

- $G$ has an identity element $1$ , such that $1a = a1 =a$ for all $a \in G$ 
- every element $a \in G$ has an inverse that is $b \in G$, such that $ab = 1$

*abelian group* : is a group whose law of composition is commutative.

---

property of composition law :

<details><summary>associative</summary> a(bc) = (ab)c, in Chinese is called 结合律.</details>

<details><summary>commutative</summary>ab = ba, in Chinese is called 交换律.</details>

---

**Cancellation law**
For $a,b,c \in G$, if we have $ab = ac$ or $ba = ca$, then we have $b = c$; And if we have $ab =a$ or $ba =a$, then we have $b = 1$.

**subgroup** is a subset $H$ of group $G$ which has the same composition law as $G$ and satisfy the following three properties:

- *Closure* : if $a, b \in H$, $ab \in H$.
- *Identity* : $1 \in H$
- *Inverses* : if $a \in H$, then $a^{-1} \in H$.

---

### Some examples of subgroup

We will see some subgroups of $\mathbb{Z}^{+}$, which is all the integers under the addition operation group. 

##### 1. $\mathbb{Z}a$

$$
\mathbb{Z}a = \{ n \in \mathbb{Z} \vert n = ka\ for\ some\ k \in \mathbb{Z}\}
$$

This is the set of all integers which are divisible by $a$. And notice that for all non-trivial subgroup of $\mathbb{Z}^{+}$, we have a non-zero $a$ such that this subgroup is equal to $\mathbb{Z}a$.

##### 2. $\mathbb{Z}a + \mathbb{Z}b$

$$
\mathbb{Z}a +\mathbb{Z}b = \{n \in \mathbb{Z} \vert n = sa +tb \ for\ some\ s,t \in \mathbb{Z}\}
$$

If we let $d = \gcd (a,b)$, then $\mathbb{Z}a + \mathbb{Z}b = \mathbb{Z}d$.

##### 3. $\mathbb{Z}a  \cap \mathbb{Z}b$

If we let $m =  lcm (a,b)$, then $\mathbb{Z}m = \mathbb{Z}a \cap \mathbb{Z}b$.

---

### Cyclic Groups

