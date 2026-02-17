Throughout this lecture $\Omega$ is a non-empty set

$\underline{\text{Defn:}}$ (semialgebra) $S \subseteq \mathcal{P}(\Omega)$ is called semialgebra if

(i) $\Omega \in S$

(ii) If $A \in S, B \in S \Rightarrow A \cap B \in S$

(iii) If $E \in S$, then $\exists A_1, \dots, A_k \in S$

s.t. $E^c = \bigcup_{j=1}^k E_j$

Example: $\Omega = \mathbb{R}$,

$S = \{ [a, b] : a \in \mathbb{R}, b \in \mathbb{R} \} \cup \{ [c, \infty) : c \in \mathbb{R} \} \cup \{ (-\infty, d) : d \in \mathbb{R} \}$

$\cup \{ \mathbb{R}, \phi \}$

$[a, b]^c = (-\infty, a) \cup (b, \infty)$

$\underline{\text{Defn:}}$ (algebra) $A \subseteq \mathcal{P}(\Omega)$ is called an algebra if

1. $\Omega \in A$
    
2. $A, B \in A \Rightarrow A \cup B \in A$
    
3. $A \in A \Rightarrow A^c \in A$
    

Remark: (i) an algebra is a semialgebra. $(A \cap B)^c = A^c \cup B^c$

(ii) a cycle is closed under intersection.

$(a, b) = \bigcup_{n=1}^\infty (a, b - \frac{1}{n}]$

$\underline{\text{Defn:}}$ ($\sigma$-algebra): $F \subseteq \mathcal{P}(\Omega)$ is called an $\sigma$-algebra if

(i) $\Omega \in F$

(ii) $A \in F \Rightarrow A^c \in F$

(iii) If $A_1, A_2 \in F \Rightarrow \bigcup_{j=1}^\infty A_j \in F$

---

Denote by $\mathscr{I}$ the collection of all intervals in $\mathbb{R}$

Then $\lambda: \mathscr{I} \to [0, \infty]$

Question: Does there exist function $M: \mathcal{P}(\mathbb{R}) \to [0, \infty]$ s.t.

$\uparrow$

Power set of $\mathbb{R}$

i) $M(I) = \lambda(I)$, $\forall I \in \mathscr{I}$

ii) $M(A+x) = M(A)$, $\forall x \in \mathbb{R}, \forall A \subseteq \mathbb{R}$

where $A+x = \{ a+x : a \in A \}$

iii) If $A = \bigcup_{j=1}^\infty A_j$, $A_j \cap A_k = \phi$ for $j \neq k$ then

$M(\bigcup_{j=1}^\infty A_j) = \sum_{j=1}^\infty M(A_j)$

Consequence: (i) $M(\phi) = 0$

(ii) If $E \subseteq F$ then $M(E) \subseteq M(F)$

$F = E \cup F - E \Rightarrow M(F) = M(E) + M(F - E) \Rightarrow M(E) \leq M(F)$

Side note: $x \in \mathbb{R}, A \subseteq \mathbb{R}$

$A+x = \{ a+x : a \in A \}$

$2 + (0, 1) = (2, 3)$

$\int_{a+x}^{b+x} f = \int_a^b f$ (per-mod-vity)

---

Question: Does there exists a map $\mu: \mathcal{P}(\mathbb{R}) \to [0, \infty]$, such that

1. $\mu(I) = \lambda(I) = \text{length of } I$
    
2. $\mu(A+x) = \mu(A)$, $\forall x \in \mathbb{R}, A+x := \{ a+x : a \in \mathbb{R} \}$
    
3. $A_j \subseteq \mathbb{R}$, $A_j \cap A_k = \phi, j \neq k$, then $\mu(\bigcup_{j=1}^\infty A_j) = \sum_{j=1}^\infty \mu(A_j)$
    

Ans: NO

<u>VITALI'S CONSTRUCTION</u>

On $\mathbb{R}$, we define an equivalence relationship $x \sim y \in$

