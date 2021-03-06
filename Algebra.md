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

This is an important sort of abstract subgroup, the *cyclic subgroup* generated by an arbitrary element $x \in G$. It is the smallest subgroup of $G$ contains $x$, which is $\{\cdots, x^{-2}, x^{-1}, 1, x, x^{2}, \cdots\}$. 

If we have $x^{k} = 1$, then we call the generated group $\langle x\rangle = \{1, x, \cdots, x^{k-1}\}$ *cyclic group of order $k$*

If there is no such $k$, we call this subgroup infinite order. 

And we call a subgroup of group $G$ generated by a subset $U$, if it is the smallest subgroup of $G$ that contains $U$ and all elements that can be generated by multiplying a list of elements of $U$ and their inverse.

And also we can find a subset $U$ that generate the group $G$ then we will say $U$ generates group $G$.

We can see that the permutation group $S_{3}$ is generated by ${}$ $\{x,y\}$.

Here are two other examples in the book, can check there.

---

### Homomorphism

**Homomorphism** is a structure-keeping map between two groups. 

##### Definition

A homomorphism is $\varphi : G \rightarrow G'$ such that for every $a,b \in G$ we have $\varphi(ab) = \varphi(a)\varphi(b)$.

This definition means that this map keep the composition law of the two groups in some sense. 

Then here are two important sets are defined they are image of $\varphi$ and kernel of $\varphi$.

image of homomorphism is just the same definition as the image of map.

kernel of a homomorphism $\varphi : G \rightarrow G'$ is a subset of $G$, whose image is $1 \in G'$. So the kernel of homomorphism has some properties. Here we need a definition called coset to describe the properties.

**coset** : $aH = \{g \in G|g = ah\ for\ some\ h\in H \}$ is called a *left coset* of $H$ in $G$. 

Then we can write the property like the following: 

For a homomorphism $\varphi: G \rightarrow G'$ the following things are equivalent:

1. $\varphi (a) = \varphi (b)$ 
2. $a^{-1}b$ is in $K$
3. $b$ is in the coset $aK$
4. the coset $aK$ and $bK$ is equal.

So it is obvious that the homomorphism is injective iff the kernel is trivial $\{1\}$.

**normal subgroup** : a subgroup $N$ is a normal subgroup of $G$ if for every $a\in N$ and every $g \in G$, $g a {g^{-1}} \in N$. And it is obvious kernel of homomorphism is a normal subgroup of group $G$.

*center* of a group is the set of elements that commute with all elements in $G$, that is $Z = \{z \in G|\forall x \in G, zx = xz\}$.

Then we want to discuss some kinds of homomorphism. The first one is isomorphism.

### isomorphism

isomorphism is a bijective map between two groups and keep the law of composition. **Then it is obvious that the inverse of isomorphism is also isomorphism.** 

When we talk about the *classifying groups*, we are talking about the isomorphic class of groups. It is very hard for us to classify all of groups. However, we can find a fact that when the order of the groups are prime number then these groups are cyclic. So prime number $p$ order groups are in one isomorphic class. 

Here is a strange point, when a isomorphism points the group $G$ to itself, then it is called **automorphism**. It is obvious the identity function is an automorphism, however there is another function which is called conjugate is also an automorphism.

A *conjugate* is defined by an element $g \in G$, for an element $a \in G$, its conjugation is $gag^{-1}$. This is a isomorphism to itself, because it has an inverse which is conjugation of $g^{-1}$. When the group is abelian, conjugation is the same as identity, well, they are not the same for non-commutative groups. 

The pair of elements $a,b$ in a group $G$ is commute iff $aba^{-1}b^{-1} = 1$.

### equivalence relations and partitions

a *partition* $\Pi$ of a set $S$ is a subdivision of $S$ into non-overlapping, non-empty subsets. And $S =$ union of disjoint subsets. 

An equivalence relation on a set $S$ is a relation between a pair of elements $a,b$. This kind of relation should satisfy the following 3 properties: 

1. transitive: $a \sim b$ and $b \sim c$, then $a \sim c$.
2. symmetric: $a \sim b$ then $b \sim a$.
3. reflexive: $\forall a, a \sim a$.

And we can find the congruent of triangular and the conjugacy are the equivalence relations.

Here is a important fact: An equivalence relations on a set $S$ determines a partition on the set $S$, and conversely. This can be proved by carefully checking the properties of partitions, all the elements are equivalent to $a$ contained in a subset $C_{a}$. These subsets constructs a partition of $S$. 

Here we can build a set $\bar{S}$ whose elements are the subsets built by the equivalence relations. 

##### The equivalence relations defined by a map

Any map $f: S \rightarrow T$ gives an equivalence relation on its domain, which is $a \sim b \iff f(a) = f(b)$. 

* The *inverse image* of the element $t$ of $T$, we should find that if the $f$ is not a bijective then there should be several elements in $S$. So $f^{-1}$ is not a map, so the inverse image of the function $f$ is called *fibres* of the map $f$.
* Then we can go back to see the partition defined by a map. So an inverse images of an element also construct an equivalence relation. So the fibres of an homomorphism are a partition of the original group. 

### Cosets

Here is an subgroup $H$ of group $G$. A left coset is 
$$
aH = \{ah| h \in H\}
$$
The cosets of $H$ in $G$ are equivalence classes for congruence relations 
$$
b \equiv a \text{  if  }b = ah\text{  for some }h \in H
$$
This relation is an equivalence relation, we can prove this by verifying the three properties of equivalence relation, which are transitivity, symmetry and reflexivity.

So here we know the left coset of a subgroup $H$ of group $G$ partition the group.

Let $H$ be a subgroup of a group $G$, and $a,b$ are elements of the same group $G$. Then the followings are equivalent:

* $b = ah$ for some $h \in H$, or, $a^{-1} b$ is an element of $H$.
* $b$ is an element of the left coset $aH$.
* the left cosets  $aH$ and $bH$ are equal.

The number of left cosets of subgroup $H$ is called the index of $H$ in $G$. We use $[G:H]$ to denote the the index.

**Theorem** All left cosets $aH$ of a subgroup $H$ of a group $G$ has the same order.

So we can get the *Counting Formula*: $|G| = |H| [G:H]$.

**Lagrange's Theorem** Let $H$ be a subgroup of a finite group $G$, the order of $H$ divides the order of $G$.

**Corollary** The order of an element of a finite group divides the order of the group.

**Corollary** Let $\varphi : G \rightarrow G'$ be a homomorphism of finite group, then we have

1. $|G| = |\text{ker } \varphi|\cdot |\text{im }\varphi|$
2. $|\text{ker } \varphi|$ divides $|G|$ and
3. $|\text{im }\varphi|$ divides both $|G|$ and $|G'|$.

##### right coset

Then we will consider right coset. Here we find normal subgroup is a useful concept. If $H​$ is a normal subgroup then the left coset and right coset of it will be the same.

### Modular Arithmetic 

We can find that the congruent under modular relation is an equivalence relation, which means it has all of the properties of equivalence relations.  

### Correspondence theorem