Let $A = \{$

---

Exercise: $A$ is uncountable

Axiom of choice: Every indexed family $\{ S_i \}_{i \in I}$ of non-empty sets

there exists an unindexed set $\{ x_i : i \in I \}$ s.t.

$x_i \in$ ____________________

Given $\alpha \in \Lambda$, there exists $x_\alpha \in (0, 1]$ (By axiom of choice)

$y \in \alpha \subseteq \mathbb{R}$

$z \in (y - \lfloor y \rfloor) \in \mathbb{Q} \Rightarrow y \sim z \Rightarrow z \in \alpha$

$x \sim y \Rightarrow x - y \in \mathbb{Q}$

Define $E = \{ x_\alpha : \alpha \in \Lambda \}$

$(E + p) \cap (E + q) = \phi$ if $p, q \in \mathbb{Q}, p \neq q$

suppose $z \in (E + p) \cap (E + q)$

Then $z = x_\alpha + p = x_\beta + q$ for some $x_\alpha, x_\beta \in E$

---

(ii) $\bigcup_{p \in \mathbb{Q} \cap (-1, 1)} (E + p) \subseteq (-1, 2]$

$x_\alpha - x_\beta = q - p \in \mathbb{Q} \Rightarrow x_\alpha \sim x_\beta \Rightarrow \alpha = \beta \Rightarrow x_\alpha = x_\beta$

$\Rightarrow p = q$, a contradiction

(iii) $(0, 1] \subseteq \bigcup_{p \in (-1, 1) \cap \mathbb{Q}} (E + p)$

Take $x \in (0, 1]$. Then $x \in \alpha$ for some $\alpha$ That is,

$x \sim x_\alpha \Rightarrow x - x_\alpha \in \mathbb{Q}$.

If $q = x - x_\alpha \in (-1, 1) \Rightarrow x = x_\alpha + q$ with $q \in (-1, 1)$

Now $\mu(\bigcup_{p \in \mathbb{Q} \cap (-1, 1)} (E + p)) \leq \mu((-1, 2])$

$\Rightarrow \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu(E + q) \leq 3$

$\Rightarrow \sum_{p \in \mathbb{Q} \cap (-1, 1)} \mu(E) \leq 3 \Rightarrow \mu(E) = 0$

For any $n \in \mathbb{N}, (0, 1 - \frac{1}{n}] \subseteq \bigcup_{p \in (-1, 1) \cap \mathbb{Q}} \mu(E + p)$

$\Rightarrow \mu((0, 1 - \frac{1}{n}]) \leq \mu(\bigcup) = \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu(E + q)$

$p \in \mathbb{Q} \cap (-1, 1) \Rightarrow \mu(E) = 0$

$\Rightarrow 1 - \frac{1}{n} \leq \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu(E + q)$

$\Rightarrow 1 \leq \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu(E) \Rightarrow 1 \leq 0$

---

Then $f_k$ is riemann integrable with $\int_0^1 f_k(x)dx = 0$

$f_k \to f$ pointwise

$\to P = \{ a = x_0, x_1, \dots, x_n = b \}$

$U(P, f) = \sum_{i=1}^n M_i (x_i - x_{i-1})$

$\left[ \text{For a set } A \subseteq \mathbb{R} \text{, we define } \chi_A \text{ called the characteristic function of } A \text{ by} \right.$

$\chi_A(x) = \begin{cases} 1 & , x \in A \\ 0 & , x \notin A \end{cases}$

$\int_a^b \chi_{[a,b]}(x)dx = b - a$

$[c, d] \subseteq [a, b]$, $\int_a^b \chi_{[c,d]}(x)dx = \int_c^d dx = d - c$ $\left. \right]$

$\Rightarrow \sum_{i=1}^n M_i \int_a^b \chi_{[x_{i-1}, x_i]}(x)dx$

$\Rightarrow \int_a^b \sum_{i=1}^n M_i \chi_{[x_{i-1}, x_i]}(x)dx = \int_a^b S_P(x)dx$.

, [x1, x2], [x2, b]]

$S_P(x) = \sum_{i=1}^n M_i \chi_{[x_{i-1}, x_i]}$

$S_P(x) = \begin{cases} M_1 & , x \in [x_0, x_1) \\ M_2 & , x \in [x_1, x_2) \\ \vdots & \\ M_n & , x \in [x_{n-1}, x_n] \end{cases}$

Denote by $\lambda$ the length we already know that is, for $a, b \in \mathbb{R}$

$\lambda([a,b]) = \lambda([a,b)) = \lambda((a,b)) = \lambda((a,b]) = b - a$

$\lambda([a, \infty)) = \lambda((a, \infty)) = \lambda((-\infty, b]) = \lambda((-\infty, b)) = \infty$
_____
____
Denote by $\mathscr{I}$ the collection of all intervals in $\mathbb{R}$

Then $\lambda : \mathscr{I} \to [0, \infty]$

Question: Does there exist function $M : \mathcal{P}(\mathbb{R}) \to [0, \infty]$ s.t.

$\uparrow$

Power set of $\mathbb{R}$

i) $M(I) = \lambda(I) \text{ , } \forall I \in \mathscr{I}$

ii) $M(A + x) = M(A) \text{ , } \forall x \in \mathbb{R}, \forall A \subseteq \mathbb{R}$

where $A + x = \{a + x : a \in A\}$

iii) If $A = \bigcup_{j=1}^{\infty} A_j \text{ , } A_j \cap A_k = \phi$ for $j \neq k$ then

$$M\left(\bigcup_{j=1}^{\infty} A_j\right) = \sum_{j=1}^{\infty} M(A_j)$$

[Side Note:

$x \in \mathbb{R}, A \subseteq \mathbb{R}$

$A + x = \{ a + x : a \in A \}$

$2 + (0, 1) = (2, 3)$

$\int_{a+x}^{b+x} f = \int_{a}^{b} f$ (per-mod-vity)

]

Consequence: (i) $M(\phi) = 0$

(ii) If $E \subseteq F$ then $M(E) \subseteq M(F)$

$F = E \cup F \setminus E \Rightarrow M(F) = M(E) + M(F - E) \Rightarrow M(E) \subseteq M(F)$

---

Then $f_k$ is riemann integrable with $\int_{0}^{1} f_k(x)dx = 0$

$f_k \to f$ pointwise

$\rightarrow P = \{ a = x_0, x_1, \dots, x_n = b \}$

$U(P, f) = \sum_{i=1}^{n} M_i (x_i - x_{i-1})$

$\left[ \text{For a set } A \subseteq \mathbb{R} \text{, we define } \chi_A \text{ called the characteristic function of } A \text{ by} \right.$

$$\chi_A(x) = \begin{cases} 1 & , x \in A \\ 0 & , x \notin A \end{cases}$$

$\int_{a}^{b} \chi_{[a,b]}(x)dx = b - a$

$[c, d] \subseteq [a, b] \text{ , } \int_{a}^{b} \chi_{[c,d]}(x)dx = \int_{c}^{d} dx = d - c$ $\left. \right]$

$\Rightarrow \sum_{i=1}^{n} M_i \int_{a}^{b} \chi_{[x_{i-1}, x_i]}(x)dx$

$\Rightarrow \int_{a}^{b} \sum_{i=1}^{n} M_i \chi_{[x_{i-1}, x_i]}(x)dx = \int_{a}^{b} S_P(x)dx$.

, [x1, x2], [x2, b]]

$$S_P(x) = \sum_{i=1}^{n} M_i \chi_{[x_{i-1}, x_i]}$$

$$S_P(x) = \begin{cases} M_1 & , x \in [x_0, x_1) \\ M_2 & , x \in [x_1, x_2) \\ \vdots \\ M_n & , x \in [x_{n-1}, x_n] \end{cases}$$

Denote by $\lambda$ the length we already know that is, for $a, b \in \mathbb{R}$

$\lambda([a,b]) = \lambda([a,b)) = \lambda((a,b)) = \lambda((a,b]) = b - a$

$\lambda([a, \infty)) = \lambda((a, \infty)) = \lambda((-\infty, b]) = \lambda((-\infty, b)) = \infty$

---

(ii) $\bigcup_{p \in \mathbb{Q} \cap (-1, 1)} (E + p) \subseteq (-1, 2]$

$x_\alpha - x_\beta = q - p \in \mathbb{Q} \Rightarrow x_\alpha \sim x_\beta \Rightarrow \alpha = \beta \Rightarrow x_\alpha = x_\beta$

$\Rightarrow p = q \text{ , a contradiction}$

(iii) $(0, 1] \subseteq \bigcup_{p \in (-1, 1) \cap \mathbb{Q}} (E + p)$

Take $x \in (0, 1]$. Then $x \in \alpha$ for some $\alpha$ That is,

$x \sim x_\alpha \Rightarrow x - x_\alpha \in \mathbb{Q}$.

If $y = x - x_\alpha \in (-1, 1) \Rightarrow x = x_\alpha + q$ with $q \in (-1, 1)$

Now. $\mu \left( \bigcup_{p \in \mathbb{Q} \cap (-1, 1)} (E + p) \right) \leq \mu ((-1, 2])$

$\Rightarrow \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu (E + q) \leq 3$

$\Rightarrow \sum_{p \in \mathbb{Q} \cap (-1, 1)} \mu (E) \leq 3 \Rightarrow \mu (E) = 0$

For any $n \in \mathbb{N} \text{, } (0, 1 - \frac{1}{n}] \subseteq \bigcup_{p \in (-1, 1) \cap \mathbb{Q}} (E + p)$

$\Rightarrow \mu ((0, 1 - \frac{1}{n}]) \leq \mu (\bigcup) = \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu (E + q)$

$p \in \mathbb{Q} \cap (-1, 1) \Rightarrow \mu (E) = 0$

$\Rightarrow 1 - \frac{1}{n} \leq \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu (E + q)$

$\Rightarrow 1 \leq \sum_{q \in \mathbb{Q} \cap (-1, 1)} \mu (E) \Rightarrow 1 \leq 0$

---

Question: Does there exists a map $\mu : \mathcal{P}(\mathbb{R}) \to [0, \infty]$, such that

1. $\mu(I) = \lambda(I) = \text{length of } I$
    
2. $\mu(A + x) = \mu(A) \text{ , } \forall x \in \mathbb{R}, A + x := \{ a + x : a \in \mathbb{R} \}$
    
3. $A_j \subseteq \mathbb{R} \text{ , } A_j \cap A_k = \phi, j \neq k \text{, then } \mu \left( \bigcup_{j=1}^{\infty} A_j \right) = \sum_{j=1}^{\infty} \mu(A_j)$
    

Ans: NO

<u>VITALI'S CONSTRUCTION</u>

On $\mathbb{R}$, we define an equivalence relationship $x \sim y \in$

Let $A = \{ \text{ \textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore } \}$

Exercise: $A$ is uncountable

Axiom of choice: Every indexed family $\{ S_i \}_{i \in I}$ of non-empty sets there exists an unindexed set $\{ x_i : i \in I \}$ s.t.

$x_i \in \text{ \textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore\textunderscore }$

Given $\alpha \in \Lambda \text{ , there exists } x_\alpha \in (0, 1] \text{ (By axiom of choice)}$

$y \in \alpha \subseteq \mathbb{R}$

$z \in (y - \lfloor y \rfloor) \in \mathbb{Q} \Rightarrow y \sim 2 \Rightarrow z \in \alpha$

$x \sim y \Rightarrow x - y \in \mathbb{Q}$

Define $E = \{ x_\alpha : \alpha \in \Lambda \}$

$(E + p) \cap (E + q) = \phi$ if $p, q \in \mathbb{Q} \text{ , } p \neq q$

suppose $z \in (E + p) \cap (E + q)$

Then $z = x_\alpha + p = x_\beta + q \text{ for some } x_\alpha, x_\beta \in E$

---

Throughout this lecture $\Omega$ is a non-empty set

$\underline{\text{Defn:}}$ (semialgebra) $S \subseteq \mathcal{P}(\Omega)$ is called semialgebra if

(i) $\Omega \in S$

(ii) If $A \in S, B \in S \Rightarrow A \cap B \in S$

(iii) If $E \in S$, then $\exists A_1, \dots, A_k \in S$

s.t. $E^c = \bigcup_{j=1}^{k} E_j$

Example: $\Omega = \mathbb{R}$,

$S = \{ [a, b] : a \in \mathbb{R}, b \in \mathbb{R} \} \cup \{ [c, \infty) : c \in \mathbb{R} \} \cup \{ (-\infty, d) : d \in \mathbb{R} \} \cup \{ \mathbb{R}, \phi \}$

$[a, b]^c = (-\infty, a) \cup (b, \infty)$

$\underline{\text{Defn:}}$ (algebra) $A \subseteq \mathcal{P}(\Omega)$ is called an algebra if

1. $\Omega \in A$
    
2. $A, B \in A \Rightarrow A \cup B \in A$
    
3. $A \in A \Rightarrow A^c \in A$
    

Remark: (i) an algebra is a semialgebra. $(A \cap B)^c = A^c \cup B^c$

(ii) a cycle is closed under intersection.

$(a, b) = \bigcup_{n=1}^{\infty} (a, b - \frac{1}{n}]$

$\underline{\text{Defn:}}$ ($\sigma$-algebra): $F \subseteq \mathcal{P}(\Omega)$ is called an $\sigma$-algebra if

(i) $\Omega \in F$

(ii) $A \in F \Rightarrow A^c \in F$

(iii) If $A_1, A_2 \in F \Rightarrow \bigcup_{j=1}^{\infty} A_j \in F$

---

Exercise:

i) If $\{ A_\alpha \}_{\alpha \in I}$ is a family of algebras then

$\bigcap_{\alpha \in I} A_\alpha$ is also an algebra.

(ii) If $\{ F_\alpha \}_{\alpha \in I}$ [unclear] $\sigma$-algebras

$\underline{\text{Defn:}}$ i) If $\mathcal{C} \subseteq \mathcal{P}(\Omega)$ then $A(\mathcal{C}) := \bigcap_{\substack{A \text{ Algebra} \\ \mathcal{C} \subseteq A}} A$

is called the algebra generated by $\mathcal{C}$

ii) $F(\mathcal{C}) = \bigcap_{\substack{F - \sigma\text{-algebra} \\ \mathcal{C} \in F}} F$

Ex: Let $\Omega$ be uncountable Consider

$F = \{ A \subseteq \Omega : A \text{ or } A^c \text{ is countable } \}$

Then $F$ is a $\sigma$-algebra.

<u>Borel $\sigma$-Algebra</u>: Let $\Omega$ be a topological space. Then the $\sigma$-algebra generated by open set in $\Omega$ is called the Borel $\sigma$-algebra on $\Omega$.