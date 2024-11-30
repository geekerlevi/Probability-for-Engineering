# EE503 Probability for Electrical and Computer Engineers

![USC Viterbi School of Engineering](https://viterbischool.usc.edu/wp-content/uploads/2021/04/USC-Viterbi-School-of-Engineering.png)

## Week 1 Session 1

### <u>Outcome space / Sample space</u>

$$\Omega=\{set\:of\:all\:possible\:outcomes\:of\:a\:random\:experiment\}$$

1. Flip 1 coin:

​	$$\Omega=\{H,T\}$$

2. Flip 2 coins:

​	$$\Omega=\{HH,TT,HT,TH\}$$

3. Number of emails in the inbox from 10:30 am to 12:30 pm:

​	$$\Omega=\{0,1,2,3,...\}$$

4. Amplitude of the received signal at the radar:

​	$$\Omega=\{0,\infty\}$$

------

### <u>**Events:**</u>

Flip 2 coins:

$$\Omega=\{HH,TT,HT,TH\}$$

$$A=\{HH,TT\}$$

Event $$A$$: a subset of $$\Omega$$

If the observed outcome belongs to event $$A$$, then event A has occured.

Radar:

$$\Omega=\{0,\infty\}$$

$$A=\{0,1\}$$

$$B=\{\pi\}$$

------

### <u>Event Space: Collection of events.</u>

1. Flip 1 coin:

   $$\Omega=\{H,T\}$$

Event Space: $$\{H\}$$, $$\{T\}$$, $$\Omega$$, $$\phi$$ [All possible subsets of $$\Omega$$ ]

Power set of $$\Omega$$:  $$2^{\Omega}$$ 

2. Flip 2 coins:

   $$\Omega=\{HH,TT,HT,TH\}$$

Event space 1: $$\phi$$, $$\Omega$$, $$\{HH\}$$, $$\{HT\}$$, $$\{TH\}$$, $$\{TT\}$$, $$\{HH, TT\}$$, $$\{HT, TH\}$$, $$\{HH,HT\}$$, $$\{HT, TT\}$$ ... 

[Power set of $$\Omega$$ ]

==For a set with $$n$$ elements, number of possible subsets is $$2^{n}$$.== 

Event Space 2: $$\Omega=\{HH,TT,HT,TH\}$$

$\{HH, TT\}$, $$\{HT, TH\}$$, $$\Omega$$, $$\phi$$ $$\leftarrow$$ Another possible event space for the experiment of flipping

------

### Requirement of an <u>Event Space</u>

1. $$\Omega$$ is in the event space (sure event)
2. If $$A$$ is in the event space, $$A^c$$ is in the event space
3. If $$A$$ and $$B$$ are in the event space, then $$A \bigcup B$$ and $$A \bigcap B$$ are also in the event space. 

<u>Deduction 1:</u>

$$\phi$$ is always in event space

<u>Deduction 2:</u>

If $$A_1, A_2, ... A_n$$ in the event space, then:

$$ \bigcap_{i=1}^{n} A_i$$ and $$ \bigcup_{i=1}^{n} A_i$$ are in the event space.

------

### Probability Law $$P$$

For each event A in the event space, $$P(A)$$ is a real number that describes our belief/ likelihood of event $$A$$. 

<u>Axioms of Probability</u>

1. $$P(\Omega)=1$$

2. For any event $$A$$, $$0\le P(A)\le1$$

3. Additivity Axiom

   (a) If $$A$$ and $$B$$ are 2 disjoint ( i.e., mutually exclusive $$\leftarrow A \bigcap B = \phi$$) events, then:

   $$P(A \bigcup B)=P(A)+P(B)$$

   (b) If $$A_1, A_2, ... A_n$$ are pairwise disjoint events (i.e., $$A_k \bigcap A_l= \phi$$ for all $$k \neq l$$), then:

   $$P(A_1 \bigcup A_2 ... \bigcup A_n)=\sum_{i=1}^{n}P(A_i)$$

------

### $\textcolor{Blue}{Example\:1}$

$$\Omega=\{H,T\}$$

Event space=Power set of $$\Omega$$

$$P(\{H\})=1/2$$

What is the value of $$P({T})$$

$\textcolor{RedViolet}{{P(\Omega)}=1}$

$\textcolor{RedViolet}{{P(\{H,T\})}=1}$

$\textcolor{RedViolet}{ { \{H,T\}= \{H\} \bigcup \{T\} } }$

$\textcolor{RedViolet}{{P(\{H\} \bigcup \{T\})}=1}$ $\leftarrow$ Additivity axiom

$\textcolor{RedViolet}{{P(\{H\}) + P(\{T\})}=1}$

$\textcolor{RedViolet}{{P(\{T\})}=1-P(\{H\})}$

$\textcolor{RedViolet}{{P(\{T\})}=1-1/2=1/2}$

------

### $\textcolor{Blue}{Example\:2}$

Throw a die

$$\Omega=\{1,2,3,4,5,6\}$$

Event space=Power set of $$\Omega$$

Probability law: For any event $$A$$, $$P(A)=\frac{|A|}{6}$$

$\textcolor{Red}{Notation: |A|= number \: of \: elements \: in \: A=cardinality\: of\: A }$

$\textcolor{RedViolet}{{P(\{6\})}=1/6}$

$\textcolor{RedViolet}{Prob\:of\:getting\:an\:even\:number:}$

$\textcolor{RedViolet}{{P(\{2,4,6\})}=3/6}$

$\textcolor{RedViolet}{{P(\phi)}=0}$

------

### $\textcolor{Blue}{Example\:3}$

Throw a die

$$\Omega=\{1,2,3,4,5,6\}$$

Event space=Power set of $$\Omega$$

$$P(\{1\})=P(\{2\})=P(\{3\})=P(\{4\})=P(\{5\})=2/15$$

$\textcolor{RedViolet}{{P(\{6\})}=1/3}$

$\textcolor{RedViolet}{{P(\{3,4,5\})}={P(\{3\} \bigcup \{4\} \bigcup \{5\})}}$

$$\textcolor{RedViolet}{=P(\{3\})+P(\{4\})+P(\{5\})}$$

$$\textcolor{RedViolet}{=6/15}$$

------

### $\textcolor{Blue}{Example\:4}$

$$\Omega=\{0,\infty\}$$

Event space consist of all possible sub-interval of $$\{0,\infty\}$$ as well as their compliments, unions and intersections.

e.g., $$(a,b)$$, $$[a,b]$$, $$(a,b]$$, $$[a, \infty)$$

$\textcolor{Blue}{Borel\:event\:space\:or\:Borel\:sigma\:algebra}$

Probability law: For any interval $$A$$

$$P(A)=\int_{A} e^{-\omega}d\omega$$

$$P((1,2))=\int_{1}^{2}e^{-\omega}d\omega$$

$$P([2,\infty))=\int_{2}^{\infty}e^{-\omega}d\omega$$

<u>Probability that the outcome is less than 1 or greater than 5 ?</u>

$$\textcolor{RedViolet}{P([0,1])\bigcup(5,\infty))=P([0,1])+P((5,\infty))}$$

$$\textcolor{RedViolet}{=\int_{0}^{1}e^{-\omega}d\omega+\int_{5}^{\infty}e^{-\omega}d\omega}$$

------

### $\textcolor{Blue}{Example\:5}$

$$\Omega=\{1,2,3,4,...\}$$

$$\mathcal{F}=Power\:set\:of\:\Omega$$ 

i.e., Event space $$\mathcal{F}$$ [sigma-algebra]

$$P(\{k\})=\frac{1}{2^k}$$, where $$k=1,2,3,...$$

Verify $$P(\Omega)=1$$

------

### <u>Event space</u>

If $$A_1, A_2, ..., A_n$$ are in the event space, then:

$$ \bigcap_{i=1}^{n} A_i$$ and $$ \bigcup_{i=1}^{n} A_i$$ are in the event space.

If $$A_1, A_2, A_3, ...$$ are in the event space, then:

$$ \bigcap_{i=1}^{\infty} A_i$$ and $$ \bigcup_{i=1}^{\infty} A_i$$ are also in the event space.

------

### <u>Probability Axioms</u>

- Additivity axiom

  $$A_1, A_2, ..., A_n$$ are pairwise disjoint events

  $$P(\bigcup_{i=1}^{n}A_i)=\sum_{i=1}^{n}P(A_i)$$

- Countable additivity axiom

  $$A_1, A_2, A_3, ...$$ are pairwise disjoint events

  $$P(\bigcup_{i=1}^{\infty}A_i)=\sum_{i=1}^{\infty}P(A_i)$$

------

$P(\Omega)=P(\{1,2,3,4...\})$

$$\{1,2,3, ... \}=\{1\} \bigcup \{2\} \bigcup ...$$

$$\textcolor{RedViolet}{P(\{1\} \bigcup \{2\} \bigcup ...)=P(\{1\})+P(\{2\})+...}$$

Countable additivity axiom: $$P(\{k\})=\frac{1}{2^k}$$

$$\textcolor{RedViolet}{=\frac{1}{2}+\frac{1}{2^2}+...}$$

$$\textcolor{RedViolet}{=\frac{1/2}{1-1/2}}$$

Note $$\leftarrow$$ Geometric series

$$a+ar+ar^2+...$$ where $$r<1$$, then 

$$ sum=\frac{a}{1-r}$$

Probability that the outcome is an even number:

$\textcolor{RedViolet}{P(\{2,4,6,8...\})=P(\{2\} \bigcup \{4\} \bigcup ...)}$

$$\textcolor{RedViolet}{=P(\{2\})+P(\{4\})+...}$$

$$\textcolor{RedViolet}{=\frac{1}{2^2}+\frac{1}{2^4}+...}$$

$$\textcolor{RedViolet}{=\frac{1/4}{1-1/4}}$$

$$\textcolor{RedViolet}{=1/3}$$

------

### $\textcolor{Blue}{Example\:6}$

$$\Omega=\{(x,y): 0\leq x, y \leq 1\}$$

![image-20240908134908031](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240908134908031.png)

$$P(A)=Area \: of \: A$$

$$P(\Omega)=Area \: of \: \Omega = 1$$

$$P(A)=1/2$$



$$B$$ is the event that the sum of $$x$$ and $$y$$ coordinate is less than or equal to $$1/2$$

$$B={(x,y) \in \Omega: x+y \leq 1/2}$$

$$P(B)=Area \: of \in B=1/2 \times 1/2 \times 1/2 =1/8$$

## Week 1 Session 2

### Random Experiment & Probability Model

- Outcome space / Sample Space $$\Omega$$

- An event is a subset of $$\Omega$$

- If the realized outcome of experiment lies in $$A$$, we say event $$A$$ has occurred.

  ![image-20240909094046291](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909094046291.png)

  Event Space / Sigma algebra $$\mathcal{F}$$

  Properties of $$\mathcal{F}$$: 

  1. $$\Omega$$ is in $$\mathcal{F}$$

  2. If $$A$$ is in $$\mathcal{F}$$, then $$A^c$$ is in $$\mathcal{F}$$

  3. (a) If $$A_1, A_2, ... A_n$$ are in $$\mathcal{F}$$, then:

     $$\bigcup_{i=1}^{n}A_i$$ is in $$\mathcal{F}$$ and $$\bigcap_{i=1}^{n}A_i$$ is in $$\mathcal{F}$$

     (b) If $$A_1, A_2, A_3, ...$$ is an infinite sequence of events that are in $$\mathcal{F}$$, then: 

     $$\bigcup_{i=1}^{\infty}A_i$$ is in $$\mathcal{F}$$ and $$\bigcap_{i=1}^{\infty}A_i$$ is in $$\mathcal{F}$$

------

### Probability Law

For each event $$A$$ in $$\mathcal{F}$$, $$P(A)$$ is a real number. 

### Probability Axioms

1. $$P(\Omega)=1$$

2. $$0 \leq P(A) \leq 1$$

3. (a) If $$A_1, A_2, ... A_n$$ are pairwise disjoint events, then: 

   $$P(\bigcup_{i=1}^{n}A_i)=\sum_{i=1}^{n}P(A_i)$$

   (b) If $$A_1, A_2, A_3, ... $$ is an infinite sequence of pairwise disjoint events, then:

   $$P(\bigcup_{i=1}^{\infty}A_i)=\sum_{i=1}^{\infty}P(A_i)$$

------

### Deduction from Axioms

1. $$P(A)+P(A^c)=1$$

![image-20240909095058830](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909095058830.png)

Proof: 

$$\textcolor{RedViolet}{1=P(\Omega)}$$

$$\textcolor{RedViolet}{=P(A \bigcup A^c)}$$

$$\textcolor{RedViolet}{=P(A)+P(A^c)}$$

2. If $$ A \subset B$$, then $$P(A) \leq P(B)$$

<img src="C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909095220745.png" alt="image-20240909095220745" style="zoom:67%;" />

Proof:

$$\textcolor{RedViolet}{B=A \bigcup C}$$

$$\textcolor{RedViolet}{P(B)=P(A \bigcup C)}$$

$$\textcolor{RedViolet}{=P(A)+P(C)}$$

$$\textcolor{RedViolet}{\rightarrow}$$ $$\textcolor{RedViolet}{P(B) \geq P(A)}$$

$$\textcolor{RedViolet}{C=B \bigcap A^c}$$



3. Union Formula

   For any 2 events $$A$$ and $$B$$

   $$P(A \bigcup B)=P(A)+P(B)-P(A \bigcap B)$$

![image-20240909095631838](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909095631838.png)

$$\textcolor{Black}{A \bigcap B}$$

$$\textcolor{red}{A \bigcap B^c}$$

$$\textcolor{green}{B \bigcap A^c}$$

Proof: 

$$\textcolor{RedViolet}{P(A)=P(A \bigcap B^c)+P(A \bigcap B)}$$  $$\enclose{circle}{1}$$

$$\textcolor{RedViolet}{P(B)=P(B \bigcap A^c)+P(A \bigcap B)}$$  $$\enclose{circle}{2}$$

$$\textcolor{RedViolet}{P(A \bigcup B)= P(A \bigcap B^c)+P(A \bigcap B)+P(B \bigcap A^c)}$$

$$\textcolor{RedViolet}{=P(A)+P(B \bigcap A^c)}$$ $$\enclose{circle}{1} \: is \: applied$$

$$\textcolor{RedViolet}{=P(A)+P(B)-P(A \bigcap B)}$$  $$\enclose{circle}{2} \: is \: applied$$

4. $$P(\phi)=0$$

Proof:

$$\textcolor{RedViolet}{P(\phi)+P(\phi^{c})=1}$$

$$\textcolor{RedViolet}{P(\phi)+P(\Omega)=1}$$

$$\textcolor{RedViolet}{P(\phi)+1=1}$$

$$\textcolor{RedViolet}{P(\phi)=0}$$

------

Exercise 1.

$$A_1, A_2, A_3$$

$$P(A_1)=a_1$$ , $$P(A_2)=a_2$$ , $$P(A_3)=a_3$$

$$P(A_1 \bigcap A_2)=b_1$$ , $$P(A_2 \bigcap A_3)=b_2$$ , $$P(A_3 \bigcap A_1)=b_3$$

$$P(A_1 \bigcap A_2 \bigcap A_3)=c$$

<u>What is the value of $$P(A_1 \bigcup A_2 \bigcup A_3)$$ ?</u>

$$\textcolor{RedViolet}{B=A_2 \bigcup A2}$$

$$\textcolor{RedViolet}{P(A_1 \bigcup B)=P(A_1)+P(B)-P(A_1 \bigcap B)}$$

$$\textcolor{RedViolet}{=P(A_1)+P(A_2 \bigcup A_3)-P(A_1 \bigcap (A_2 \bigcap A_3))}$$

Exercise, show that:

$$A_1 \bigcap (A_2 \bigcup A_3)=(A_1 \bigcap A_2) \bigcup (A_1 \bigcap A_3)$$

------

### Union Bound

Theorem:

$$A_1, A_2, ... A_n$$ are $$n$$ events $$(n \geq 2)$$

$$P(\bigcup_{i=1}^{n}A_i) \leq \sum_{i=1}^{n}P(A_i)$$

Proof: Induction argument

$$n=2$$

$$P(A_1 \bigcup A_2)=P(A_1)+P(A_2)-P(A_1 \bigcap A_2) \leq P(A_1)+P(A_2)$$

Assume that the theorem is true for $$n=k$$

i.e., $$P(\bigcup_{i=1}^{k}A_i) \leq \sum_{i=1}^{k}P(A_i)$$

Then in the $$k+1$$ case, where

$$A_1, A_2, ... A_k, A_{k+1}$$

$$P(\bigcup_{i=1}^{k+1}A_i)=P((\bigcup_{i=1}^{k} \bigcup A_{k+1}) \leq P(\bigcup_{i=1}^{k}A_i+P(A_{k+1}))$$

$$P(\bigcup_{i=1}^{k+1}A_i)\leq \sum_{i=1}^{k}P(A_i)+P(A_{k+1})$$

$$P(\bigcup_{i=1}^{k+1}A_i)=\sum_{i=1}^{k+1}P(A_i)$$

------

### Cardinality of sets

#### Finite sets

$$\Omega=\{1,2,3,4,5,6\}$$

$$\Omega=\{a,b,c,... z\}$$

#### Infinite sets

##### Countably infinite sets

$$N=\{1,2,3, ...\}$$

A set $$A$$ that is "as large" as $$N$$ is called a countably infinite set.

![image-20240909122130247](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909122130247.png)

Formally, $$A$$ is countably infinite if we can find a function $$f$$ from $$A$$ to $$N$$, such that 

($$i$$) $$f$$ is a one-to-one function

i.e., if $$a \neq b$$, then $$f(a) \neq f(b)$$

($$ii$$) for every positive integer $$n$$, there is an $$a \subset A$$ such that $$f(a)=n$$



###### $$\textcolor{Blue}{Example 1}$$

$$A=\{0,1,2,3,...\}$$

$$N=\{1,2,3,...\}$$

![image-20240909122535975](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909122535975.png)

$$f(a)=a+1=n$$

$$a=n-1$$

Therefore, $$A$$ is countably infinite



###### $$\textcolor{Blue}{Example 2}$$

$$B=\{2,4,6,8,...\}$$

$$N=\{1,2,3,...\}$$

$$f(b)=b/2=n$$

$$b=2n$$



###### $$\textcolor{Blue}{Example 3}$$ 

$$C=\{2,4,8,16,32, ...\}$$

$$f(c)=\log_{2}{c}=n$$

$$c=2^n$$



###### $$\textcolor{Blue}{Example 4}$$

$$\{-1,-2,-3, ...\}$$

$$\{..., -1,0, 1,2, ...\}$$

are countably infinite sets

------

##### Uncountably infinite sets

Much larger sets of positive integers

e.g., $$[0,1]$$, $$[0, \infty]$$, $$(-\infty, \infty)$$

$$[0,1]$$

There is no way of finding a one-to-one association(correspondence) between $$[0,1]$$ and $$N$$

![image-20240909123909785](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909123909785.png)

------

### $$\textcolor{Blue}{Example 5}$$

![image-20240909125104936](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909125104936.png)

$$A_1 \subset A_2$$

$$P(A_1 \bigcup A_2)=P(A_2)$$



$$A_1 \subset A_2 \subset ... \subset A_k$$

$$P(\bigcup_{i=1}^{k}A_i)=P(A_k)$$



$$A_1 \subset A_2 \subset ... \subset A_k \subset A_{k+1}... $$

$$P(\bigcup_{i=1}^{\infty}A_i)=\lim_{k \rightarrow \infty}P(A_k)$$



![image-20240909125113221](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909125113221.png)

$$A_1 \supset A_2$$

$$P(A_1 \supset A_2)=P(A_2)$$

$$A_1 \supset A_2 \supset ... \supset A_k$$

$$P(\bigcap_{i=1}^{k}A_i)=P(A_k)$$



$$A_1 \supset A_2 \supset ... \supset A_k \supset A_{k+1}... $$

$$P(\bigcap_{i=1}^{\infty}A_i)=\lim_{k \rightarrow \infty}P(A_k)$$

------

### $$\textcolor{Blue}{Example 6}$$

$$\Omega =[0,1]$$

$$P(interval)=length \: of \: interval$$

$$A_1=[0,1]$$

$$A_2=[0,1/2]$$

$$A_3=[0,1/3]$$

$...$

$$A_k=[0,1/k]$$

$$A_1 \supset A_2 \supset A_3 \supset ...$$

$$P(A_1 \bigcap A_2 \bigcap A_3)=P(A_3)=1/3$$

$$P(\bigcap_{i=1}^{\infty}A_i)=\lim_{k \rightarrow \infty}P(A_k)=\lim_{k \rightarrow \infty}1/k=0$$

$$\bigcap_{i=1}^{\infty}A_i=\{0\}=[0,0]$$

$$P([0,0])=0$$

------

### Finite outcome space

$$\Omega=\{\omega_1, \omega_2, ..., \omega_n\}$$

$$\mathcal{F}= power \: set \: of \: \Omega$$

$$P({\omega_1})=p_1$$, $$P({\omega_2})=p_2$$, $$...$$ $$P({\omega_n})=p_n$$

$$P(\{\omega_1, \omega_2, \omega_3\})=P(\{\omega_1\} \bigcup \{\omega_2\} \bigcup \{\omega_3\} )$$

$$=P\{\omega_1\}+P\{\omega_2\}+P\{\omega_3\}$$

$$=p_1+p_2+p3$$

------

$$p_1+p_2+...+p_n=1$$

$$1=P(\Omega)=P(\{\omega_1, ..., \omega_n\})$$

------

Special case:

$$\Omega=\{\omega_1, ..., \omega_n\}$$

$$\mathcal{F}=Power \: set$$

$$P({\omega_i})=p$$  for $$i=1,2,... n$$ <u>Equally likely outcomes</u>

$$1=p+p+...+p$$

$$1=np$$

$$p=1/n$$

$$P(\{\omega_2, \omega_4, \omega_6\})=P(\{\omega_2\})+P(\{\omega_4\})+P(\{\omega_6\})$$

$$=3/n$$

$$A=\{\omega_{k1}, ..., \omega_{km}\}$$

$$P(A)=m/n$$

$$P(A)=\frac{|A|}{n}$$

If $$\Omega$$ is countably infinite,

$$\Omega=\{\omega_1, \omega_2, ...\}$$

we will usually work with power set on our event space

------

### $$\textcolor{Blue}{Example 6}$$

$$\Omega=[0,1]$$

Borel Sigma algebra: all sub-interval, union, intersections, compliments

$$P(sub-interval\:of\:[0,1])=length\:of\:sub-interval$$

$$0\leq a\leq b\leq 1$$

$$P([a,b])=b-a$$

$$A=\{\omega \in [0,1]: |\omega-0.5|\geq 0.1\}$$

![image-20240909183705942](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240909183705942.png)

$$P(A)=0.8$$

$$A=[0, 0.4] \bigcup [0.6,1]$$

$$P(A)=0.4+0.4=0.8$$



Exercise

$$B=\{\omega \in [0,1]: (\omega-1/2)^2 \geq 1/4\}$$

$$P(B)=?$$

------

$$P([0,1])=1$$

$$P([0,1])=P(\bigcup_{0 \leq \omega \leq 1} {\omega})$$

$$=\sum_{0 \leq \omega \leq 1}P({\omega})$$

$$\neq \sum_{0 \leq \omega \leq 1}P([\omega, \omega])$$

$$\neq 0$$

------

### Conditional Probability

Roll a fair die

$$\Omega=\{1,2,3,4,5,6\}$$

$$\mathcal{F}=Power \: set$$

Equally likely outcomes

$$P({k})=1/6$$, $$1 \leq k \leq 6$$

$$B=\{2,4,6\}$$

$$A=\{2\}$$

Given that $$B$$ has occurred, the new probability for event $$A=1/3$$

$$C=\{1,2,3\}$$

Given that $$B$$ has occurred, what is the revised probability for event C?

$$\textcolor{RedViolet}{1/3}$$

$$\textcolor{RedViolet}{New \: prob \: of \: A=\frac{|A \bigcap B|}{|B|}}$$

$$\textcolor{RedViolet}{New \: prob \: of \: C=\frac{|C \bigcap B|}{|B|}}$$



Definition:

If $$A$$ and $$B$$ are 2 events, and $$P(B)>0$$

$$P(A|B)=\frac{P(A \bigcap B)}{P(B)}$$

$$P(B|B)=1$$

$$P(B^c|B)=0$$

$$P(\Omega|B)=\frac{P(\Omega \bigcap B)}{P(B)}=\frac{P(B)}{P(B)}=1$$

------

## Week 2 Session 1

### Deductions from Axioms

1. $$P(A)+P(A^c)=1$$
2. $$P(A \bigcup B)=P(A)+P(B)-P(A \bigcap B)$$
3. If $$A \subset B$$ , then $$P(A) \leq P(B)$$

### Finite outcome space

$$\Omega=\{\omega_1, ... \omega_n\}$$

Typically, $$\mathcal{F}=$$ Power set of $$\omega$$

$$P(\{\omega_1)\})=p_1, ... , P(\{\omega_n\})=p_n$$ 

Special case: Finite $$\omega$$ with equally likely outcome

$$P(\{\omega_i\})=\frac{1}{n}$$ , $$n=|\Omega|$$

$$P(A)=\frac{|A|}{n}$$

------

### Conditional Probabilities 

Definition: If $$A$$ and $$B$$ are 2 events, and $$P(B) > 0$$

$$P(A|B)=\frac{P(A \bigcap B)}{P(B)}$$



#### Example

4 sided die, roll it twice

$$\Omega=\{(x,y):x,y\in\{1,2,3,4\}\}$$

$$=\{(1,1),(1,2),(1,3), ... (4,4,)\}$$



Equally likely outcome $$P(\{x,y\})=\frac{1}{16}$$

$$E=\{\text{Both number are less than 3}\}=\{(1,1),(1,2),(2,1),(2,2)\}$$ 

$$F=\{\text{Both numbers are 1}\}=\{(1,1)\}$$

$$P(F|E)=\frac{P(F \bigcap E)}{P(E)}$$

$$P(E)=\frac{4}{16}$$

$$P(F \bigcap E)=\frac{1}{16}$$

$$P(F|E)=\frac{1}{4}$$



$$P(E|F)=\frac{P(E \bigcap F)}{P(F)}$$

$$P(E|F)=\frac{1}{16} / \frac{1}{16}=1$$

------

$$B=\{\text{minimum of 2 number is 2}\}=\{(2,2), (2,3), (3,2), (2,4), (4,2)\}$$

$$A=\{\text{maximum of 2 number is 3}\}=\{(3,3), (3,1), (1,3), (2,3), (3,2)\}$$

$$P(A|B)=\frac{P(A \bigcap B)}{P(B))}=\frac{2/16}{5/16}=2/5$$

$$C=\{\text{maximum of 2 number is 1}\}$$

$$P(C|B)=\frac{P(C \bigcap B)}{P(B)}=\frac{P(\phi)}{P(B)}=0$$

------

Probability Axioms

1. $$P(\Omega)=1$$
2. $$0 \leq P(A) \leq 1$$
3. Additivity axiom

------

Fix event $$B$$ with $$P(B)>0$$. Consider conditional probability of various event given $$B$$. These new probability will satisfy probability axioms.

1. $$P(\Omega|B)=\frac{P(\Omega \bigcap B)}{P(B)}=\frac{P(B)}{P(B)}=1$$

2. $$0 \leq P(A|B) \leq 1$$

   $$0 \leq \frac{P(A \bigcap B)}{P(B)} \leq 1$$

3. If $$A_1$$ and $$A_2$$ are disjoint events

   $$P(A_1 \bigcup A_2 | B)= \frac{P((A_1 \bigcup A_2)\bigcap B)}{P(B)}$$

   $$=\frac{P((A_1\bigcap B)\bigcup(A_2 \bigcap B))}{P(B)}$$

   $$=\frac{P(A_1\bigcap B)+P(A_2 \bigcap B)}{P(B)}$$

   $$=P(A_1|B)+P(A_2|B)$$

------

### Deduction from Axioms

1. $$P(A|B)+P(A^c|B)=1$$
2. $$P(A \bigcup C | B)=P(A|B)+P(C|B)-P(A \bigcap C|B)$$
3. If $$A \subset C$$. then $$P(A|B) \leq P(C|B)$$

------

### Chain Rule / Multiplication Rule

If $$P(B)>0$$ , then $$P(A|B)=\frac{P(A\bigcap B)}{P(B)}$$

$$P(A \bigcap B)= P(A|B)P(B)$$  - Chain Rule

If $$P(A)>0$$ , then $$P(B|A)=\frac{P(B \bigcap A)}{P(A)}$$

$$P(B \bigcap A)=P(B|A)P(A)$$

------

$$P(B)>0 , P(B^c)>0$$

$$P(A|B)$$ , $$P(A|B^c)$$

$$P(A \bigcap B)=P(A|B)P(B)$$

$$P(A \bigcap B^c)=P(A|B^c)P(B^c)$$

<u>Law of total probability</u>

$$P(A)=P(A|B)P(B)+P(A|B^c)P(B^c)$$

------

### Partition

Partition of $$\Omega$$

$$B_1, ... , B_n$$ forms a partition of $$\Omega$$

if $$B_i \bigcap B_j = \phi$$ for $$i \neq j$$ (pairwise disjoint) and $$\bigcup_{i=1}^{n}B_i=\Omega$$ 

$$P(B_i)$$ for $$i=1,...,n$$

$$P(A|B_i)$$ for $$i=1, ... ,n$$

$$P(A)=P(A \bigcap \Omega)$$

$$=P(A \bigcap (\bigcup_{i=1}^{n}B_i))$$

$$=P((A\bigcap B_1) \bigcup ...(A \bigcap B_n))$$

$$=\sum_{i=1}^{n}P(A \bigcap B_i)$$

Law of total probability

$$P(A)=\sum_{i=1}^{n}P(A|B_i)P(B_i)$$



#### Example

Say a sender and receiver with transmission route 1 and 2

$$P(R1)=3/4, P(D|R1)=1/3, P(R2)=1/4, P(D|R2)=2/3$$ where $$D$$ is the packet get dropped



$$P(D)=P(D \bigcap R1) + P(D \bigcap R2)$$

$$=P(D|R1)P(R1)+P(D|R2)P(R2)$$

$$=1/3 \cdot 3/4 + 2/3 \cdot 1/4 =5/12$$



$$P(\text{Packet not getting dropped|R1})=P(D^c|R1)$$

$$=1-P(D|R1)$$

$$=2/3$$



$$P(R1|D)=\frac{P(R1 \bigcap D)}{P(D)}$$

$$=\frac{P(D|R1)P(R1)}{5/12}$$

------

### Bayes' Rule

$$P(A)>0, P(B)>0$$

$$P(B|A)=\frac{P(B \bigcap A)}{P(A)}=\frac{P(A|B)P(B)}{P(A)}$$ 



$$P(R1|D^c)=\frac{P(D^C|R1)P(R1)}{P(D^c)}$$

$$=\frac{(1-P(D|R1)) \cdot 3/4}{1-P(D)} \neq P(R1)$$

This it because $$P(R1|D^c)$$ is the posterior probability and $$P(R1)$$ is the prior probability. 

------

Law of total probability + Bayes' Rule

Partition of $$\Omega: B_1, ... B_n$$

$$B_i \bigcap B_j=\phi$$

$$\bigcup_{i=1}^{n}B_i=\Omega$$

Given $$P(B_i), P(A|B_i)$$

$$P(B_i|A)=\frac{P(A|B_i)P(B_i)}{P(A)}$$

Bayes' Rule: 

$$P(B_i|A)=\frac{P(A|B_i)P(B_i)}{\sum_{i=1}^{n}P(A|B_i)P(B_i)}$$



#### Example

Binary communication channel 

$$P(S0)=1-\alpha$$ , $$P(S1)=\alpha$$ 

$$P(R0|S0)=1-q$$ , $$P(R1|S0)=q$$

$$P(R0|S0)=p$$ , $$P(R1|S1)=1-p$$

$$P(R1)=P(R1 \bigcap S1)+P(R1 \bigcap S0)$$

$$=P(R1|S1)P(S1)+P(R1|S0)P(S0)$$

$$=(1-p)\alpha+q(1-\alpha)$$



$$P(S1|R1)=\frac{P(R1|S1)P(S1)}{P(R1)}$$

$$=\frac{(1-p)\alpha}{(1-p)\alpha+q(1-\alpha)}$$

------

### Chain Rule

$$P(A \bigcap B)=P(A|B)P(B)$$

$$P(A \bigcap B \bigcap C)=P(A|(B \bigcap C))P(B \bigcap C)$$

$$=P(A|(B \bigcap C))P(B|C)P(C)$$



$$P(A_1 \bigcap ...  \bigcap A_n)=P(A_1|A_2 \bigcap ... \bigcap A_n)P(A_2|A_3 ... \bigcap A_n)...P(A_{n-1}|A_n)P(A_n)$$



#### Example

Two urns

Urn 1: 5 red balls and 5 green balls

Urn 2: 2 red balls and 4 green balls

Randomly pick one ball from the selected urn and remove it 

Randomly pick $$2^{nd}$$ ball from the same urn



$$U1=\{\text{Urn 1 is selected}\}$$ , $$P(U1)=2/3$$

$$U2=\{\text{Urn 2 is selected}\}$$ , $$P(U2)=1/3$$ 

$$R1=\{\text{first ball is red}\}$$

$$R2=\{\text{second ball is red}\}$$



$$P(R1 \bigcap R2)= P(R1 \bigcap R2 \bigcap U1)+ P(R1 \bigcap R2 \bigcap U2)$$

$$P(R2 \bigcap R1 \bigcap U1)=P(R2|R1\bigcap U1)P(R1|U1)P(U1)$$

$$=4/9 \cdot 5/10 \cdot 2/3$$

$$P(R2 \bigcap R1 \bigcap U2)=P(R2|
R1 \bigcap U2)P(R1|U2)P(U2)$$

$$=1/5 \cdot 2/6 \cdot 1/3$$

$$P(U1|R1 \bigcap R2)=\frac{P(R1 \bigcap R2|U1)P(U1)}{P(R1 \bigcap R2)}$$

$$=\frac{4/9 \cdot 5/10 \cdot 2/3}{P(R1 \bigcap R2)}$$

------

## Week 2 Session 2

$$P(A|B)=\frac{P(A \bigcap B)}{P(B)}$$ if $$P(B)>0$$

<u>Chain Rule:</u>

$$P(A \bigcap B)=P(A|B)P(B)$$

$$P(A \bigcap B \bigcap C)=P(A|B \bigcap C)P(B|C)P(C)$$

<u>Law of total probability:</u>

If $$B_1, ... B_n$$ is a partition of $$\Omega$$
Then $$P(A)=\sum_{i=1}^{n}P(A \bigcap B_i)$$

$$=\sum_{i=1}^{n}P(A|B_i)P(B_i)$$



Can be extended to a countable partition, i.e., $$B_1, B_2, ...$$

that are pairwise disjoint and $$ \bigcup_{i=1}^{\infty}B_i=\Omega$$ 

Then, $$P(A)=\sum_{i=1}^{\infty}P(A\bigcap B_i)=\sum_{i=1}^{\infty}P(A|B_i)P(B_i)$$



Bayes' Rule

$$P(B|A)=\frac{P(A|B)P(B)}{P(A)}$$

------

$$P(A \bigcap B)=P(A|B)P(B)$$



Statement: $$P(A \bigcap B|C)=P(A|B\bigcap C)P(B|C)$$

LHS: $$P(A\bigcap B|C)=\frac{P(A \bigcap B \bigcap C)}{P(C)}$$

RHS: $$P(A|B \bigcap C)P(B|C)=\frac{P(A \bigcap B \bigcap C)}{P(B \bigcap C)} \frac{P(B \bigcap C)}{P(C)}$$

------

Two urns example 

$$P(R2 \bigcap R1|U1)P(U1)$$

$$=P(R2|R1 \bigcap U1)P(R1|U1)P(U1)$$

------

$$P(A \bigcap B) \sim \frac{\text{number of}(A \bigcap B)}{n}$$ relative frequency

$$P(B) \sim \frac{\text{number of} B}{n}$$

$$P(A|B) \sim \frac{\text{number of }(A \bigcap B)}{\text{number of }B}$$

------

### Independent Events

Definition: Two events $$A$$ and $$B$$ are independent if $$P(A \bigcap B)=P(A)P(B)$$

Let $$A$$ and $$B$$ be independent events and $$P(B)>0$$
$$P(A|B)=\frac{P(A \bigcap B)}{P(B)}=\frac{P(A)P(B)}{P(B)}=P(A)$$

$$P(B^c)>0$$

$$P(A|B^c)=\frac{P(A \bigcap B^c)}{P(B^c)}=\frac{P(A)-P(A \bigcap B)}{1-P(B)}=\frac{P(A)-P(A)P(B)}{1-P(B)}=P(A)$$

------

Independence $$\neq$$ Disjoint events

$$C \bigcap D = \phi$$ , $$P(C), P(D) >0$$

<u>Are $$C$$ and $$D$$ independent?</u> 

$$P(C \bigcap D)=P(\phi)=0$$ 

$$P(C)P(D)>0$$ 

$$P(C \bigcap D) \neq P(C)P(D)$$

$$C$$ and $$D$$ are not independent

$$P(C|D)=0$$

------

### Lemma 1 

If $$A$$ and $$B$$ are independent events, then so are the following events: 

(a) $$A$$ and $$B^c$$ 

$$P(A \bigcap B^c)=P(A)P(B^c)$$

(b) $$A^c$$ and $$B$$ are independent

(c) $$A^c$$ and $$B^c$$ are independent

Proof:

(a) $$P(A \bigcap B^c)= P(A)-P(A \bigcap B)$$

$$=P(A)-P(A)P(B)$$

$$=P(A)(1-P(B))$$

$$=P(A)P(B^c)$$

(b) $$A^c$$ and $$B$$

(c) $$A^c$$ and $$B^c$$

Using property: $$(A \bigcup B)^c=A^c \bigcap B^c$$

$$P(A^c \bigcap B^c)= 1 - P(A \bigcup B)$$

$$=1-P(A)-P(B)+P(A \bigcap B)$$

$$=1-P(A)-P(B)-P(A)P(B)$$

$$=(1-P(A))(1-P(B))$$

$$=P(A^c)P(B^c)$$



#### Example

4 sided die, $$\Omega=\{1,2,3,4\}$$

Equally likely outcomes

$$A=\{1,4\}$$ , $$B=\{2,4\}$$

$$P(A)=1/2 , P(B)=1/2$$

$$P(A \bigcap B)=1/4$$



#### Example

$$\Omega=\{1,2,3,4\}$$

$$P(\{1\})=P(\{2\})=P(\{3\})=p$$

$$A=\{1,4\}$$ , $$B=\{2,4\}$$

$$P(A)=1-2p$$

$$P(B)=1-2p$$

$$P(A \bigcap B)=P(\{4\})=1-3p$$

$$A$$ and $$B$$ are independent if $$1-3p=(1-2p)^2$$

------

### Independence of 3 events

Def: $$A,B,C$$ are independent (mutually independent) if

1. $$P(A\bigcap B \bigcap C)=P(A)P(B)P(C)$$
2. $$P(A \bigcap B)=P(A)P(B)$$
3. $$P(B \bigcap C)=P(B)P(C)$$
4. $$P(C\bigcap A)=P(C)P(A)$$

$$P(A\bigcap B|C)=\frac{P(A\bigcap B \bigcap C)}{P(C)}=\frac{P(A)P(B)P(C)}{P(C)}=P(A)P(B)=P(A \bigcap B)$$

$$P(A|C)=P(A)$$

$$P(A \bigcup B |C)=\frac{P((A \bigcup B)\bigcap C)}{P(C)}$$

$$=\frac{P((A\bigcap C)\bigcup (B \bigcap C))}{P(C)}$$

$$=\frac{P(A \bigcap C)+P(B \bigcap C)-P(A \bigcap B \bigcap C)}{P(C)}$$

$$=\frac{P(A)P(C)+P(B)P(C)-P(A)P(B)P(C)}{P(C)}$$

$$=P(A)+P(B)-P(A)P(B)$$

$$=P(A \bigcup B)$$

$$P(A \bigcup C)=P(A|C)+P(B|C)-P(A\bigcap B|C)$$

$$=P(A)+P(B)-P(A \bigcap B)$$

$$=P(A \bigcup B)$$

------

### Pairwise independence

$$A,B,C$$ are pairwise independent if

$$P(A\bigcap B)=P(A)P(B)$$

$$P(B \bigcap C)=P(B)P(C)$$
$$P(C \bigcap A)=P(C)P(A)$$

------

#### Example

4 sided die equally likely outcomes $$\Omega=\{1,2,3,4\}$$

$$A=\{1,4\}$$ , $$B=\{2,4\}$$ , $$C=\{3,4\}$$

$$P(A \bigcap B)=1/4$$ , $$P(A)=1/2$$ , $$P(B)=1/2$$

$$A,B,C$$ are pairwise independent

$$P(A \bigcap B \bigcap C)=1/4$$

$$P(A)P(B)P(C)=1/8$$ 

$$P(A \bigcap B \bigcap C) \neq P(A)P(B)P(C)$$ meaning $$A,B,C$$ are not independent

$$P(A\bigcap B|C)=\frac{P(A \bigcap B \bigcap C)}{P(C)}=\frac{1/4}{1/2}=1/2$$

------

### Lemma 2

$$A,B,C$$ are independent then

(a) $$A^c ,B, C$$ are independent

Proof:

$$P(A^c \bigcap B)=P(A^c)P(B)$$

$$P(A^c \bigcap C)=P(A^c)P(C)$$

$$P(B \bigcap C)=P(B)P(C)$$

$$P(A^c \bigcap B \bigcap C)=P(B \bigcap C)-P(B \bigcap C \bigcap A)$$

$$=P(B)P(C)-P(B)P(C)P(A)$$

$$=(1-P(A))P(B)P(C)$$

$$=P(A^c)P(B)P(C)$$

(b) $$A^c, B^c, C$$ are independent  

$$E=A^c$$

From Part (a) $$E, B, C$$ are independent

$$\implies$$ $$E,B^c,C$$ are independent

$$\implies$$ $$A^c, B^c, C$$ are independent

(c) $$A^c, B^c, C^c$$ are independent 

$$E=A^c, F=B^c$$

From Part (b) 

$$\implies$$ $$E,F,C$$ are independent

using Part (a)

$$\implies$$ $$E, F, C^c$$ are independent

$$\implies$$ $$A^c, B^c, C^c$$ are independent re

------

#### Example

3 bits are transmitted over a noisy channel

For each bit, the probability of correct reception is $$\lambda$$ 

$$P(C_i)=\lambda$$ , $$P(E_i)=1-\lambda$$

The error events for the 3 bits are mutually independent

$$E_i=\{\text{bit\:}i \text{\:incorrectly received}\}$$

$$E_1,E_2,E_3$$ are independent

$$C_i=\{\text{bit\:}i \text{\:correctly received}\}$$

$$C_1, C_2, C_3$$ are independent

$$C_1, C_2, E_3$$ are independent

------

#### Example

Find the probability that the number of correctly received bits is 2

$$S=\{\text{Number of correct bits is 2}\}$$

$$(C_1\bigcap C_2 \bigcap E_3)\bigcup(C_1 \bigcap E_2 \bigcap C_3)\bigcup(E_1 \bigcap C_2 \bigcap C_3)$$

say $$F_1=C_1\bigcap C_2 \bigcap E_3, F_2=C_1 \bigcap E_2 \bigcap C_3, F_3=E_1 \bigcap C_2 \bigcap C_3$$

$$S=F_1 \bigcup F_2 \bigcup F_3$$

$$P(S)=P(F_1)+P(F_2)+P(F_3)$$ 

because $$F_1, F_2, F_3$$ are pairwise disjoint

$$P(C_1 \bigcap C_2 \bigcap E_3)=\lambda \lambda (1-\lambda)$$

$$P(S)=3\lambda^{2}(1-\lambda)$$

Probability that all bits are correctly received:

$$=P(C_1 \bigcap C_2 \bigcap C_3)=\lambda^{3}$$

Probability that at least 2 bits are correctly received: 

$$=\lambda^{3}+3\lambda^{2}(1-\lambda)$$

------

Finite $$\Omega$$ and equally likely outcomes

$$P(\{\omega\})=\frac{1}{|\Omega|}$$ , $$|\Omega|$$ is the cardinality of $$\Omega$$

$$P(A)=\sum_{\omega \in A}P(\{\omega\})=\sum_{\omega \in A}\frac{1}{|\Omega|}=\frac{|A|}{|\Omega|}$$



#### Example

Antenna array consists of $$n$$ antennas

Arrange $$n$$ antennas in a straight line 

$$m$$ out of the $$n$$ antennas are defective

All arrangement of $$n$$ antennas are equally likely

The array will not work if 2 defective antennas are next to each other

Probability of the array that does not work?

$$n=4, m=2$$

$$A=\{DDNN,NNDD,NDDN,NDND,DNDN,DNND\}$$ 

$$P(\text{Array not work})=\frac{|A|}{|\Omega|}=\frac{3}{6}$$

$$n=12, m=4$$

Systematic / Efficient way of counting number of elements in a set without listing all elements $$\rightarrow$$ Combinatorics

------

### Basis principle of counting

![image-20240926021632508](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20240926021632508.png)

$$n_1 n_2$$ ways of doing this procedure

------

#### Example

4 digit passcode

$$10^4$$



#### Example

7 character license plate where first 3 characters are letter other 4 are digits

$$26 \cdot 26 \cdot 26 \cdot 10 \cdot 10 \cdot 10 \cdot 10$$

Repetition of letter or digits is not allowed

$$26 \cdot 25 \cdot 24 \cdot 10 \cdot 9 \cdot 8 \cdot 7$$

## Week 3 Session 1

### Independent events

Definition: Two events $$A$$ and $$B$$ are independent if $$P(A \bigcap B)=P(A)P(B)$$

Independence $$\implies P(A|B)=P(A|B^c)=P(A)$$

### Independence of 3 events

Def: $$A,B,C$$ are independent (mutually independent) if

1. $$P(A\bigcap B \bigcap C)=P(A)P(B)P(C)$$
2. $$P(A \bigcap B)=P(A)P(B)$$
3. $$P(B \bigcap C)=P(B)P(C)$$
4. $$P(C\bigcap A)=P(C)P(A)$$

### Independence of multiple events

Definition: $$A_1, ... A_n$$ are (mutually) independent if

$$P(\bigcap_{i \in I}A_i)=\prod_{i\in I}P(A_i)$$

for every non-empty $$I \subset \{1,2,...,n\}$$

------

Definition: $$A_1, A_2, ... $$ are (mutually) independent if

$$P(\bigcap_{i \in I}A_i)=\prod_{i\in I}P(A_i)$$

for every non-empty and finite $$I \subset \{1,2,...\}$$

------

Finite $$\Omega$$ and equally like outcomes

$$P(A)=\frac{|A|}{|\Omega|}$$

------

Basic principle of Counting

Total number of ways of doing 2-stage procedure is $$n_1n_2$$

------

### Permutations

Definition: Any arrangement of elements of $$S$$ in a sequence

$$S=\{I_1, ... I_n\}$$

How many permutation of $$S$$ are possible? 

Imagine have $$n$$ slots, 

$$n \cdot (n-1) ... \cdot 1=n!$$



#### Example

4 digit passcode using all of these digits 2,4,6,8

number of passcodes=number of permutations=$$4!$$

------

$$S=\{I_1, ... I_n\}$$

Sampling an ordered k-tuple with repetitions allowed

$$k=2$$ , $$(I_1 \: I_2) \neq (I_2 \: I_1)$$ , $$(I_1 \: I_1) \neq (I_1 \: I_1)$$

How many ordered pairs are possible? 

$$n^2$$

Ordered $$k$$-tuple

$$n^k$$ ordered $$k$$-tuple



#### Example

Flipping a coin $$k$$ times. How many sequence of $$H,T$$ are possible?

$$k$$-tuple: $$2^k$$

------

Sampling ordered $$k$$-tuple without repetitions $$1 \leq k \leq n$$ 

$$S=\{I_1, ... I_n\}$$

Within $$k$$ slots, then $$n \cdot (n-1) \cdot ... \cdot (n-k+1)$$

Number of ordered $$k$$-tuple without repitition

$$n \cdot (n-1) \cdot ... \cdot (n-k+1)=\frac{n!}{(n-k)!}$$

------

#### Example 

$$n$$ people in a department.

Need to form a committee consisting of a chair, a vice chair and a secretary

Same person cannot serve in more than 1 role

How many such committees are possible?

$$n(n-1)(n-2)=\frac{n!}{(n-3)!}$$



#### Example: Birthday problem

$$k$$ people , $$1\leq k\leq 365$$

All were born in non-leap year

a) How many birthday sequences are possible?

$$(d_1, ... d_k)$$ where every slot has 365 possibilities

$$365^k$$

b) How many birthday sequences are possible without repitition?

$$\frac{365!}{(365-k)!}=365 \cdot 364 \cdot ... \cdot (365-k+1)$$

c) Assume that all birthday sequence are equally likely? 

Probability that the group of $$k$$-people have distinct birthdays

$$\frac{|A|}{|\Omega|}=\frac{\frac{365!}{(365-k)!}}{365^k}$$

d) Probability that at least 2 people in this $$k$$-people group have the same birthday?

$$P(B)=1-P(\text{everyone has a different birthday})$$

$$=1-\frac{\frac{365!}{(365-k)!}}{365^k}$$

------

Selecting a subset with $$k$$ elements, $$1\leq k \leq n$$

- Order is not important
- No repetitions
- A subset of $$k$$ elements is called a "combination" with $$k$$-elements

Say $$S=\{I_1,I_2,I_3\}$$ has a subset of size 2

$$\{I1, I2\},\{I1, I3\},\{I3, I2\}$$ all 3 possibilities

------

With $$n$$ elements in $$S$$

number of $$k$$ element subsets $$n \mathrm{C}_k$$

$$n \mathrm{C}_k=\frac{n!}{(n-k)!k!}=\binom{n}{k}$$ where $$\frac{n!}{(n-k)!k!}$$ is the binomial coefficient

------

number of subset of 0 elements=1

$$k=0$$

$$\binom{n}{0}=\frac{n!}{n!0!}=1$$

------

for $$k \geq n+1$$

$$n \mathrm{C}_k=0$$

------

Why is the number of subsets of $$S$$ with $$k$$-elements=$$\binom{n}{k}$$ 

Task: Select an order $$k$$-tuple from $$S$$ without repititions

$$n(n-1)...(n-k+1)=\frac{n!}{(n-k)!k!}$$

Indirect method for task

Stage1: 

Pick a subset of $$k$$ elements (without considering order)

$$n \mathrm{C}_k$$

Stage2:

Pick a permutation for the $$k$$-element subset chosen in stage1

$$k!$$

$$n \mathrm{C}_k k!=\frac{n!}{(n-k)!}$$

$$n \mathrm{C}_k=\frac{n!}{(n-k)!k!}$$

------

#### Example

a) 20 people in an organization need a committee of 3 people

number of possible committees$$=\binom{20}{3}=\frac{20!}{3!17!}$$

b) 12 people - 5 women and 7 men

Need to form a committee with 2 women and 3 men

number of possible committees$$=\binom{5}{2}\binom{7}{3}$$

c) 7 people

Committee of 3 people 

Two of 7 people - Person 1 and Person 2 refuse to serve together

number of possible committees$$=\binom{7}{3}-\binom{5}{1}$$



Method 2: $$S={P_1, ... P_7}$$

Committees with $$P_1$$ but not $$P_2=\binom{5}{2}$$

Committees with $$P_2$$ but not $$P_1=\binom{5}{2}$$

Committees with neither $$P_1$$ or $$P_2=\binom{5}{3}$$

$$\binom{5}{2}+\binom{5}{2}+\binom{5}{3}=30$$

------

#### Example

50 items: 10 of items are defective, 40 are functional

Randomly pick 10 items

<u>Probability that exactly 5 of selected items are defective</u>

$$\frac{\binom{10}{5}\binom{40}{5}}{\binom{50}{10}}$$

------

#### Example

32 bit binary number. <u>How many such numbers have exactly 5 zeros</u>

$$\binom{32}{5}$$

------

A computer randomly generate a 32 bit binary number.

<u>Probability that the number generated has exactly 5 zeros.</u>

$$\frac{\binom{32}{5}}{2^{32}}$$

------

#### Example

$$n$$ antennas, $$m$$ defective , $$n-m$$ functional, $$1\leq m \leq n$$

$$n$$ antennas are arranged in a row

a) How many ways can I arrange $$m$$ defective (0) and $$(n-m)$$ functional (1) antennas?

say $$n=4,m=2$$ 

$$\binom{4}{2}=\frac{4!}{2!2!}=6$$

$$n$$ - bit binary number with $$m$$ 0 and $$n-m$$ 1

$$\binom{n}{m}$$

b) How many arrangement where no 2 defective antennas are adjacent to each other?

$$n$$ bits where no 2 zeros are adjacent

$$m$$ zeros and $$n-m$$ ones

say $$m=2$$ then $$n-2$$ ones simply

$$\binom{n-1}{2}$$



$$^{n-m+1} \mathrm{C}_m$$ number of valid arrangement

If $$m \leq n-m+1$$

$$^{n-m+1} \mathrm{C}_{m}=\binom{n-m+1}{m}$$

If $$m>n-m+1$$

$$^{n-m+1} \mathrm{C}_{m}=0$$

c) Antenna system works as long as no two defective antennas are next to each other

$$P(\text{Antenna system works})=\frac{^{n-m+1} \mathrm{C}_{m}}{\binom{n}{m}}$$

------

#### Example

$$S=(I_1, ... I_n)$$

Divide $$S$$ into groups: Group 1 with $$k_1$$ items, Group with $$k_2$$ items

where $$k_1+k_2=n$$ , $$1 \leq k_1 \leq n$$ , $$1 \leq k_2 \leq n$$

How many such division of $$S$$ are possible?

$$\binom{n}{k_1}\binom{n-k_1}{k_2}=\binom{n}{k_1}\binom{k_2}{k_2}=\binom{n}{k_1}$$

Problem:

Divide $$S$$ into $$r$$ groups 

Group 1: $$k_1$$ items

...

Group r: $$k_r$$ items

where $$k_1+...+k_r=n$$

How many such divisions are possible?

$$\binom{n}{k_1}\binom{n-k_1}{k_2}...\binom{n-k_1-k_2-...-k_{r-1}}{k_r}$$

$$=\frac{n!}{k_1!(n-k_1)!} \frac{(n-k_1)!}{k_2!(n-k_1-k_2)!}...$$

$$=\frac{n!}{k_1!k_2!...k_r!}$$ 

Multinomial coefficient

------

#### Example

6 sided die. Roll it 12 times.

How man sequence with 10 ones, 1 twos and 1 threes?

12 positions

Divide 12 positions into 3 groups

G1- 10

G2- 1

G3- 1

$$\frac{12!}{10!1!1!}$$

Exercise: How many outcomes where each number appears exactly twice

------

## Week 3 Session 2

### Combinatorial Problems

$$S={I_1, ... I_n}$$

1. Number of ordered $$k$$-tuple with repetitions allowed

   $$n^k$$

2. Number of ordered $$k$$-tuples without repetition $$1\leq k \leq n$$

   $$\frac{n!}{(n-k)!}$$ 

3. Number of possible subsets of size $$k$$ , $$1\leq k \leq n$$

   $$\binom{n}{k}$$ 

4. Partition $$S$$ into $$r$$ groups of sizes $$k_1, k_2, ... k_r$$ respectively $$(k_1+k_2+...+k_r=n)$$

   Number of possible partitions

   $$\frac{n!}{k_1!...k_r!}=\binom{n}{k_1, k_2, ... k_r}$$

------

Example: $$k$$ identical items ($$k$$ $1 bills)

Divide among two people

| $$P1$$  | $$P2$$  |
| ------- | ------- |
| 0       | $$k$$   |
| 1       | $$k-1$$ |
| 2       | $$k-2$$ |
| $$...$$ | $$...$$ |
| $$k-1$$ | 1       |
| $$k$$   | 0       |

Each outcome compounds to $$k+1$$ bit number with exactly one 0

Number of such number$$=\binom{k+1}{1}$$



Divide among 3 people 

Each outcome compounds to a $$k+2$$ bit number with exactly two 0

$$\binom{k+2}{2}$$



Divide $$k$$ identical item among $$n$$ people

$$\binom{n-1+k}{n-1}=$$ number of possible division of $$k$$ identical items among $$n$$ people 

$$\binom{n-1+k}{n-1}=\binom{n-1+k}{k}$$

------

#### Example

Consider the equation

$$x_1+x_2+...+x_n=k$$

Non-negative integer $$x_1, ... , x_n$$ that satisfy the equation above.

<u>How many such solutions are possible?</u>

$$\binom{n-1+k}{n-1}$$

------

#### Example

Unordered sampling with replacement

$$S=\{a,b,c\}$$

Sample this set $$k$$ times with repitition allowed

Outcome is triplet $$(x_a,x_b,x_c)$$

$$x_a+x_b+x_c=k$$ where $$x_a$$ is the number of times $$a$$ was picked, $$x_b$$ is the number of times $$b$$ was picked, $$x_c$$ is the number of times $$c$$ was picked

Number of possible outcomes$$=\binom{k+2}{2}$$



Ordered sampling with replacement

$$S=\{a,b,c\}$$

Sample this set $$k$$ times with repitition allowed

Outcome is the sequence of items selected

E.g., $$aabb...b$$ 



$$S=\{a,b,c\}$$

Sampling without repetition, 3 times

Number of ordered triplets$$=3\times 2 \times 1$$

Picking a subset of size 3

Number of subsets$$=\binom{3}{3}=1$$

 

$$S=\{a,b,c\}$$

Sampling with repetition, ordered $$k$$-tuple

Number of order $$k$$-tuple$$=3^k$$

Number of such tuples with 1$$a$$, 1$$b$$, $$k-2$$  $$c$$

$$\frac{k!}{1!1!(k-2)!}$$

------

#### Example

Roll a 6-sided die $$n$$ times

Outcome is the sequence of number obtained

Number of possible outcomes$$=6^n$$

Number of possible outcomes with $$k_1$$ ones, $$k_2$$ twos, ... $$k_6$$ sixes

$$\binom{n}{k_1, k_2, ... , k_6}$$

Number of possible outcomes with $$x$$ even numbers and $$n-x$$ odd numbers

------

Sequential experiment with independent sub-experiments

Toss a coin $$n$$ times $$(n=3)$$

$$\Omega=\{HHH,TTT,...\}$$

$$P(\{HTH\})=P(\{\text{Heads on 1st toss}\}\{\text{Tails on 2nd toss}\}\{\text{Heads on 3rd toss}\})$$

Assume Independence 

$$=P(\text{Heads on 1st toss})P(\text{Tails on 2nd toss})P(\text{Heads on 3rd toss})$$

$$=p(1-p)p$$

$$P(\text{Heads on\:}k^{th}\text{\: toss})=p$$

$$P(\text{Tails on\:}k^{th}\text{\: toss})=1-p$$

------

#### Example

Roll a 4-sided die 3 times.

Rolls are independent. The die is fair.

$$P((\text{Even number of 1st roll})\bigcap (\text{Even number of 2nd roll}) \bigcap (\text{4 on 3rd roll}))$$

$$=P((\text{Even number of 1st roll})P(\text{Even number of 2nd roll})P(\text{4 on 3rd roll})$$

$$=1/2 \cdot 1/2 \cdot 1/4$$

------

Suppose we have a sequential experiment with $$n$$ independent sub-experiments

This means that if we consider any $$n$$ events $$A_1, ..., A_n$$

where $$A_i$$ occurrence depends only on the outcomes of $$i$$th sub-experiments

Then, $$A_1,...,A_n$$ are independent

------

#### Example

Coin toss $$n$$ times

Each toss is $$H$$ with probability $$p$$ and $$T$$ with probability $$(1-p)$$

Coin tosses are independent

$$P(HHTT...T)=p \cdot p \cdot (1-p)...\cdot (1-p)$$

$$=p^2(1-p)^{n-2}$$

$$P(THHT...T)=p^2(1-p)^{n-2}$$

$$P(\text{a sqeunce of length\:}n \text{\:with\:} k \: H, (n-k) \:T)=p^k(1-p)^{n-k}$$

Probability that we get $$k$$ heads and $$n-k$$ tails

$$=\sum_{\text{sequence with\:}k \: H, (n-k) \:T)}P(\text{sequence})$$

 $$=\sum_{\text{sequence with\:}k \: H, (n-k) \:T)}p^k(1-p)^{n-k}$$

$$=\text{sequence with\: k \: H, (n-k) \:T} \:p^k(1-p)^{n-k}$$

$$=\binom{n}{k}\:p^k(1-p)^{n-k}$$



$$P(\{\text{Getting\:}k\text{\:heads in\:}n\text{independent coin tosses}\})=\binom{n}{k}\:p^k(1-p)^{n-k}$$

------

$$k=0,1,2, ... n$$

### Binomial probability law

#### Example

$$n$$ trials of a new drug

Each trial is a success with probability or a failure with probability $$1-p$$

Trials are independent

$$P(\{\text{Get exactly \:}k \text{\:success in\:}n\text{\:trials}\})=\binom{n}{k}\:p^k(1-p)^{n-k}$$



#### Example

100 bits are transmitted over a noisy channel. The transmission of each bit are independent.

Each bit is received correctly with probability $$\lambda$$ or incorrectly with probability $$1-\lambda$$

$$P(\{\text{Get \:}k \text{\:bits correctly})=\binom{100}{k}\lambda^k(1-\lambda)^{100-k}$$

------

#### Example

A coin is tossed infinitely many times. Coin tosses are independent

For each toss, $$H\rightarrow p, T\rightarrow 1-p$$ , $$0\leq p \leq 1$$

Probability that the first $$H$$ appears on the $$m^{th}$$ toss

| $$m=1$$ | $$p$$            |
| ------- | ---------------- |
| $$m=2$$ | $$(1-p)\cdot p$$ |

Probability that first $$H$$ on $$m^{th}$$ toss

$$=P(\{TT...TH\})=(1-p)^{m-1}p$$ where $$m=1,2,3,...$$



Exercise: Probability that it takes more than $$m$$ tosses to get the first $$H$$



$$P(\{\text{first\:}H\text{\:on\:}m+1\text{\:toss}\}\bigcup\{\text{first\:}H\text{\:on\:}m+2\text{\:toss}\}\bigcup\{...\})$$

Additivity since disjoint events

$$=\sum_{k=m+1}^{\infty}P(\text{first\:}H \text{\:on\:} k^{th}\text{toss})$$

$$=\sum_{k=m+1}^{\infty}P(TT...H)$$

$$=\sum_{k=m+1}^{\infty}(1-p)^{k-1}p$$

$$=(1-p)^mp+(1-p)^{m+1}p+...$$

$$=\frac{(1-p)^mp}{1-(1-p)}=(1-p)^m$$

$$P(\{TTT...T\})=(1-p)^m$$

------

#### Example

Roll a 6-sided die 7 times. Rolls are independent

Once each roll, probability of getting $$k, (k=1,2,...,6)$$ is $$p_k$$

$$p_1+p_2+...+p_6=1$$

Probability of getting this sequence (1123456)$$=p_1 \cdot p_1 \cdot p_2 \cdot p_3 \cdot p_4 \cdot p_5 \cdot p_6$$

Probability of getting (2311564) $$=p_1 \cdot p_1 \cdot p_2 \cdot p_3 \cdot p_4 \cdot p_5 \cdot p_6$$

Probability of getting 2 ones, 1 two, 1 three, 1 four, 1 five, 1 six?

$$=\sum_{\text{sequence with 2 ones, 1 twos, ...}}P(\text{sequence})$$

$$=\{\text{Number of sequence with 2 ones, 1 twos, ...}\} \cdot p_1^2p_2...p_6$$

$$=\frac{7!}{2!1!...1!}p_1^2p_2...p_6$$

------

Sequential experiment with $$n$$ independent sub-experiments

On each sub-experiment, there are $$m$$ possible outcomes with probability $$p_1, p_2, ... p_m$$

$$\sum_{i=1}^{m}p_i=1$$

Probability(Outcome 1 happens $$k_1$$ times, Outcome 2 happen $$k_2$$ times, ... Outcome $$m$$ happens $$k_m$$ times)

$$k_1+k_2+...k_m=n$$

$$=\{\text{Number of valid sequences}\}p_1^{k_1}p_2^{k_2}...p_m^{k_m}$$

$$=\binom{n}{k_1,k_2, ...k_m}p_1^{k_1}p_2^{k_2}...p_m^{k_m}$$

### Multinomial probability Law

------

### Random Variable

6-sided die

Roll it 3 times

Number of sequence with 1 even 2 odds

Pick 1 position for even number:  $$\binom{3}{1}$$

Pick an even number to put in the selected position: 3

Pick 2 odd number to put in the other 2 position: $$3^2$$

$$\binom{3}{1} \cdot 3 \cdot 3^2=3^4$$



6-sided die

$$n$$ rolls, $$k$$ even numbers, $$n-k$$ odd numbers

Pick $$k$$ positions for the evens: $$\binom{n}{k}$$

Pick $$k$$ even numbers: $$3^k$$

Pick $$(n-k)$$ odds: $$3^{n-k}$$

$$\sum_{k=0}^{n}\binom{n}{k}3^n=\sum_{k=1}^{n}\text{Number of sequence with\: }k \text{\:events}=\text{Total number of sequence}$$

$$3^n\sum_{k=0}^{n}\binom{n}{k}=6^n$$

$$3^n2^n=6^n$$

------

## Week 4 Session 1

Suppose we have a sequential experiment with $$n$$ independent sub-experiments

Consider event $$A_1,A_2, ... A_n$$

where $$A_i's$$ occurrence depends only on outcome of $$i^{th}$$ sub-experiment

Then $$A_1, A_2, ... A_n$$ are independent



#### Example

Coin toss $$n$$ times

Each toss is $$H$$ with probability $$p$$ and $$T$$ with probability $$(1-p)$$

Coin tosses are independent

$$P(\text{Getting\:}k \text{\:heads in\:} n \text{\:independent coin tosses})=p^k(1-p)^{n-k}$$

$$k=\{0,1,2,...n\}$$

Binomial probability law

$$A=\{\text{first\:}k\text{\:out of\:}n\text{\:coin tosses are\:}H\}$$

$$B=\{\text{There were\:\}}k H\text{\:in\:}n\text{\:coin tosses}$$

$$P(A|B)=\frac{P(A\bigcap B)}{P(B)}=\frac{p^k(1-p)^{n-k}}{\binom{n}{k}\:p^k(1-p)^{n-k}}=\frac{1}{\binom{n}{k}}$$

$$A\bigcap B=HH...HT...T$$ where there are $$kH,(n-k)T$$ 



$$\sum_{k=0}^{n}\binom{n}{k}\:p^k(1-p)^{n-k}=1$$

Probabilistic way:

$$\sum_{k=0}^{n}P(\{\text{Getting\:}kH \text{\:in tosses}\})$$

$$=P(\{\text{Getting 0H\}}\bigcap\{1H\}...\bigcap{nH})$$

$$=P(\Omega)=1$$



Algebraic way:

Binomial expansion:

$$(a+b)^n=\sum_{k=0}^{n}\binom{n}{k}a^kb^{n-k}$$

where $$a=p,b=1-p$$

$$\sum_{k=0}^{n}\binom{n}{k}p^k(1-p)^{n-k}=(p+1-p)^n=1$$

say $$p=1/2$$

$$\sum_{k=0}^{n}\binom{n}{k}\frac{1}{2^n}=1$$

$$\sum_{k=0}^{n}\binom{n}{k}=2^n$$

------

### Random Variables

Probability model $$\Omega, \mathcal{F}, p$$

Definition: A random variable (RV) is a function from $$\Omega$$ to real number $$\R$$

$$X:\Omega \rightarrow \R$$



#### Example

Coin toss $$n=2$$ times with independent tosses

$$X(\omega)=\{\text{Number of \:}H \text{\:in\:} \omega\}$$



#### Example

$$H: \Omega \rightarrow \R$$

$$H(\omega)=\{\text{Height of selected student}\}$$



### Remark

1. $$X$$ is a function

   Fix $$\omega$$, then $$X(\omega)$$ is a fixed real number

2. $$X$$ may be a many-to-one function

   It is possible to have $$X(\omega_1)=X(\omega_2)$$ for some $$\omega_1 \neq \omega_2$$

------

Events in terms of RVs

$$X: \omega \rightarrow \R$$

$$A=\{\omega \in \Omega: X(\omega)=2\}$$ is an event

$$B=\{\omega \in \Omega: 0\leq X(\omega) \leq2\}$$

$$C=\{\omega \in \Omega: sin(X(\omega))>0\}$$

$$P(\{\omega \in \Omega: X(\omega)=2\})$$

Notation: $$P(X=2)$$

$$P(\{\omega \in \Omega: X(\omega)\leq2\})$$

Notation: $$P(X\leq2)$$

$$P(\{\omega \in \Omega: X(\omega)\in (a,b)\})$$

Notation: $$P(X\in (a,b))=P(a<x<b)$$



#### Example

$$n$$ coin toss, independent toss

Probability of $$H=p$$

Probability of $$T=1-p$$

$$X(\omega)=\text{Number of\:}H \text{\:in\:} \omega$$

$$P(X=0)= P(\{\omega \in \Omega: X(\omega)=0\})$$

$$=P(\{TT...T\})$$

$$=(1-p)^n$$



$$P(X\leq1)= P(\{T...T,HT...T,TH...T,...\})$$

$$=(1-p)^n+np(1-p)^{n-1}$$

$$P(X\leq1)=P(\{X=0\}\bigcap\{X=1\})$$

$$=P(X=0)+P(X=1)$$

$$=P(\text{Getting 0H})+P(\text{Getting 1H})$$

$$=\binom{n}{0}p^k0(1-p)^{n-0}+\binom{n}{1}p^1(1-p)^{n-1}$$

$$=(1-p)^n+np(1-p)^{n-1}$$



#### Example

Roll a 4-sided die two times

Rolls are independent. Die is fair.

$$\Omega=\{(1,1),(1,2),...(4,4)\}$$

$$z=\text{Number on the 2nd roll}$$

$$P(z=1)=P(\text{Get 1 on 2nd roll})=1/4$$

$$P(\{1,1\}=P(\text{1 on first})P(\text{1 on second})=1/4 \cdot 1/4=1/16$$

$$P(\{(1,1),(1,2),...(4,4)\})=4 \cdot 1/16=1/4$$

$$X=$$ minimum if the numbers on the 2 roll

$$P(X=4)=P(\{4,4\})=1/16$$

$$P(X=2)=P(\{2,2\},\{2,3\},\{2,4\},\{3,2\},\{4,2\})=5/16$$



Exercise: $$P(X=3), P(X=1)$$

------

### Discrete RVs

Range of RV $$X=$$ all possible values $$X(\omega)$$ can take

Coin toss example $$X=\text{number of }H$$ 

Range of $$X$$: $$S_x=\{0,1,2...,n\}$$

Definition: A RV $$X$$ is discrete if $$S_x$$ is a finite or a countably infinite set.



#### Example

Coin with probability $$H=p, T=1-p$$

Independent coin tosses.

Keep tossing until a $$H$$ appears

$$N=\text{Number of tosses until an\:}H\text{\:appears}$$

$$S_N=\{1,2,3,...\}$$

$$N$$ is a discrete RV

$$P(N=1)=p$$

$$P(N=k)=(1-p)^{k-1}p$$ where $$k \geq 2$$



$$S_x=\{x_1,x_2,...x_n\}$$

$$S_x=\{x_1,x_2,x_3,...\}$$

Notations: $$X,Y,Z$$ to indicate RV

$$P(X=x)$$ 

$$x,y,z$$ indicates real number/ values that a RV may take



### Probability Mass Function (PMF)

$$S_x=\{x_1,x_2,...x_n\}$$

$$P_{X}(x_i)=P(X=x_i)=P(\{\omega\in \Omega:X(\omega)=x_i\})$$

1. $$0 \leq P_{X}(x_i) \leq 1$$

2. $$S_x=\{x_1,x_2,...x_n\}$$

   $$a \neq S_x$$

   $$P(X=a)=P(\{\omega\in \Omega:X(\omega)=a\})=P(\phi)=0$$

3. $$P(\{X=x_1\}\bigcap\{X=x_2\})=0$$

   Disjoint Events

4. $$P(\{X=x_1\}\bigcup\{X=x_2\}\bigcup...\{X=x_n\})=P(\Omega)=1$$

   $$\sum_{i=1}^{n}P(X=x_i)$$

   $$\sum_{i=1}^{n}P_X(x_i)$$

   $$\sum_{i=1}^{n}P_X(x_i)=1$$

   PMF add up to 1

5. $$\{X=x_1\}, \{X=x_2\}, ..., \{X=x_n\}$$ form a partition of $$\Omega$$

6. Let $$(a,b)$$ be an interval in $$\R$$

   $$P(X\in (a,b))$$

   Law of total probability: $$\sum_{i=1}^{n}P(X \in (a,b)\bigcap X=x_i)$$

   $$=\sum_{i: x_i \in (a,b)}P(X\in (a,b) \bigcap X=x_i)+\sum_{i: x_i \notin (a,b)}P(X\in (a,b) \bigcap X=x_i)$$

   where $$\sum_{i: x_i \notin (a,b)}P(X\in (a,b) \bigcap X=x_i)=0$$

   $$=\sum_{i: x_i \in (a,b)}P(X=x_i)$$

   $$=\sum_{i: x_i \in (a,b)}P_X(x_i)$$

   Therefore: $$P(X\in (a,b))=\sum_{i: x_i \in (a,b)}P_X(x_i)$$

$$P(X\in(1,2)\bigcup X\in(4,5))$$

$$=P(X \in (1,2))+P(X\in(4,5))$$

$$=\sum_{x_i \in(1,2)P_X(x_i)}+\sum_{x_i \in(4,5)P_X(x_i)}$$

$$=\sum_{x_i\in (1,2)\bigcup (4,5)}P_X(x_i)$$

For any arbitrary subset $$B$$ pf the real line

$$P(X \in B)=\sum_{i: x_i\in B}P_X(x_i)$$



#### Example

Coin toss $$n$$ times independent. 

$$X=\text{Number of \:} H\text{\: that appear}$$

$$S_x=\{0,1,...,n\}$$

Binomial RV:

$$P_X(k)=\binom{n}{k}p^k(1-p)^{n-k}$$ where $$0 \leq k \leq n$$

$$X \sim \text{Binomial}(n,p)$$

$$X \sim \text{Binomial}(10,1/2)$$

$$P_X(k)=\binom{10}{k}\frac{1}{2^k}\frac{1}{2^{n-k}}$$ where $$0 \leq k \leq 10$$

$$P(X \geq 9)=P_X(9)+P_X(10)$$

$$P(X < 0.8)=P_X(0)$$

$$P(|X-5|\leq 1)=P_X(4)+P_X(5)+P_X(6)$$



#### Example

If $$X \geq n-1$$, then I win $100.

Otherwise if $$X<n-1$$, I lose $10

$$Y=$$ my earnings, $$y=g(x)$$

<u>What is the PMF of y?</u>

$$S_y=\{100,-10\}$$

$$P_Y(100)=P(y=100)=P(X \geq n-1)=P_X(n-1)+P_X(n)$$

$$P_Y(-10)=1-P_Y(100)=1-P_X(n-1)-P_X(n)$$



#### Example

Keep repeating independent coin tosses until $$H$$ 

$$N=$$ Number of coin tosses until $$H$$

<u>What is the PMF of $$N$$</u>

$$S_N=\{1,2,3,...\}$$

For $$k \geq 1$$

$$P_N(k)=P(N=k)=(1-p)^{k-1}p$$ 

Geometric RV

$$X \sim \text{Geometric}(p)$$



$$X\sim \text{Binomial}(n,p)$$

$$P_X(k)=\binom{n}{k}p^k(1-p)^{n-k}$$

#### Example

Roll a fair 4-sided die.

$$X=$$ Number that appears

$$S_X=\{1,2,3,4\}$$

$$P_X(k)=P(X=K)=1/4$$

Uniform RV

Uniform RV with range $$=\{1,2,...,m\}$$ where $$1\leq k \leq m$$

$$P_X(k)=1/m$$ 

Uniform RV with range $$=\{-m,-(m-1),...,m\}$$ where $$-m\leq k \leq m$$

$$P_X(k)=1/(2m+1))$$ 

------

## Week 4 Session 2

### Random Variable

$$X: \Omega \rightarrow \R$$

for each $$\omega \in \Omega$$, $$X(\omega)$$ is a real number

Events:

$$P(a<X \leq b)=P(\{\omega \in \Omega: a<X(\omega)\leq b\})$$

Discrete RV:

finite or countably infinite range $$S_X$$

$$S_x=\{x_1,x_2,...x_n\}$$

$$S_x=\{x_1,x_2,x_3,...\}$$

$$S_X=\{\text{All possible values of\:}X(\omega)\text{\:for all\:}\omega \in \Omega\}$$ 

PMF of $$X$$: 

$$P(X\in B)=\sum_{i: x_i \in B}P_X(x_i)$$

$$P(a< X\leq b)=\sum_{i: a<x_i \leq b}P_X(x_i)$$

$$P(ax^3+bx^2+cx>0)=\sum_{i: ax_i^3+bx_i^2+cx_i>0}P_X(x_i)$$



#### Example

$$X\sim \text{Binomial}(n,p)$$

$$P_X(k)=\binom{n}{k}p^k(1-p)^{n-k}$$ where $$0 \leq k \leq n$$

$$P(X \geq 1)=\sum_{k \geq 1}P_X(k)$$

$$=\sum_{k \geq 1}\binom{n}{k}p^k(1-p)^{n-k}$$

or

$$=1-P(X<1)$$

$$=1-P(X=0)$$

$$=1-\binom{n}{0}p^0k(1-p)^{n-0}$$

$$=1-(1-p)^n$$

------

### Bernoulli RV

$$S_X=\{0,1\}$$

$$P_X(1)=p, P_X(0)=1-p$$

$$X \sim \text{Bernoulli}(p)$$



#### Example

$$X:\Omega \rightarrow \R$$

$$X(\omega)= \begin{cases}1 &\text{if\:} \omega \in A \\0 &\text{if\:} \omega \notin A \end{cases}$$

Indicator RV for event $$A$$, $$I_A$$

$$P_X(1)=P(X=1)$$

$$=P(\{\omega \in \Omega: X(\omega)=1\})$$

$$=P(A)$$

$$P_X(0)=1-P_X(1)=1-P(A)=P(A^c)$$

------

### Poisson RV

$$S_X=\{0,1,2,3...\}$$

$$P_X(k)=\frac{e^{-\lambda}\lambda^k}{k!}$$ for $$k=0,1,2...$$

Here, $$\lambda$$ is a fixed positve number

$$X \sim \text{Poisson}(\lambda)$$

$$P_X(k) \geq 0$$

$$\sum_{k \geq 0}P_X(k)=\sum_{k\geq 0}\frac{e^{-\lambda}\lambda^k}{k!}$$

$$=e^{-\lambda} \sum_{k\geq 0} \frac{\lambda^k}{k!}$$

$$=e^{-\lambda}e^{\lambda}=1$$

$$P(X \geq 1)=1-P(X<1)$$

$$=1-P(X=0)$$

$$=1-\frac{e^{-\lambda}\lambda^0}{0!}$$

$$=1-e^{-\lambda}$$

------

#### Example

$$Z$$ is a discrete RV

$$P(Z \leq 1) \leq P(Z\leq 2)$$

where $$P(Z\leq 1)=0.1, P(Z\leq 2)=0.2$$

$$P(Z \leq2)=P(\{Z \leq 1\}\bigcup\{1<Z \leq 2\})$$

$$=P(Z\leq 1)+P(1<Z \leq 2)$$

$$P(1<Z\leq 2)=0.2$$

------

### Expected Value of RV

Definition: $$X$$ is a discrete RV

$$E[X]=\sum_{x \in S_X}xP_X(x)$$

$$S_X=\{x_1,x_2, ... x_n\}$$

$$E[X]=\sum_{x_i \in S_X}x_iP_X(x_i)$$ , finite value



$$S_X=\{x_1,x_2, ... \}$$

$$E[X]=\sum_{i=1}^{\infty}x_iP_X(x_i)$$

It is possible that this infinite series doesn't converge. In that case, $$E[X]$$​ is undefined.

------

#### Example

$$X \sim \text{Bernoulli}(p)$$

$$S_X=\{0,1\}$$

$$P_X(1)=p, P_X(0)=1-p$$

$$E[X]=0 \cdot (1-p)+1 \cdot p=p$$

------

#### Example

$$X \sim \text{Uniform with range\:} S_X=\{0,1, ..., (M-1)\}$$

$$P_X(k)=1/M, 0 \leq k \leq M-1$$

$$E[X]=\sum_{k=0}^{M-1}k \cdot 1/M$$

$$=1/M \cdot \sum_{k=0}^{M-1}k$$ 

$$=1/M \cdot \frac{M(0+M-1)}{2}$$

$$=\frac{M-1}{2}$$

In general of PMF is symmetric about same number $$c$$

$$P_X(c+a)=P_X(c-a), \forall a \in \R$$

Then $$E[X]=c$$

------

#### Example

$$X \sim \text{Binomial}(3,0.5)$$

$$P_X(k)\binom{3}{k}\frac{1}{2^k}(1/2)^{3-k}$$ , $$k=0,1, 2, 3$$

$$E[X]=\sum_{k=0}^{3}k \cdot P_X(k)$$

$$=1 \cdot \binom{3}{1}\frac{1}{2^3}+2 \cdot \binom{3}{2}\frac{1}{2^3}+3 \cdot \binom{3}{3}\frac{1}{2^3}=1.5$$

Result:

$$X \sim \text{Binomial}(n,p)$$

$$E[X]=np$$

------

### Interpretation of $$E[X]$$

$$S_X=\{1,2,4\}$$

$$P_X(1)=1/4, P_X(2)=1/2, P_X(4)=1/4$$

------

$$N$$ independent repetitions of the underlying random experiment and record the value of $$X$$ in each experiment

$$2,2,4,1,2,1,2,4,...$$

Average value$$=\frac{\text{Add up all numbers}}{N}$$

$$=\frac{(\text{number of times 1})\cdot 1+(\text{number of times 2})\cdot 2+(\text{number of times 4})\cdot 4}{N}$$

$$=\sum_{x\in S_X}x \cdot \frac{\text{number of times\:}x \text{\:appears}}{N}$$

As $$N \rightarrow \infty$$, $$\text{number of times\:}x \text{\:appears} \rightarrow P_X(x)$$

Empirical average $$\rightarrow \sum_{n \in S_X}x \cdot P_X(x)=E[X]$$

------

$$X \sim \text{Binomial}(n,p), E[X]=np$$

$$P_X(k)=\binom{n}{k}p^k(1-p)^{n-k}$$ , $$0 \leq k \leq n$$

Binomial expansion

$$(a+b)^n=\sum_{k=0}^{n}\binom{n}{k}a^kb^{n-k}$$

$$E[x]=\sum_{k=0}^{n}kP_X(k)$$

$$=\sum_{k=0}^{n}k\binom{n}{k}p^k(1-p)^{n-k}$$

$$=\sum_{k=0}^{n}k\frac{n!}{k!(n-k)!}p^k(1-p)^{n-k}$$

$$=\sum_{k=1}^{n}\frac{n!}{(k-1)!(n-k)!}p^k(1-p)^{n-k}$$

$$=\sum_{k=1}^{n}n\frac{(n-1)!}{(k-1)!((n-1)-(k-1)!)}p^k(1-p)^{n-k}$$

say $$j=k-1$$

$$=n\sum_{j=0}^{n-1}\frac{(n-1)!}{j!(n-1-j)!}p^{j+1}(1-p)^{(n-1)-j}$$

$$=np\sum_{j=0}^{n-1}\binom{n-1}{j}p^{j}(1-p)^{(n-1)-j}$$

where $$\binom{n-1}{j}p^{j}(1-p)^{(n-1)-j} $$ is a term from Binomial $$(n-1,p)$$ 

$$=np(p+1-p)^{n-1}$$

$$=np$$

------

$$X \sim \text{Geometric}(p), p >0$$

$$P_X(k)=(1-p)^{k-1}p$$ , $$k=1,2,3,...$$

say $$q=1-p$$

$$P_X(k)=q^{k-1}p$$

$$E[X]=\sum_{k=1}^{\infty}kq^{k-1}p$$

$$=p\sum_{k=1}^{\infty}kq^{k-1}$$

$$=p\frac{1}{(1-q)^2}$$

$$=1/p$$

Mathematics used:

$$\sum_{k=0}^{\infty}a^k=\frac{1}{1-a}$$ , $$0<a<1$$

$$\sum_{k=1}^{\infty}ka^{k-1}=\frac{1}{(1-a)^2}$$ , $$0<a<1$$

$$\sum_{k=1}^{\infty}ka^k=\frac{a}{(1-a)^2}$$ , $$0<a<1$$

------

#### Example

$$X \sim \text{Poisson}(\lambda)$$

$$P_X(k)=\frac{e^{-\lambda}\lambda^{k}}{k!}$$ , $$k=0,1,2,3...$$

$$E[X]=\sum_{k \geq 0}k\frac{e^{-\lambda}\lambda^{k}}{k!}$$

$$=\sum_{k \geq 1}k\frac{e^{-\lambda}\lambda^{k}}{k!}$$

$$=\sum_{k \geq 1}\lambda\frac{e^{-\lambda}\lambda^{k-1}}{(k-1)!}$$

$$=\lambda e^{-\lambda} \sum_{k \geq 1}\frac{\lambda^{k-1}}{(k-1)!}$$

where $$\sum_{k \geq 1}\frac{\lambda^{k-1}}{(k-1)!}=e^\lambda$$

$$=\lambda$$



#### Example

$$S_X={3}$$ constant RV, degenerate RV

$$P_X(3)=1$$

$$E[X]=\sum_{x\in S_X}xP_X(x)=3 \cdot 1=3$$

$$E[3]=3$$

In general $$E[a]=a$$ where $$a \in \R$$



#### Example

$$S_X=\{1,2,3,...\}$$

$$P_X(k)=\frac{1}{ck^2}$$ where $$k=1,2,...$$ , $$c$$ is a positive constant

$$\sum_{k \geq1}\frac{1}{ck^2}=1$$

$$\frac{1}{c}\sum_{k \geq1}\frac{1}{k^2}=1$$

$$\sum_{k \geq1}\frac{1}{k^2}=c$$

where $$\sum_{k \geq1}\frac{1}{k^2}\rightarrow \frac{\pi^2}{6}$$

$$E[X]=\sum_{k \geq 1}k P_X(k)$$

$$=\frac{1}{c}\sum_{k \geq1}\frac{k}{k^2}$$

$$=\frac{1}{c}\sum_{k \geq1}\frac{1}{k}$$

where $$\sum_{k \geq1}\frac{1}{k} \rightarrow \infty$$

$$E[X]=\infty$$

------

### Remarks

If $$S_X$$ is countably infinite and it included both positive and negative values

$$E[X]=\sum_{x\in S_X}xP_X(x)$$

$$=\sum_{x\in S_X, x\geq 0}xP_X(x)+\sum_{x\in S_X, x < 0}xP_X(x)$$

If $$\sum_{x\in S_X, x\geq 0}xP_X(x)\rightarrow \infty$$  

If $$\sum_{x\in S_X, x < 0}xP_X(x)\rightarrow -\infty$$

$$E[X]=\infty-\infty$$ which is undefined

------

### Properties of $$E[X]$$

$$S_X=\{x_1, x_2, ...\}$$

Suppose $$x_i \geq a$$ for $$i=1,2...$$

$$E[X]\geq a$$

$$E[X]=\sum_{x\in S_X}xP_X(x)=\sum_{x\in S_X}aP_X(x)=a\sum_{x\in S_X}P_X(x)=a$$

Similarly if $$x_i \leq b \forall x_i \in S_X$$ 

$$E[X] \leq b$$

------

### Function of a RV

$$S_X=\{-3,-1,1,3\}$$

$$X \sim \text{uniform over the range \:}S_X$$ 

$$E[X]=0, Y=X^2$$ 

$$S_Y=\{1,9\}$$

$$P_Y(y)$$

$$P_Y(1)=P(Y=1)=P(X^2=1)=P_X(1)+P_X(-1)=1/2$$

$$P_Y(9)=1-P_Y(1)=1/2$$

$$E[Y]=1 \cdot 1/2 + 9 \cdot 1/2=5$$

------

#### Result

If $$y=g(x)$$, then

$$E[Y]=\sum_{x \in S_X}g(x)P_X(x)$$

------

$$E[Y]=E[X^2]=5 \neq (E[X])^2$$

In general $$E[g(x)] \neq g(E[X])$$



Proof of result

$$Y=g(x)$$ , $$S_y=\{y_1,y_2, ... y_m\}$$

$$E[Y]=\sum_{y \in S_y}yP_Y(y)$$

$$P_Y(y)=P(Y=y)=P(g(x)=y)$$

$$=\sum_{x_i: g(x_i)=y}P_X(x_i)$$

So, $$E[Y]=\sum_{y \in S_y}y(\sum_{x_i: g(x_i)=y}P_X(x_i))$$

RHS: 

$$\sum_{x \in S_X}g(x)P_X(x)$$

$$=\sum_{x\in S_X: g(x)=y_1}g(x)P_X(x)+\sum_{x\in S_X: g(x)=y_2}g(x)P_X(x)+...\sum_{x\in S_X: g(x)=y_m}g(x)P_X(x)$$

$$=\sum_{x\in S_X: g(x)=y_1}y_1P_X(x)+\sum_{x\in S_X: g(x)=y_2}y_2P_X(x)+...\sum_{x\in S_X: g(x)=y_m}y_mP_X(x)$$

$$=y_1\sum_{x\in S_X: g(x)=y_1}P_X(x)+y_2\sum_{x\in S_X: g(x)=y_2}P_X(x)+...y_m\sum_{x\in S_X: g(x)=y_m}P_X(x)$$

------

## Week 5 Session 1

Expected value of RV

Definition: $$X$$ is a discrete RV

$$E[X]=\sum_{x\in S_X}x P_X(x)$$

Function of a RV

If $$y=g(x)$$

Then $$E[Y]=\sum_{x\in S_X}g(x)P_X(x)$$

Why?

By definition of $$E[Y]$$

$$E[Y]=\sum_{y \in S_Y}yP(Y=y)$$ where $$P(Y=y)=P(g(x))=y)$$

$$=\sum_{y \in S_Y}y(\sum_{x:g(x)=y}P_X(x))$$

$$=y_1\sum_{x:g(x)=y_1}P_X(x)+y_2\sum_{x:g(x)=y_2}P_X(x)+ ...$$

Moreover

$$\sum_{x \in S_X}g(x)P_X(x)$$ $$\text{rearrange terms}$$ equals to the above

------

#### Example

$$X$$ uniform $$S_X=\{-3,-1,1,3\}$$

$$E[X]=0$$

$$Y=g(x)=\begin{cases}1 & \text{\:if\:} x<0 \\ 0 & \text{\:if\:} x \geq0 \end{cases}$$

$$E[Y]=\sum_{x \in S_X}g(x)P_X(x)=1 \cdot 1/4 + 1 \cdot 1/4 + 0 \cdot 1/4 + 0 \cdot 1/4=1/2$$

$$g(E[X])=0 \neq E[g(x)]$$

------

### Linearity properties of Expectation

1. $$E[aX+b]=aE[X]+b$$

   $$Y=aX+b$$

   $$E[Y]=\sum_{x \in S_X}(ax+b)P_X(x)$$

   $$=\sum_{x \in S_X}a_xP_X(x)+\sum_{x\in S_X}bP_X(x)$$

   $$=aE[X]+b$$

2. $$E[ag(x)+bh(x)+c]$$

   $$=aE[g(x)]+bE[h(x)]+c$$
   
   $$Z=ag(x)+bh(x)+c$$
   
   $$E[Z]=\sum_{x\in S_X}(ag(x)+bh(x)+c)P_X(x)$$
   
   $$=a\sum_{x}g(x)P_X(x)+b\sum h(x)P_X(x)+c\sum P_X(x)$$
   
   $$=aE[g(x)]+bE[h(x)]+c$$



#### Example

$$E[X]=0$$ ,mean of $$X$$, mean value of $$X$$, $$1^{st}$$ moment of $$X$$

$$E[X^2]=5$$ , $$2^{nd}$$ moment of $$X$$

$$E[X^n]$$ , $$n^{th}$$ moment of $$X$$

$$Y=(2x+10)^2$$

$$E[Y]=E[(2X+10)^2]$$

$$=E[4X^2+40X+100]$$

$$=4E[X^2]+40E[X]+100$$

$$=120$$



#### Example

$$X \sim \text{Binomial}(48,1/3)$$ , $$S_X=\{0,1,...,48\}$$

$$X$$ is the number of voice packets that need to be transmitted.

Transmitter can only send 20 packets.

If $$X$$ is more than 20, the excess packets are discarded.

<u>Expected number of discarded packets</u>

$$Y=g(x)=\begin{cases}x-20 &\text{if\:}x>20 \\ 0 &\text{if\:} x \leq 20\end{cases}$$ 

$$E[Y]=\sum_{x\in S_X}g(x)P_X(x)$$

$$=\sum_{k=0}^{20}0 \cdot P_X(x)+\sum_{k=21}^{48}(k-20) \cdot P_X(k)$$

$$=\sum_{k=21}^{48}(k-20)\binom{48}{k}(\frac{1}{3})^k(\frac{2}{3})^{48-k}$$

$$=0.182$$

------

$$E[X]=0$$

$$Var(X)=E[(X-0)^2]$$

$$=E[X^2]=(1)^2 \cdot 1/2 + (-1)^2 \cdot 1/2$$

$$=1$$



$$E[Y]=0$$

$$Var[Y]=E[(Y-0)^2]$$

$$=E[Y^2]=100$$



### Variance of a RV

$$E[(X-m_X)^2]$$

Variance of $$X$$ : $$Var(X)$$ or $$\sigma_X^2$$

------

Standard Deviation

$$\sigma_X=+\sqrt{Var(X)}$$



#### Example

$$X \sim \text{Bernoulli}(p)$$

$$S_X=\{0,1\}$$

$$P_X(1)=p, P_X(0)=1-p$$

$$E[X]=0\cdot P_X(0)+1 \cdot P_X(1)=p$$

$$Var[X]=E[(X-p)^2]$$

$$=(0-p)^2P_X(0)+(1-p)^2P_X(1)$$

$$=p^2(1-p)+(1-p)^2p$$

$$=p(1-p)$$

------

#### Example: Degenerate/ Constant RV

$$S_X=\{c\}$$

$$E[X]=c \cdot 1=c$$

$$Var(X)=E[(X-c)^2]$$

$$=\sum_{x \in S_X}(x-c)^2P_X(x)=0$$

------

$$Var(X)=E[(X-m_X)^2]=\sum_{x \in S_X}(x-m_X)^2P_X(x)$$

$$Var(X)=E[(X-m_X)^2]=E[X^2-2m_XX+m_X^2]$$

$$=E[X^2]-2m_XE[X]+m_X^2$$

$$=E[X^2]-2m_Xm_X+m_X^2$$

$$=E[X^2]-m_X^2$$

$$E[ag(x)+bh(x)+c]=aE[g(x)]+bE[h(x)]+c$$ applied

$$Var(X)=E[X^2]-m_X^2$$

------

#### Example

$$Y=X+c$$

$$E[Y]=E[X+c]=E[X]+c$$ where $$E[X]=m_X$$ 

$$Var(Y)=E[(Y-m_Y)^2]$$ where $$m_Y=m_X+c$$

$$=E[(x+c-(m_X+c))^2]$$

$$=E[(X-m_X)^2]$$

$$=\sigma_X^2$$

If $$Y=X+c$$, then $$Var(Y)=Var(X)$$

------

#### Example

$$Y=c \cdot X$$

$$E[Y]=E[cX]=cE[X]=cm_X$$

$$Var(Y)=E[(Y-m_Y)^2]$$

$$=E[(cX-cm_X)^2]$$

$$=E[c^2(X-m_X)^2]$$

$$=c^2E[(X-m_X)^2]$$

$$=c^2Var(X)$$

If $$Y=cX$$, then $$Var(Y)=c^2Var(X)$$

If $$Y=-X$$, then $$Var(Y)=Var(X)$$

------

#### Example

$$X, m_X, \sigma_X^2$$

$$Y=\frac{X-m_X}{\sigma_X}$$

$$E[Y]=E[\frac{1}{\sigma_X}(X-m_X)]$$

$$=\frac{1}{\sigma_X}E[(X-m_X)]$$

$$=\frac{1}{\sigma_X}(E[X]-m_X)$$

$$=0$$

$$Var(Y)=E[(Y-0)^2]$$

$$=E[Y^2]$$

$$=E[\frac{(X-m_X)^2}{\sigma_X^2}]$$

$$=E[\frac{1}{\sigma_X^2}(X-m_X)^2]$$

$$=\frac{1}{\sigma_X^2}E[(X-m_X)^2]$$

$$=\frac{\sigma_X^2}{\sigma_X^2}=1$$

$$\frac{X-m_X}{\sigma_X} \rightarrow$$ Normalized form of $$X$$ has mean 0 and variance 1

------

Conditional probability

Bayes' Rule

Total probability law



Let $$C$$ be any event with $$P(C)>0$$

$$P(A|C)=\frac{P(A \bigcap C)}{P(C)}$$

$$A=\{X=x\}=\{\omega \in \Omega: X(\omega)=x\}$$

$$P(A|C)=P(X=x|C)$$

$$=\frac{P(\{X=x\} \bigcap C)}{P(C)}$$

$$P_X(x|C):=\frac{P(\{X=x\} \bigcap C)}{P(C)}=P({X=x}|C)$$

We can use the above definition for all $$x\in S_X$$ 

$$S_X=\{x_1, x_2, ... , x_n\}$$

$$P_X(x_1|C), P_X(x_2|C), ... $$ are conditional PMF of $$X$$ given $$C$$

Results

1. $$0 \leq P_X(x_i|C) \leq 1$$

2. $$\sum_{x \in S_X}P_X(x|C)=1$$

3. a) $$P(x\in (a,b)|C)=\sum_{x \in (a,b)}P_X(x|C)$$

   b) If $$B$$ is any subset of $$\R$$

   $$P(X\in B|C)=\sum_{x \in B}P_X(x|C)$$

------

$$S_X=\{x_1,...,x_n\}$$

$$\sum_{i=1}^{n}P(X=x_i|C)=P(\Omega|C)=1$$

------

#### Example

$$X$$ has uniform PMF with $$S_X=\{1,2,...,L\}$$ for $$1 \leq k \leq L$$

$$P_X(k)=\frac{1}{L}$$

$$C=\{X>1\}$$

Conditional PMF of $$X$$ given $$C$$

$$P_X(1|C)=P(X=1|X>1)=\frac{P(X=1 \bigcap X>1)}{P(X>1)}=0$$

For $$2\leq k \leq L$$

$$P_X(k|C)=P(X=2|X>1)=\frac{P(X=2 \bigcap X>1)}{P(X>1)}=\frac{1/L}{1-1/L}=\frac{1}{L-1}$$

------

#### Example

$$X\sim \text{Geometric}(p)$$

$$S_X=\{1,2,3...\}$$ 

$$P_X(k)=(1-p)^{k-1}p$$ where $$k\geq 1$$

$$C=\{X>1\}$$

$$Y=X-1$$

Conditional PMF of $$Y$$ given $$C$$

$$P(Y=k|C)=P(Y=k|X>1)$$

$$=P(X-1=k|X>1)$$

$$=P(X=1+k|X>1)$$

$$=\frac{P(X=1+k \bigcap X>1)}{P(X>1)}$$

$$=\begin{cases} \frac{0}{1-p} & k=0\\ \frac{P_X(1+k)}{1-p} & k=1,2,...\end{cases}$$

$$P(Y=k|X>1)=P(X=k)$$

------

Exercise

$$X \sim \text{Geometric}(p)$$

$$C=\{X>m\}$$ where $$m$$ is a positive integer

$$Z=X-m$$

Find the conditional PMF of $$Z$$ given $$C$$

------

Chain Rule

$$P(A\bigcap B)=P(A|B)P(B)$$

Bayes' Rule

$$P(A|B)=\frac{P(B|A)P(A)}{P(B)}$$

Law of total probability

$$P(A)=\sum_{i=1}^{n}P(A \bigcap C_i)$$

$$=\sum_{i=1}^{n}P(A|C_i)P(C_i)$$

------

#### Example

Factory that produce 2 types of devices

Type 1 is produced with probability $$\alpha$$

Lifetime $$\sim \text{Geometric}(r)$$

Type 2 is produced with probability $$1-\alpha$$
Lifetime $$\sim \text{Geometric}(s)$$

I purchase a device from this factory $$X=$$ lifetimes of purchased device

$$S_X=\{1,2,3,...\}$$

<u>PMF of $$X$$</u>

$$P_X(k)=P(X=k)$$

$$=P(X=k|\text{Type 1})P(\text{Type 1})+P(X=k|\text{Type 2})P(\text{Type 2})$$

$$=(1-r)^{k-1}r\alpha+(1-s)^{k-1}s(1-\alpha)$$



Verify that $$P_X(k)$$ adds up to 1 of summed over all $$k \geq 1$$

Suppose I observe that $$X=m$$

$$P(\text{Type 1 device was purchased}|X=m)=\frac{P(X=m|\text{Type 1})P(\text{Type 1})}{P(X=m)}$$

$$=\frac{(1-r)^{m-1}r\alpha}{(1-r)^{m-1}r\alpha+(1-s)^{m-1}s(1-\alpha)}$$

$$P(\text{Type 1}|X> m)=\frac{P(X>m|\text{Type 1})P(\text{Type 1})}{P(X>m)}$$

where $$P(X>m|\text{Type 1})=\sum_{k=m+1}^{\infty}(1-r)^{k-1}r$$ 

$$P(X>m)=P(X>m|\text{Type 1})\alpha+P(X>m|\text{Type 2})(1-\alpha)$$

------

| PMF             | Expectation                         |
| --------------- | ----------------------------------- |
| $$P_X(k)$$      | $$E[X]=\sum_{x \in S_X}xP_X(x)$$    |
| Conditional PMF | Conditional Expectation             |
| $$P_X(x|C)$$    | $$E[X|C]=\sum_{x\in S_X}xP_X(x|C)$$ |

$$E[\text{lifetime}|\text{Type 1}]=\sum_{k=1}^{\infty}kP_X(k|\text{Type 1})$$

$$=\sum_{k=1}^{\infty}k(1-r)^{k-1}r$$

## Week 5 Session 2

1. $$E[aX+b]=aE[X]+b$$

2. $$Var[X]=E[(X-m_X)^2]=E[X^2]-m_X^2$$

3. Conditional PMF of RV $$X$$ given event $$C$$

   $$P_X(x|C)$$ for $$x\in S_X$$

------

Using law of total probability with RVs

Suppose $$C_1, C_2, ... C_n$$ is a partition of $$\Omega$$, then

$$P_X(x)=P(X=x)$$

$$=\sum_{i=1}^{n}P(\{X=x\}\bigcap C_i)$$

$$=\sum_{i=1}^{n}P(X=x|C_i)P(C_i)$$

$$=\sum_{i=1}^{n}P_X(x|C_i)P(C_i)$$

------

#### Example

$$X$$ is a discrete RV with range $$S_X=\{x_1,x_2,...x_n\}$$

For any real number $$c$$, the mean squared error is defined as follows

$$f(c)=E[(X-c)^2]$$

What choice of $$c$$ given the minimum value of $$f(c)$$

$$E[(X-c)^2]=\sum_{i=1}^{n}(x_i-c)^2P_X(x_i)$$

$$f(c)=\sum_{i=1}^{n}(x_i-c)^2P_X(x_i)$$

$$\frac{df(c)}{dc}=0$$

$$\sum_{i=1}^{n}-2(x_i-c)P_X(x_i)=0$$

$$\sum_{i=1}^{n}x_iP_X(x_i)=c\sum_{i=1}^{n}P_X(x_i)$$

$$c=m_X$$

$$\frac{d^2f(c)}{dc}>0$$

$$c=m_X$$

$$f(c)=f(m_X)=E[(X-m_X)^2]=Var(X)$$

------

### Conditional PMF given $$C$$

$$P_X(x|C), x\in S_X$$

Conditional expectation given $$C$$

$$m_{X|c}=E[X|C]=\sum_{x\in S_X}xP_X(x|C)$$

$$E[g(X)|C]=\sum_{x \in S_X}g(x)P_X(x|C)$$

Conditional variance given $$C$$

$$E[(X-m_{X|C})^2|C]=\sum_{x\in S_X}(x-m_{X|C})^2P_X(x|C)$$

------

### Law of total expectation

Theorem: Suppose $$C_1,...C_n$$ is a partition of $$\Omega$$. Then

$$P_X(x)=\sum_{i=1}^{n}P_X(x|C_i)P(C_i)$$

$$E[X]=\sum_{i=1}^{n}E[X|C_i]P(C_i)$$

Proof: 

$$E[X]=\sum_{x\in S_X}xP_X(x)$$

$$=\sum_{x\in S_X}x\sum_{i=1}^{n}P_X(x|C_i)P(C_I)$$

$$=\sum_{i=1}^{n}\sum_{x\in S_X}xP_X(x|C_i)P(C_i)$$

$$=\sum_{i=1}^{n}E[X|C_i]P(C_i)$$



$$Y=g(x)$$

$$E[Y]=\sum_{i=1}^{n}E[Y|C_i]P(C_i)$$

$$E[g(x)]=\sum_{i=1}^{n}E[g(x)|C_i]P(C_i)$$

------

Example

$$C_1,C_2$$ form a partition of $$\Omega$$

Given $$C_1$$. $$X\sim \text{Geometric}(r)$$

Given $$C_2$$. $$X\sim \text{Geometric}(s)$$

$$Z\sim \text{Geometric}(p)$$

$$E[Z]=1/p$$

$$E[Z^2]=\frac{1+p}{p^2}$$

<u>Find $$Var(X)$$</u>

$$Var(X)=E[X^2]-m_X^2$$

$$m_X=E[X]=E[X|C_1]P(C_1)+E[X|C_2]P(C_2)$$

$$=\frac{1}{r} P(C_1)+\frac{1}{s} P(C_2)$$

$$E[X^2]=E[X^2|C_1]P(C_1)+E[X^2|C_2]P(C_2)$$

$$=\frac{1+r}{r^2}P(C_1)+\frac{1+s}{s^2}P(C_2)$$

$$Var(X)=E[X^2]-(m_X)^2$$

------

#### Example

$$n$$ independent Bernoulli trials

Each trial may result in a success with probability $$p$$ or a failure with probability $$1-p$$
$$X=$$ number of successes in $$n$$ trials

$$P_X(k)=\binom{n}{k}p^k(1-p)^{n-k}$$ where $$0\leq k \leq n$$

Suppose $$X=1$$

<u>What is the conditional probability that the first trial was successful?</u>

$$A_1=\{\text{first trial is success}\}$$

$$P(A_1|X=1)=\frac{P(A_1\bigcap X=1)}{P(X=1)}$$

$$=\frac{P(SFFFF...F)}{\binom{n}{1}p^1(1-p)^{n-1}}$$

$$=\frac{p^1(1-p)^{n-1}}{\binom{n}{1}p^1(1-p)^{n-1}}$$

$$=\frac{1}{n}$$



$$A_2=\{\text{second trial is success}\}$$

$$P(A_2|X=1)=\frac{P(A_2\bigcap X=1)}{P(X=1)}$$

$$=\frac{P(FSFFF...F)}{\binom{n}{1}p^1(1-p)^{n-1}}$$

$$=\frac{1}{n}$$

------

#### Example

Given $$A_1$$, find the conditional PMF of $$X$$

$$S_X=\{0,1,...,n\}$$

$$P_X(0|A_1)=P(X=0|A_1)=0$$

For $$n \geq k \geq 1$$

$$P_X(k|A_1)=P(X=k|A_1)=\frac{P(X=k\bigcap A_1)}{P(A_1)}$$

$$P(A_1)=p$$

$$P(X=k \bigcap A_1)=P(A_1 \bigcap k-1 \text{\: success trials\: }2,3,...n)$$

$$=P(A_1)P(k-1 \text{\: success trials\: }2,3,...n)$$

$$=p\binom{n-1}{k-1}p^{k-1}(1-p)^{n-k}$$

$$P_X(k|A_1)=\binom{n-1}{k-1}p^{k-1}(1-p)^{n-k}$$ for $$1\leq k \leq n$$

------

$$P(X\geq n-1|A_1)=P_X(n-1|A_1)+P_X(n|A_1)$$

$$=\binom{n-1}{n-2}p^{n-2}(1-p)^{1}+p^{n-1}$$

$$=(n-1)p^{n-2}(1-p)+p^{n-1}$$

------

Conditional PMF of $$X$$ given $$A_1^c$$ 

$$S_X=\{0,1,...,n\}$$

$$P_X(n|A_1^c)=P(X=n|A_1^c)=0$$

For $$0 \leq k \leq n-1$$

$$P_X(k|A_1^c)=P(X=k|A_1^c)$$

$$=\frac{P(X=k \bigcap A_1^c)}{P(A_1^c)}$$

$$=\frac{P(A_1^c \bigcap k\text{\: success in trials 2,...,n})}{1-p}$$

$$=\frac{P(A_1^c)P(\text{success in trials 2,...,n})}{1-p}$$

$$=\binom{n-1}{k}p^k(1-p)^{n-1-k}$$

------

$$P_X(k|A_1), P_X(k|A_1^c)$$ where $$0 \leq k \leq n$$

Verify

$$P(X=k)=P(X=k|A_1)P(A_1)+P(X=k|A_1^c)P(A_1^c)$$



$$k=0$$

LHS: $$P(X=0)=(1-p)^n$$

RHS: $$P(X=0|A_1)P(A_1)+P(X=0|A_1^c)P(A_1^c)$$

$$=0 P(A_1)+(1-p)^{n-1}(1-p)$$

$$=(1-p)^n$$

------

$$P(A_1|X=2)=\frac{P(X=2|A_1)P(A_1)}{P(X=2)}$$

$$P(A_1 \bigcap A_2|X=2)=\frac{P(A_1 \bigcap A_2 \bigcap X=2)}{P(X=2)}$$

$$=\frac{pp(1-p)^{n-2}}{\binom{n}{2}p^2(1-p)^{n-2}}$$

$$=\frac{1}{\binom{n}{2}}$$



If $$A,B$$ are independent

$$P(A \bigcap B)=P(A)P(B)$$

If $$A,B$$ are disjoint

$$P(A \bigcup B|C)=P(A|C)+P(B|C)$$

$$P(A \bigcup B|C)=\frac{P(A\bigcup B \bigcap C) }{P(C)}$$

$$=\frac{P(A \bigcap C \bigcup B \bigcap C}{P(C)}$$

$$=\frac{P(A \bigcap C)+P(B \bigcap C)}{P(C)}$$

$$=P(A|C)+P(B|C)$$

------

$$Z \sim \text{Poisson}(\lambda)$$

$$P_X(k)=\frac{\lambda^ke^{-\lambda}}{k!}$$ for $$k=0,1,2...$$

$$E[Z]=\lambda$$

$$Var[Z]=\lambda$$

$$E[Z^2]=\lambda+\lambda^2$$

------

#### Example

Optical Communication

Receiver in an optical communication system. If message is being sent, then the receiver gets a random number of photons that has a Poisson PMF $$\lambda_1$$

If message is not being sent, then receiver gets a random number of photons with a Poisson PMF $$\lambda_0$$

$$\lambda_0 < \lambda_1$$

The prior probability that a message is being sent is $$p$$

a) Suppose the receiver get $$k$$ photons. <u>Conditional probability that a message was sent</u>

$$X=$$ number of photons at the receiver

$$M=\{\text{message is sent}\}$$ 

$$A=\{\text{message is absent}\}$$ , $$A=M^c$$

$$P(M|X=k)=\frac{P(X=k|M)P(M)}{P(X=k)}$$

Number$$=\frac{\lambda_1^ke^{-\lambda_1}}{k!}p$$

Denominator $$P(X=k)=P(X=k|M)P(M)+P(X=k|A)P(A)$$

$$=\frac{\lambda_1^ke^{-\lambda_1}}{k!}p+=\frac{\lambda_0^ke^{-\lambda_0}}{k!}(1-p)$$



b) Receiver calculates $$I=P(M|X=k)$$ and $$II=P(A|X=k)$$

Declares message present if $$I>II$$

Declares message absent if $$I<II$$

Declare present if: 

$$P(M|X=k)>P(A|X=k)$$ 

$$\frac{\frac{\lambda_1^ke^{-\lambda_1}}{k!}p}{P(X=k)}>\frac{\frac{\lambda_0^ke^{-\lambda_0}}{k!}(1-p)}{P(X=k)}$$

$$\frac{\lambda_1}{\lambda_0}^k>\frac{1-p}{p}e^{\lambda_1-\lambda_0}$$

$$k>\frac{log\frac{1-p}{p}+(\lambda_1-\lambda_0)}{log(\frac{\lambda_1}{\lambda_0})}=c$$

Receiver decision rule is 

Declare present if Number of photons $$>c$$

Declare absent if Number of photons $$\leq c$$



c) Suppose that a message is present. <u>What is the probability that the receiver makes a wrong declaration?</u> 

$$P(\text{Declaring Absent}|M)=P(X\leq c|M)$$

$$=\sum_{0  \leq k \leq c}e^{-\lambda_1}\frac{\lambda_1^k}{k!}$$



d) $$P(\text{Declares present}|A)=P(X>c|A)$$

$$=\sum_{k>c}e^{-\lambda_0}\frac{\lambda_0^k}{k!}$$



e) Probability that receiver makes a wrong declaration

$$W=\{\text{Weong declaration}\}$$

$$P(W)=P(W|M)P(M)+P(W|A)P(A)$$

$$=P(W|M)p+P(W|A)(1-p)$$



f) $$M \rightarrow X\sim \text{Poisson}(\lambda_1)$$

$$A \rightarrow X\sim \text{Poisson}(\lambda_0)$$

$$E[X]=E[X|M]P[M]+E[X|A]P[A]$$

$$=\lambda_1p+\lambda_0(1-p)$$



g) $$E[X^2]=E[X^2|M]P[M]+E[X^2|A]P[A]$$

$$=(\lambda+\lambda^2)p+(\lambda_0+\lambda_0^2)(1-p)$$

------

$$P(X=2), x\in S_X$$ 

Cumulative Distribution Function (CDF)

$$F_X(x)=P(X\leq x) \forall x \in \R$$

## Week 6 Session 1 (Only 1)

### Random variable (RV)

<u>Discrete RVs</u>

PMF

$$P_X(x_i)=P(X=x_i)$$ for each $$x_i \in S_x$$

<u>Non-discrete RV</u>

range of values in an uncountably infinite set

Example

$$S_x=[a,b]$$

$$S_x=\R$$

$$S_x=[0,\infty)$$

------

### Cumulative distribution function (CDF)

$$F_X(x)=P(X \leq x)$$ for all $$x\in \R$$

can be defined for all RVs (discrete or non-discrete)



#### Example

$$X \sim \text{Bernoulli} (p)$$

$$S_x=\{0,1\}$$

$$P_X(1)=p$$

$$P_X(0)=1-p$$

$$F_X(x)=P(X\leq x)$$

$$F_X(0)=P(X\leq 0)=(1-p)$$

$$F_X(1)=P(X \leq 1)=1$$



#### Example

$$X \sim \text{Binomial}(3,1/2)$$

$$S_X=\{0,1,2,3\}$$

$$P_X(k)=\binom{3}{k}(1/2)^3$$ where $$k=0,1,2,3$$

CDF: $$F_X(x)=P(X\leq x)$$

$$F_X(0)=P(X \leq 0)=P(X=0)=1/8$$

$$F_X(1)=P(X \leq 1)=P_X(0)+P_X(1)=4/8$$



#### Example

A constant RV $$S_X=\{0\}$$

$$P_X(0)=1$$



#### Example

Non-discrete RV

$$\Omega=(0,1]$$

$$P(\text{Any sub-interval of\:} \Omega)=\text{length of sub-interval}$$

$$X: \Omega \rightarrow \R$$

$$X(\omega)=\omega$$

$$S_X=(0,1]$$

$$P(1/2 \leq X \leq 1)=P(\{\omega \in \Omega: 1/2 \leq X(\omega) \leq1 \})$$

$$=P([1/2,1])=1/2$$

$$P(X \leq 1/3)=P(\{\omega \in \Omega: X(\omega) \leq 1/3\})$$

$$=P((0,1/3])=1/3$$



CDF $$F_X$$ for uniform RV over $$(0,1]$$

$$F_X(0)=P(X\leq 0)=0$$

$$F_X(2/3)=P(X\leq 2/3)=P((0,2/3])=2/3$$

$$0 < x \leq 1$$

$$F_X(x)=P(X \leq x)=P((0,x])=x$$



#### Example

A taxi is present with probability $$p$$ at the taxi when I arrive

Waiting time =0 if taxi is present

If not taxi is present, waiting time is uniform $$(0,1]$$ random variable

CDF of waiting time $$Y$$
$$F_Y(x)=P(Y \leq x)=P(Y \leq x | \text{Taxi present})P(\text{Taxi present})+P(Y \leq x | \text{Taxi absent})P(\text{Taxi absent})$$

$$=P(Y \leq x | \text{Taxi present})p+P(Y \leq x | \text{Taxi absent})(1-p)$$

$$P(Y \leq x | \text{Taxi present})=\begin{cases} 0 & \text{if\:} x<0 \\ 1 & \text{if\:} x \geq 0 \end{cases}$$

$$P(Y \leq x | \text{Taxi absent})=\begin{cases} 0 & \text{if\:} x\leq0 \\ x & \text{if\:} 0<x \leq 1 \\ 1 & \text{if\:} x>1 \end{cases}$$

$$F_Y(x)=\begin{cases} 0 & \text{if\:} x<0 \\ p & \text{if\: } x=0\\ p+(1-p)x & \text{if\:} 0<x \leq 1\\ 1 & \text{if\:} x>1 \end{cases}$$

Mixed RV

------

### Properties of CDF

1. $$0 \leq F_X(x) \leq 1$$

2. Let $$a<b$$

   $$F_X(a) \leq F_X(b)$$

   $$F_X$$ is a non decreasing function

   $$\{X \leq a\} \subset \{X \leq b\}$$

   $$F_X(a)=P(X \leq a) \leq P(X \leq b)=F_X(b)$$

3. Recall $$A_1 \subset A_2 ... \subset A_n$$

   $$P(\bigcup_{i=1}^{n}A_i)=P(A_n)$$

   $$A_1 \subset A_2 ... $$

   $$P(\bigcup_{i=1}^{\infty}A_i)=\lim_{n \rightarrow \infty}P(A_n)$$

   $$A_1=\{X\leq 1\}, A_2=\{X \leq 2\}, ... A_n=\{A \leq n\}$$

   $$P(\bigcup_{i=1}^{\infty}A_i)=\lim_{n \rightarrow \infty}P(X \leq n)$$

   $$P(\Omega)=\lim_{n \rightarrow \infty}F_X(n)$$

   ==$$1=\lim_{n \rightarrow \infty}F_X(n)$$==

4. $$B_1 \supset B_2 ... \supset B_n$$

   $$P(\bigcap_{i=1}^{n}B_i)=P(B_n)$$

   $$B_1 \supset B_2 ...$$

   $$P(\bigcap_{i=1}^{\infty}B_i)=\lim_{n \rightarrow \infty}P(B_n)$$

   $$B_1=\{X \leq -1\},B_2=\{X \leq -2\}... B_n=\{X \leq -n\}$$

   $$P(\bigcap_{i=1}^{\infty}B_i)=\lim_{n \rightarrow \infty}P(X \leq -n)$$

   $$P(\phi)=\lim_{n \rightarrow \infty}F_X(-n)$$

   $$0=\lim_{n \rightarrow \infty}F_X(-n)$$

   ==$$\lim_{x \rightarrow -\infty}F_X(x)=0$$==

5. $$\lim_{h \downarrow 0}F_X(b+h)=F_X(b)$$

   $$F_X$$ is a right continuous function

   Decreasing sequence

   $$B_1=\{X \leq b+1\}$$

   $$B_2=\{X \leq b+1/2\}$$

   $$...$$

   $$B_n=\{X \leq b+ 1/n\}$$

   $$P(\bigcap_{i=1}^{\infty}B_i)=\lim_{n \rightarrow \infty}P(B_n)$$

   $$P(X \leq b)=\lim_{n \rightarrow \infty}P(X \leq b+ 1/n)$$

   $$=\lim_{n \rightarrow \infty}F_X(b+1/n)$$

   ==$$F_X(b)=\lim(h \downarrow 0)F_X(b+h)$$==

   

   In general $$F_X$$ is not left-continuous, i.e., $$F_X(b)$$ and $$\lim_{h \downarrow 0}F_X(b-h)$$ may or may not be equal

   Example

   $$X \sim \text{Bernoulli}(p)$$

   $$P(X=0)=1-p$$

   $$F_X(0^{+})-F_X(0)=0$$

   $$F_X(0)=P(X\leq 0)=P(X=0)=1-p$$

   $$F_X(-h)=0$$

   $$\lim_{h \rightarrow 0}F_X(-h)=0 \neq F_X(0)$$

   

   $$F_X(b^{+}):= \lim_{h \downarrow 0}F_X(b+h)$$

   $$F_X(b^{-}):=\lim_{h \downarrow 0}F_X(b-h)$$

   $$F_X(b^{+})=F_X(b)$$

   but $$F_X(b^{-1})$$ and $$F_X(b)$$ may or may not be equal

6. $$P(X >x)=1-F_X(x)$$

7. Let $$a<b$$

   $$P(a < X \leq b)=F_X(b)-F_X(a)$$

   $$\{X \leq b\}=\{X \leq a\} \bigcup \{a < X \leq B\}$$     disjoint

   $$P(X \leq b)=P(X \leq a) +P (a < X \leq B)$$

8. $$P(X=b)=F_X(b)-F_X(b^{-})$$

   $$F_X(b^{-1})=\lim_{h \downarrow 0}F_X(b-h)$$

   Interval: $$(b-h,b]$$

   $$P(X=b)\leq P(b-h < X \leq b)=F_X(b)-F_X(b-h)$$

   $$P(X=b)\leq \lim_{h \downarrow 0}P(b-h < X \leq b)$$

   $$=F_X(b)-\lim_{h\downarrow 0}F_X(b-h)$$

   $$=F_X(b)-F_X(b^{-})$$

   More precisely,

   $$P(X=b)=F_X(b)-F_X(b^{-})$$

   

$$B_1=\{X \in (b-1,b)\}$$

$$B_2=\{X \in (b-1/2,b)\}$$

$$...$$

$$B_n=\{X \in (b-1/n,b)\}$$

$$P(\bigcap_{i=1}^{\infty}B_i)=\lim_{n\rightarrow \infty}P(B_n)$$

$$P(X=b)=\lim_{n \rightarrow \infty}P(b-1/n < X \leq b)$$

$$P(X=b)=\lim_{n \rightarrow \infty}F_X(b)-F_X(b-1/n)$$

$$P(X=b)=F_X(b)-\lim_{h \downarrow 0} F_X(b-h)$$

$$=F_X(b)-F_X(b^{-})$$



$$P(a < X \leq b)=F_X(b)-F_X(a)$$

$$P(X=b)=F_X(b)-F_X(b^{-})$$



#### Example

$$P(a \leq X \leq b)$$

$$\{a \leq X \leq b\}=\{X=a\} \bigcup \{a < X \leq b\}$$

$$P(a \leq X \leq b)=F_X(a)-F_X(a^{-})+F_X(b)-F_X(a)$$

$$=F_X(b)-F_X(a^{-})$$



#### Example

$$P(a \leq X <b)$$

$$\{a \leq X \leq b\}=\{a \leq X < b\} \bigcup \{X=b\}$$

$$P(a \leq X <b)=F_X(b)-F_X(a^{-})-(F_X(b)-F_X(b^{-}))$$

$$=F_X(b^{-})-F_X(a^{-})$$



#### Example

$$F_X(x)=\begin{cases} 0 & \text{if \: }x < -1 \\ 1/2 & \text {if\:} -1 \leq x\leq 0\\ \frac{1+x}{2} & \text{if\:} 0 < x \leq 1 \\ 1 & \text{if\:} x>1\end{cases}$$

$$P(X=-1)=F_X(-1)-F_X(-1^{-})$$

$$=1/2-0=1/2$$

$$P(X<1/2)=P(X \leq 1/2)-P(X=1/2)$$

$$=F_X(1/2)-(F_X(1/2)-F_X(1/2^{-}))$$

$$=F_X(1/2^{-})=3/4$$

$$P(-1/2 < X \leq 1/2)=F_X(1/2)-F_X(-1/2)=1/4$$

$$P(-1/2 < X < 1/2)=P(-1/2 < X \leq 1/2)-P(X=1/2)$$

$$=1/4-(F_X(1/2)-F_X(1/2^{-}))$$

$$=1/4$$



#### Example

$$F_X(x)=\begin{cases} 0 & \text{if\:} x<0 \\ 1-e^{-x} & \text{if\:} x \geq 0\end{cases}$$

$$P(0<X \leq 1)=F_X(1)-F_X(0)$$

$$=1-e^{-1}-0=1-e^{-1}$$

$$P(0<X<1)=P(0<X\leq 1)-P(X=1)$$

$$F_X(1)-F_X(1^{-})=0$$

==Note==

If $$F_X$$ is continuous at a point $$b$$

$$F_X(b)=F_X(b^{-})=F_X(b{+})$$, then 

$$P(X=b)=0$$

------

### Continuous RV

(i) $$S_X$$ is an interval of real line or $$\R$$ or union of interval

(ii) $$F_X$$ is a continuous function

(iii) $$F_X(x)=\int_{-\infty}{x}f_x(t)dt$$

where $$f_x$$ is called the probability density function of $$x$$

It means that for any number $$b$$

$$P(X=b)=F_X(b)-F_X(b^{-})=0$$

## Discussion 6

![image-20241102181133756](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102181133756.png)

a) $$N$$ as a discrete RV

$$A:\{1 \leq N \leq 3\}$$

$$P[N=2|A]=\frac{P[N=2 \bigcap A]}{P[A]}=\frac{P[N=2]}{P[A]}=\frac{P(N=2)}{P[N=1]+P[N=2]+P[N=3]}$$

$$P[A|N=2]=1$$

b) $$0<P(B)<1$$

Given $$P[N=2|B]>P[N=2]$$

S.T. $$P[N=2|B^c]< P(N=2)$$

Proof by contradiction

Suppose that

$$P[N=2|B^c] \geq P[N=2]$$

$$P[N=2]=P[N=2|B]P[B]+P[N=2|B^c]P[B^c]$$

where $$P[N=2|B]>P[N=2], P[N=2|B^c] \geq P[N=2]$$

$$P[N=2] > P[N=2]P[B]+P[N=2]P[B^c]$$

$$=P[N=2][P[B]+P[B^c]]$$

$$P[N=2]>P[N=2]$$

so we arrive at contradiction

$$P[N=2|B^c] < P[N=2]$$
![image-20241102181920771](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102181920771.png)

$$A:$$ Event where webpage is listed first

$$B:$$ Event where webpage is clocked

$$P[A]=p, P[A^c]=1-p$$

$$P[B|A]=q_1, P[B|A^c]=q_2$$

a) $$P[B]=P[B|A]P[A]+P[B|A^c]P[A^c]$$

$$P[B]=q_1p+q_2(1-p)$$

b) $$P[A|B]=\frac{P[B|A]P[A]}{P[B]}$$

$$P[A|B]=\frac{q_1p}{q_1p+q_2(1-p)}$$

c) $$P[A^c|B^c]=\frac{P[B^c|A^c]P[A^c]}{P[B^c]}$$

$$=\frac{(1-P[B|A^c])P[A^c]}{P[B^c]}$$

$$=\frac{(1-q_2)(1-p)}{1-(q_1p+q_2(1-p))}$$

d) If $$A \perp B$$ then

$$P[A\bigcap B]=P[A]P[B]$$

$$P[A|B]P[B]=P[q_1p+q_2(1-p)]$$

$$\frac{q_1p}{P[B]}P[B]=P[q_1p+q_2(1-p)]$$

$$q_1p=q_qp^2+q_2(1-p)p$$

$$q_1p-q_1p^2=q_2(1-p)p$$

$$(q_1-q_2)(1-p)=0$$

$$q_1=q_2$$

![image-20241102182722102](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102182722102.png)

|                        | Dependent             | Independent          |
| ---------------------- | --------------------- | -------------------- |
| Repetition allowed     | $$n^k$$               | $$\binom{n+k-1}{k}$$ |
| Repetition not allowed | $$\frac{n!}{(n-k)!}$$ | $$\binom{n}{k}$$     |

Urn 1: 1R, 4G

Urn 2: 3R, 2G

Total number possible wats to$$=\binom{5}{2}\binom{5}{2}=10 \cdot 10=100$$

i) You pick 2 green balls and 2 red balls from urn 1 and urn 2

$$=\binom{4}{2}\binom{3}{2}$$

$$=6 \cdot 3=18$$

ii) You pick 1 green and 1 red from urn

$$=1 \cdot \binom{4}{1} \binom{3}{1} \binom{2}{1}$$

$$=4 \times 3 \times 2$$

$$=24$$

number of possible ways to pick 2G&2R=18+24=42

$$P[G=2,R=2]=\frac{42}{100}$$

b) maximum number of transition in a string (binary) of length $$n=(n-1)$$

01010

10101

If the first bit is fixed, number of $$k \leq (n-1)$$ transitions $$=\binom{n-1}{k}$$

$$=2 \binom{n-1}{k}$$

### Cumulative distribution function (CDF)

CDF returns the probability that a RV $$X$$ is less than or equal to a value $$x$$

$$F_X(x)=P[X \leq x]$$

CDF can be defined for both discrete and non-discrete RV's

Properties:

1. Normalization

   $$F_X(-\infty)=0, F_X(\infty)=1$$

2. Non-negativity

   $$F_X(x)$$ is non-decreasing positive function of $$x$$

3. For $$b \geq a$$

   $$F_X(b)-F_X(a)=P[a<X \leq b]$$

4. For discrete RV's, CDF is piecewise constant function

![image-20241102184859050](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102184859050.png)

$$Y:$$ the number of heads - the number of tails

$$N=3$$

Let, $$n_H,n_T$$ be number of head and tails

$$Y=n_H-n_T$$

$$Y=n_H-(N-n_H)=2n_H-N$$

| $$n_H$$  | 0    | 1    | 2    | 3    |
| -------- | ---- | ---- | ---- | ---- |
| $$Y$$    | -3   | -1   | 1    | 3    |
| $$P[Y]$$ | 1/8  | 3/8  | 3/8  | 1/8  |

![image-20241102185113828](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102185113828.png)

b) $$P[|Y|<y]=P[-y < Y < y]$$

$$=F_Y(y^{-}) -F_Y(-y)$$

where $$F_Y(y^{-})=\lim_{h \downarrow 0}F_X(y-h)$$

![image-20241102185230804](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102185230804.png)

a,b) $$\Omega=\{(x,y):x^2+y^2 \leq 2^2\}$$

$$R=\sqrt{x^2+y^2}$$

$$S_R\in \{0,2\}$$

![image-20241102185408129](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102185408129.png)

c) $$P[A]=P[R \leq 1/4]=\frac{\text{Area \: of \: bulls \: eye}}{\text{total \: area}}$$

$$=\frac{\pi (1/4)^2}{\pi (2)^2}$$

$$=1/64$$

d) $$F_R(r)=P(R\leq r)=\frac{\pi r^2}{\pi 2^2}=\frac{r^2}{4}$$

![image-20241102185559624](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102185559624.png)

## Week 7 Session 1

Cumulative distribution function (CDF)

$$F_X(x)=P(X \leq x)$$ for all $$x\in \R$$

Properties:

1.  $$F_X(x)$$ is a non-decreasing function

2. $$\lim_{x \rightarrow \infty}F(X)=1, \lim_{x\rightarrow -\infty}F(X)=0$$

3. Right continuous:

   $$\lim_{h \downarrow 0}F_X(b+h)=F_X(b)$$

4. Let $$a<b$$

   $$P(a<X \leq b)=F_X(b)-F_X(a)$$

5. $$P(X=b)=F_X(b)-F_X(b^{-})$$

   $$F_X(b^{-})=\lim_{h \downarrow 0}F_X(b-h)$$

Continuous RV

1. $$S_{X}$$ is an interval of real line or $$\R$$ or union of interval

2. $$F_X$$ is a continuous function 

   $$F_X(b)=F_X(b^{+})=F_X(b^{-})$$ for all real number $$b$$

3. $$F_X(x)=\int_{-\infty}^{x}f_x(t)dt$$

   where $$f_x$$ is called the probability density function of $$X$$

   

$$P(X=b)=F_X(b)-F_X(b^{-})=0$$

$$X$$ is the lifetimes of a device measured in seconds

$$S_X=[0,\infty)$$

$$P(X=-10)=P(\phi)=0$$

$$X$$ is a continuous RV

$$P(X=0.33333333...)=0$$

$$F_X(x)=\int_{-\infty}^{x}f_x(t)dt$$

### Results

1. For all $$x$$ where $$F_X$$ is differentiable

   $$\frac{dF_X(x)}{dx}=f_X(x)$$ is the rate of change of CDF

   2. $$f_X(x) \geq 0$$ for all $$x \in \R$$

      $$f_X(x)$$ does not have to be $$\leq 1$$

      ![image-20241011103427494](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011103427494.png)

      3. $$P(x<X \leq x+h)=F_X(x+h)-F_X(x)$$

         $$=\frac{F_X(x+h)-F_X(x)}{h}h$$

         $$\approx f_X(x)h$$

         $$f_X(x) \approx \frac{P(x<X \leq x+h)}{h}$$

      4. $$P(a<X\leq b)=F_X(b)-F_X(a)$$ where $$a<b$$

         $$=\int_{-\infty}^{b}f_X(t)dt-\int_{-\infty}^{a}f_X(s)ds$$

         $$=\int_{a}^{b}f_X(t)dt$$

         

         Discrete RV

         $$Z$$ is a discrete RV $$P_Z$$

         $$P(a<Z\leq b)=\sum_{a< Z \leq b}P_Z(z)$$

         

         $$P(a<X\leq b)=\int_{a}^{b}f_X(t)dt$$

         $$P(a \leq X \leq b)=P(a<X\leq b)+P(X=a)$$

         $$=\int_{a}^{b}f_X(t)dt$$

         

         $$P(a \leq X <b)=P(a \leq X \leq b)-P(X=b)$$

         $$=\int_{a}^{b}f_X(t)dt$$

         $$P(\{X \in (1,2)\} \bigcup \{X \in {3,4}\})$$

         $$=\int_{1}^{2}f_X(t)dt+\int_{3}^{4}f_X(t)dt$$

         In general, for any subset $$B$$ of the real line

         $$P(X \in B)= \int_{B}f_X(t)dt$$

         ![image-20241011112259320](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011112259320.png)

         $$Z$$ Discrete RV $$P_Z$$

         $$P(Z \in B)=\sum_{Z \in B}P_Z(z)$$

      5. $$\int_{-\infty}^{\infty}f_X(t)dt=1$$

         

         For Discrete RV

         $$\sum_{Z \in \R}P_Z(z)=1$$

         

         $$\int_{-\infty}^{\infty}f_X(t)dt=\lim_{a \rightarrow \infty}\int_{-a}^{a}f_X(t)dt$$

         $$=\lim_{a \rightarrow \infty}(F_X(a)-F_X(-a))$$

         $$=\lim_{a \rightarrow \infty}F_X(a)-\lim_{a \rightarrow \infty}F_X(-a)$$

         $$=1-\lim_{c \rightarrow -\infty}F_X(c)$$

         $$=1$$

         

         #### Example

         Uniform RV over interval $$[a,b], a< b$$ 

         $$f_X(x)=\begin{cases} \frac{1}{b-a} & \text{if \: } a \leq x \leq b\\ 0 & \text{otherwise}\end{cases}$$

      ![image-20241011112921036](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011112921036.png)

      CDF: $$F_X(x)=\int_{-\infty}^{x}f_X(t)dt$$

      Case 1:  $$x<a$$

      $$F_X(x)=0$$

      Case 2: $$a \leq x \leq b$$

      $$F_X(x)=\int_{-\infty}^{x}f_X(t)dt$$

      $$=\int_{a}^{x}\frac{1}{b-a}dt$$

      $$=\frac{x-a}{b-a}$$

      Case 3: $$x>b$$

      $$F_X(x)=\int_{-\infty}^{x}f_X(t)dt=1$$

      ![image-20241011113414912](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011113414912.png)

      

      #### Example

      $$f_X(x)=\begin{cases} \lambda e^{-\lambda x} & \text{if \: } a \leq x \leq b\\ 0 & \text{otherwise}\end{cases}$$

      Here, $$\lambda$$ is a positive parameter

      exponential density with parameter $$\lambda$$

      $$P(X>1)=\int_{1}^{\infty}f_X(t)dt$$

      $$=\int_{1}^{\infty}\lambda e^{-\lambda x} dt$$

      $$=\lambda \frac{e^{-\lambda t}}{-\lambda} |_{1}^{\infty}$$

      $$=e^{-\lambda }$$

      for $$x>0$$

      $$P(X>x)=\int_{x}^{\infty}\lambda e^{-\lambda t}dt$$

      $$=e^{-\lambda x}$$

      $$F_X(x)=\begin{cases} 0 & x<0 \\ 1-e^{-\lambda x} & x \geq 0\end{cases}$$

      

      #### Laplacian Random Variable

      $$f_X(x)=ce^{-\alpha |x|}, x\in \R$$ where $$c>0, \alpha>0$$ are constants

      ![image-20241011120629683](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011120629683.png)

      $$\int_{-\infty}^{\infty}ce^{-\alpha |x|}dx=1$$

      $$2\int_{0}^{\infty}ce^{-\alpha |x|}dx=1$$

      $$2c\int_{0}^{\infty}e^{-\alpha x}dx=1$$

      $$\frac{2c}{\alpha}=1$$

      $$P(|X|<v)=P(-v < X < v)$$ where $$v>0$$

      $$=\int_{-v}^{v}ce^{-\alpha |x|}dx$$

      $$=2\int_{0}^{v}ce^{-\alpha |x|}dx$$

      $$=2c\int_{0}^{v}e^{-\alpha x}dx$$

      $$=1-e^{-\alpha v}$$

      $$2c=\alpha$$

### Standard Gaussian PDF (Standard normal pdf)

$$f_X(x)=\frac{1}{\sqrt{2 \pi}}e^{-\frac{x^2}{2}}, x\in \R$$

Bell-shaped curve symmetric around $$x=0$$

![image-20241011121220424](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011121220424.png)

Gaussian pdf with parameters $$m$$ and $$\sigma^2$$

$$f_X(X)=\frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{(x-m)^2}{2 \sigma^2}}, x \in \R$$

![image-20241011121341932](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011121341932.png)

------

$$F_X(x)=P(X \leq x)$$

$$C$$ is some event with $$P(C)>0$$

$$F_X(x|C)$$ is the conditional CDF of $$X$$ given $$C$$

$$F_X(x|C)=P(X \leq x|C)$$

$$\frac{dF_X(x)}{dx}=f_X(x)$$ (PDF)

$$\frac{dF_X(x|C)}{dx}=f_X(x|C)$$ (conditional density function)



#### Example

$$X$$ is a continuous RV

$$C=\{x>1\}$$

$$F_X(x|C)=P(X \leq x| C)$$

$$=\frac{P(X \leq x \bigcap C)}{P(C)}$$

$$=\frac{P(X \leq x \bigcap X>1)}{P(X>1)}$$

$$F_X(x|C)=\begin{cases} \frac{0}{1-F_X(1)} & x\leq 1\\ \frac{F_X(x)-F_X(1)}{1-F_X(1)} & x>1\end{cases}$$

$$f_X(x|C)=\begin{cases} 0 & x \leq 1 \\ \frac{f_X(x)}{1-F_X(1)} & x>1\end{cases}$$

$$\int_{1}^{\infty}f_X(x|C)dx=\frac{1}{1-F_X(1)}\int_{1}^{\infty}f_X(x)dx$$

$$=\frac{1-F_X(1)}{1-F_X(1)}=1$$

1. $$0 \leq F_X(x) \leq 1$$

   $$0 \leq F_X(x|C)\leq 1$$

2. $$\lim_{x \rightarrow \infty}F_X(x|C)=1$$

   $$\lim_{x \rightarrow -\infty}F_X(x|C)=0$$

3. $$F_X(x|C)$$ is non-decreasing and right continuous function of $$x$$
4. $$C_1, C_2, ... C_n$$ is a partition of $$\Omega$$

$$P(X \leq x)=\sum_{i=1}^{n}P(X \leq x |C_i)P(C_i)$$



Discrete RV

$$F_X(x)=\sum_{i=1}^{n}F_X(x|C_i)P(C_i)$$

$$f_X(x)=\sum_{i=1}^{n}f_X(x|C_i)P(C_i)$$

------

#### Example

Communication system

Bit 0 with probability $$p$$ or 1 with probability $$1-p$$

0 is sent a $$-v$$ voltage signal

1 is sent a $$+v$$ voltage signal

Receiver get signal plus noise

$$Y=X+N$$

where $$Y$$ is the received signal, $$X$$ is the transmitted signal, $$N$$ is the noise

$$P(X=+v)=p$$

$$P(X=-v)=1-p$$

$$N$$ is a standard Gaussian RV

$$f_N(x)=\frac{1}{\sqrt{2 \pi}}e^{-\frac{x^2}{2}}$$

Independence assumption: For any number $$a,b$$ that $$\{X=a\}$$ and $$\{N \leq b\}$$ are independent

Find CDF of the received signal $$Y$$
$$F_Y(y)=P(Y \leq y)$$

$$=P(Y\leq y|X=+v)P(X=+v)+P(Y\leq y|X=-v)P(X=-v)$$

$$P(Y\leq y|X=+v)=P(X+N \leq y | X=+v)$$

$$=P(+v+N \leq y | X=+v)$$

$$=P(N \leq y-v|X=+v)$$

$$=P(N \leq y-v)$$

$$=F_N(y-v)$$

$$=\int_{-\infty}^{y-v}f_N(t)dt$$

$$=\int_{-\infty}^{y-v}\frac{1}{\sqrt{2 \pi}}e^{-\frac{x^2}{2}}dt$$

$$P(Y\leq y|X=-v)=\int_{-\infty}^{y+v}\frac{1}{\sqrt{2 \pi}}e^{-\frac{x^2}{2}}dt$$

$$F_Y(y)=pF_N(y-v)+(1-p)F_N(y+v)$$

PDF of $$Y$$

$$f_Y(y)=\frac{dF_Y(y)}{dy}=pf_N(y-v)+(1-p)f_N(y+v)$$

$$=\frac{1}{\sqrt{2 \pi}} [p e^{-\frac{(y-v)^2}{2}} + (1-p)e^{-\frac{(y+v)^2}{2}} ] $$

------

### Expected value

Discrete $$Z$$

$$E[Z]=\sum z P_Z(z)$$



$$E[X]=\int_{-\infty}^{\infty}x f_X(x)dx$$

#### Example

$$X\sim$$ Uniform $$[a,b]$$

$$f_X(x)=\begin{cases} \frac{1}{b-a} & a \leq x \leq b \\ 0 & \text{otherwise}\end{cases}$$

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx$$

$$=\frac{1}{b-a}\int_{a}^{b}xdx$$

$$=\frac{1}{b-a}\frac{b^2-a^2}{2}=\frac{b+a}{2}$$

![image-20241011132058515](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241011132058515.png)

$$X \sim \text{exp} (\lambda)$$ 

$$f_X(x)=\begin{cases} \lambda e^{-\lambda x} & x \geq 0\\ 0 & x<0\end{cases}$$

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx$$

$$=\int_{0}^{\infty}x \lambda e^{-\lambda x}dx$$

$$=-xe^{-\lambda x}|^{\infty}_{0}+\int_{0}^{\infty}e^{-\lambda x}dx$$

$$=0-\frac{e^{-\lambda x}}{\lambda} |^{\infty}_{0}$$

$$=\frac{1}{\lambda}$$



Integration by parts:

$$\int u dv =uv- \int vdu$$

------

## Week 8 Session 1

### Continuous RVs

$$F_X(x)=\int_{-\infty}^{x}f_X(t)dt=P(X\leq x)$$

where $$f_X$$ is called the probability density function of $$X$$

Probability density function $$f_X$$

1. $$f_X(x)=\frac{dF_X(x)}{dx}$$ where $$F_X(x)$$ is differentiable

2. For small $$h>0$$

   $$f_X(x)\cdot h \approx P(x<X<x+h)$$

3. $$P(X\in B)=\int_{B}f_X(t)dt$$ 

   where $$B$$ is any subset of $$\R$$

Expected value

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx$$



Discrete:

$$E[X]=\sum xP_X(x)$$

------

#### Example

$$X$$ is a continuous RV with $$f_x$$ symmetric about 0

$$f(x)=f(-x)$$ for all $$x\in \R$$

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx=0$$

$$=\int_{-\infty}^{0}xf_X(x)dx+\int_{0}^{\infty}xf_X(x)dx$$

Let $$x=-u$$

$$=\int_{\infty}^{0}(-u)f_X(-u)(-du)+\int_{0}^{\infty}xf_X(x)dx$$

$$=-\int_{0}^{\infty}uf_X(-u)du+\int_{0}^{\infty}xf_X(x)dx$$

as $$f_X(u)=f_X(-x)$$

$$-\int_{0}^{\infty}uf_X(-u)du=-\int_{0}^{\infty}xf_X(x)dx$$

$$E[X]=0$$

as long as $$\int_{0}^{\infty}xf_X(x)dx$$ is finite

If $$f_X$$ is symmetric around 0 and $$\int_{0}^{\infty}xf_X(x)dx$$ is finite

then $$E[X]=0$$

------

Standard Normal RV

$$f_X(x)=\frac{1}{\sqrt{2 \pi}}e^{-\frac{x^2}{2}}$$

$$E[X]=0$$ since $$f(x)=f(-x)$$ and $$\int_{0}^{\infty}xf_X(x)dx < \infty$$

------

#### Example

Symmetric $$f_X$$ around $$m$$

$$f_X(m+x)=f_X(m-x)$$ for all $$x \in \R$$

$$E[X]-m=\int_{-\infty}^{\infty}xf_X(x)dx-m\int_{-\infty}^{\infty}f_X(x)dx$$

$$=\int_{-\infty}^{\infty}(x-m)f_X(x)dx$$

$$=\int_{-\infty}^{m}(x-m)f_X(x)dx+\int_{m}^{\infty}(x-m)f_X(x)dx$$



For $$\int_{-\infty}^{m}(x-m)f_X(x)dx$$

Let $$m-x=t$$

when $$x=-\infty, t=\infty$$

when $$x=m, t=0$$



For $$\int_{m}^{\infty}(x-m)f_X(x)dx$$

Let $$x-m=t$$

when $$x=m, t=0$$

when $$x=\infty, t=\infty$$



$$=\int_{\infty}^{0}(-t)f_X(m-t)(-dt)+\int_{0}^{\infty}tf_X(m+t)dt $$

$$=-\int_{\infty}^{0}tf_X(m-t)(-dt)+\int_{0}^{\infty}tf_X(m+t)dt $$

as $$f_X(m-t)=f_X(m+t)$$

$$=0$$



as long as $$\int_{0}^{\infty}tf_X(m+t)dt=\int_{m}^{\infty}(x-m)f_X(x)dx < \infty$$

$$E[X]-m=0$$

$$E[X]=m$$



If $$f_X$$ is symmetric around $$m$$ and $$\int_{m}^{\infty}(x-m)f_X(x)dx$$, then $$E[X]=m$$



Gaussian density with parameters $$m, \sigma^2$$

$$f_X(x)=\frac{1}{\sqrt{2 \pi \sigma^2}}e^{-\frac{(x-m)^2}{2 \sigma^2}}$$

$$f_X(m+t)=f_X(m-t)$$ for $$t\in \R$$

$$E[X]=m$$ since $$\int_{m}^{\infty}(x-m)f_X(x)dx < \infty$$



#### Example

$$X$$ is a continuous RV with $$f_X$$

$$X$$ is a non-negative RV

$$P(X\geq 0)=1$$

$$P(X<0)=0$$

$$\int_{-\infty}^{0}f_X(dx)dx=0$$

$$f_X(x)=0$$ for all $$x<0$$



Show that $$E[X]=\int_{0}^{\infty}(1-F_X(t))dt$$

Proof:

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx$$

$$=\int_{0}^{\infty}xf_X(x)dx$$ 

$$=\int_{0}^{\infty} [\int_{0}^{x} 1 dt] f_X(x)dx$$

$$=\int_{0}^{\infty} \int_{0}^{x} 1 f_X(x)dt dx$$

![image-20241018120805492](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241018120805492.png)

$$=\int_{0}^{\infty} [\int_{t}^{\infty} 1 f_X(x)dx] dt$$

$$=\int_{0}^{\infty} P(X>t) dt$$

Recall:

$$\int_{a}^{b}f_X(x)dx=P(a<X<b)$$

$$=\int_{0}^{\infty}(1-F_X(t))dt$$



#### Example

Exponential RV

$$f_X(x)=\begin{cases} \lambda e^{-\lambda x} & \text{for\:} x \geq 0 \\ 0 & \text{for\:} x<0 \end{cases}$$

$$E[X]=\int_{0}^{\infty}(1-F_X(t))dt$$

$$F_X(t)=1-e^{-\lambda t}$$

$$E[X]=\int_{0}^{\infty}e^{-\lambda t}dt$$

$$=\frac{-1}{\lambda}e^{-\lambda t} |^{\infty}_{0}$$

$$=\frac{1}{\lambda}$$

------

#### Example

$$X$$ is a standard Gaussian RV

$$f_X(x)=\frac{1}{\sqrt{2 \pi}}e^{-\frac{x^2}{2}}$$

$$E[X]=0$$
$$Y=X^2$$

Find the CDF and the pdf of $Y$

$$F_Y(y)=P(Y \leq y)$$

$$=P(X^2 \leq y)$$

$$=\begin{cases} 0 & \text{if\:} y<0 \\ P(X^2 \leq y) & \text{if\:} y \geq 0\end{cases}$$

$$P(X^2 \leq y)=P(-\sqrt{y} \leq X \leq \sqrt{y})$$

$$=\int_{-\sqrt{y}}^{\sqrt{y}}f_X(x)dx$$

$$=F_X(\sqrt{y})-F_X(-\sqrt{y})$$

$$F_Y(y)=\begin{cases} 0 & \text{if\:} y<0 \\ F_X(\sqrt{y})-F_X(-\sqrt{y}) & \text{if\:} y \geq 0\end{cases}$$

$$f_Y(y)=\begin{cases} 0 & \text{if\:} y<0 \\ \frac{1}{2\sqrt{y}}f_X(\sqrt{y})+\frac{1}{2\sqrt{y}}f_X(-\sqrt{y}) & \text{if\:} y \geq 0\end{cases}$$



If $$Y=g(X)$$

$$F_Y(y)=P(Y \leq y)$$

$$=P(g(X)\leq y)$$



Theorem:

If $$X$$ is continuous RV with $$f_X$$ and $$Y=g(X)$$

$$E[Y]=\int_{-\infty}^{\infty}g(x)f_X(x)dx$$



Recap:

$$X,Y$$ are discrete RV

$$Y=g(X)$$

$$E[Y]=\sum_{x}g(x)P_X(x)$$



#### Example

$$Y=\cos(\omega t+ \theta)$$

where $$\theta \sim $$ uniform $$(0,2 \pi)$$ and $$\omega, t$$ are constant

![image-20241018123307779](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241018123307779.png)

$$f(\theta)=\frac{1}{2 \pi}$$

$$E[\theta]=\pi$$

$$E[Y]=\int_{-infty}^{\infty}g(\theta)f_{\theta}\theta d\theta$$

$$=\int_{0}^{2 \pi} \cos(\omega t+ \theta) \frac{1}{2 \pi} d\theta$$

$$=\frac{1}{2\pi} \sin(\omega t+ \theta)|^{2 \pi}_{0}$$

$$=\frac{1}{2\pi} [\sin(\omega t+ 2\pi)-sin(\omega t+0)]$$

$$=0$$



$$Z=\begin{cases} 1 &\text{if\:} \theta \in [\pi, 2\pi] \\ 0 & \text{if\:} \theta \in (0,\pi)\end{cases}$$

$$P_Z(1)=P(Z=1)$$
$$=P(\theta \in [\pi, 2\pi])$$

$$=\int_{\pi}^{2\pi}\frac{1}{2\pi}d\theta$$

$$=1/2$$

$$P_Z(0)=1/2$$

$$E[Z]=0\cdot 1/2 + 1\cdot 1/2=1/2$$

$$E[Z]=\int_{-\infty}^{\infty}g(\theta)f_{\theta}(\theta)d\theta$$

where $$g(\theta)=\begin{cases} 1 & \text{if\:} \theta \in [\pi,2\pi] \\ 0 &\text{otherwise}\end{cases}$$

$$=\int_{0}^{2\pi}g(\theta)f_{\theta}(\theta)d\theta$$

$$=\int_{0}^{\pi}0 \cdot f_\theta(\theta)d\theta + \int_{\pi}^{2\pi}1 \cdot f_\theta(\theta)d\theta$$

$$=\frac{1}{2\pi}d\theta=1/2$$



Properties of Expectation of continuous RVs

1. If $$X$$ is a non-negative RV (i.e., $$f_X(x)=0$$ for $$x<0$$)

   then $$E[X] \geq 0$$

​	$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx=\int_{0}^{\infty}xf_X(x)dx \geq 0$$

2. $$E[X+c]=E[X]+c$$

   where $$c$$ is a constant

   Proof: $$Y=X+c$$

   $$E[Y]=\int_{-\infty}^{\infty}(x+c)f_X(x)dx$$

   =$$\int_{-\infty}^{\infty}xf_X(x)dx+c\int_{-\infty}^{\infty}f_X(x)dx$$

   $$=E[X]+c$$

3. $$E[cX]=cE[X]$$

   Proof: $Y=<span class="md-search-hit">cX</span>$
   $$E[Y]=\int_{-\infty}^{\infty}cxf_X(x)dx$$

   $$=cE[X]$$

4. $$E[aX+b]=aE[x]+b$$

5. $$Z=ag(X)+bh(X)+c$$

   where $$a,b,c$$ are constants, $$g,h$$ are functions

   $$E[Z]=aE[g(X)]+bE[h(X)]+c$$

   Proof: $$E[Z]=E[ag(X)+bh(X)+c]$$

   Let $$ag(X)+bh(X)+c=Y=k(X)$$

   $$=\int_{-\infty}^{\infty}k(X)f_X(x)dx$$

   $$=\int_{-\infty}^{\infty}(ag(X)+bh(X)+c)f_X(x)dx$$

   $$=\int_{-\infty}^{\infty}ag(x)f_X(x)dx+\int_{-\infty}^{\infty}bh(x)f_X(x)dx+\int_{-\infty}^{\infty}cf_X(x)dx$$

   $$=aE[g(x)]+bE[h(x)]+c$$

------

#### Example

Travel from point $$A$$ to point $$B$$ 

Travel time is a non-negative RV with pdf $$f$$
I leave at $$t=0$$, my appointment is at $$t=60 min$$

If I arrive $$s$$ minutes early, my cost is $$cs$$

If I arrive $$s$$ minutes late, my cost is $$ds$$

Find the expected value of cost

$$X=$$ travel time

$$\text{Cost}(X) =\begin{cases} d(X-60) & \text{if\:} X>60 \\ c(60-X) & \text{if\:} X<60 \\ 0 & \text{if\:}X=60\end{cases}$$

$$E[\text{Cost}(X)]=\int_{-\infty}^{\infty}\text{cost}(x)f_X(x)dx$$

$$=\int_{0}^{60}c(60-x)f_X(x)dx+\int_{60}^{\infty}d(x-60)f_X(x)dx$$

------

Variance of $$X$$

Discrete: 

$$Var[X]=E[(X-m_X)^2]=E[X^2]-(m_X)^2$$

Continuous: 

$$Var[X]=E[(X-m_X)^2]=E[X^2]-(m_X)^2$$

$$Var[X]=E[(X-m_X)^2]=\int_{-\infty}^{\infty}(x-m_X)^2f_X(x)dx$$

$$n^{th}$$ moment of $$X$$

$$E[X^n]=\int_{-\infty}^{\infty}x^nf_X(x)dx$$

Standard Deviation: $$+\sqrt{Var(X)}$$



#### Example

$$X \sim$$ Uniform $$[a,b]$$   $$(a<b)$$

$$f_X(x)=\begin{cases}\frac{1}{b-a} & \text{if\:} x \in [a,b] \\ 0 & \text{if\:} x \notin [a,b]\end{cases}$$

![image-20241018185554388](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241018185554388.png)

$$E[X]=\frac{b+a}{2}$$

$$Var[X]=E[(X-m_X)^2]$$

$$=\int_{-\infty}^{\infty}(x-\frac{a+b}{2})^2 f_X(x)dx$$

$$=\frac{1}{b-a}\int_{a}^{b}(x-\frac{a+b}{2})dx$$

$$=\frac{(b-a)^2}{12}$$

Standard deviation: $$\frac{|b-a|}{\sqrt{12}}$$



#### Example

Standard Gaussian

$$f_Y(y)=\frac{1}{\sqrt{2 \pi}}e^{-\frac{y^2}{2}}$$

$$E[Y]=0$$

$$Var[Y]=E[(Y-0)^2]$$

$$=\int_{-\infty}^{\infty}y^2 \frac{1}{\sqrt{2 \pi}} e^{-\frac{y^2}{2}}dy$$

$$=1$$

------

Gaussian with parameters $$m, \sigma^2$$

$$f_X(x)=\frac{1}{\sqrt{2 \pi \sigma^2}}e^{-\frac{(x-m)^2}{2\sigma^2}}$$

$$E[X]=m$$

$$Var[X]=E[(X-m)^2]=\sigma^2$$

$$=\int_{-\infty}^{\infty}(x-m)^2\frac{1}{\sqrt{2 \pi \sigma^2}}e^{-\frac{(x-m)^2}{2\sigma^2}}dx$$

Let $$\frac{x-m}{\sigma}=y$$

$$x-m=\sigma y$$

$$dx=\sigma dy$$

$$=\int_{-\infty}^{\infty} \sigma^2 y^2 \frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{y^2}{2}} \sigma dy$$

$$=\sigma^2 \int_{-\infty}^{\infty} y^2 \frac{1}{\sqrt{2 \pi}} e^{-\frac{y^2}{2}} dy$$

$$=\sigma^2$$

------

#### Example

$$X,f_X$$

(a) $$Y=X+c$$

$$E[Y]=E[X+c]=E[X]+c$$

$$Var[Y]=E[(Y-m_Y)^2]$$

$$=E[(X+c-(m_X+c))^2]$$

$$=E[(X-m_X)^2]$$

$$=Var[X]$$



(b) $$Z=cX$$

$$E[Z]=E[cX]=cE[X]$$

$$Var[Z]=E[(Z-m_Z)^2]$$

$$=E[(cX-cm_X)^2]$$

$$=E[c^2(X-m_X)^2]$$

$$=c^2 E[(X-m_X)^2]$$

$$=c^2Var[X]$$

------

## Week 8 Session 2

Theorem:

If $$X$$ is a continuous RV with $$f_X$$ as its pdf and $$Y=g(x)$$

$$E[Y]=\int_{-\infty}^{\infty}g(x)f_X(x)dx$$

1. $E[aX+b]=aE[X]+b$
2. $$E[ag(x)+bh(x)+c]=aE[g(x)]+bE[h(x)]+c$$

#### Example

$$E[x^3+2x^2+1]=E[X^3]+2E[X^2]+1$$

$$Var[x]=E[(X-m_X)^2]=\int_{-\infty}^{\infty}(X-m_X)^2 f_X(x)dx$$

------

### Exponential RV

$$X \sim \text{exp}(\lambda)$$

$$f_X(x)=\begin{cases} \lambda e^{-\lambda x} & \text{if\:} x \geq 0 \\ 0 & \text{if\:} x<0\end{cases}$$

$$\lambda >0$$ is a paramater

$$F_X(x)=\begin{cases} 1- e^{-\lambda x} & \text{if\:} x \geq 0 \\ 0 & \text{if\:} x<0\end{cases}$$

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx$$

$$=\int_{-\infty}^{\infty} x \lambda e^{-\lambda x} dx$$

$$=\frac{1}{\lambda}$$

$$X$$ is a non-negative RV

$$E[X]=\int_{0}^{\infty}(1-F_X(t))dt$$

$$=\int_{0}^{\infty}e^{-\lambda t}dt$$

$$=\frac{-1}{\lambda} e^{-\lambda t}|^{\infty}_{0}$$

$$=\frac{1}{\lambda}$$



$$E[X^2]=\int_{-\infty}^{\infty} x^2 f_X(x)dx$$

$$=\int_{0}^{\infty} x^2 \lambda e^{-\lambda x}dx$$

Say $$y=\lambda x$$ and $$dy=\lambda dx$$

$$=\int_{0}^{\infty}\frac{y^2}{\lambda^2}e^{-y}dy$$

$$=\frac{1}{\lambda^2} \int_{0}^{\infty}y^2 e^{-y} dy$$

Integration by parts: $$y^2=u$$ and $$e^{-y}dy=dv$$

$$=\frac{1}{\lambda^2}[-y^2e^{-y}|^{\infty}_{0}-\int_{0}^{\infty}2y(-e^{-y})dy]$$

$$=\frac{1}{\lambda^2}[0+2\int_{0}^{\infty}ye^{-y}dy]$$

$$\int_{0}^{\infty}ye^{-y}dy$$ is the expected value of an exponential RV with $$\lambda=1$$

$$\lim_{y \rightarrow \infty} y^2 e^{-y} =0$$

$$\lim_{y \rightarrow \infty} \frac{y^2}{e^y} = \lim_{y \rightarrow \infty} \frac{2y}{e^y}=\lim_{y \rightarrow \infty} \frac{2}{e^y}=0$$

$$=\frac{2}{\lambda^2} \cdot 1$$

$$E[X^2]=\frac{2}{\lambda^2}, E[X]=\frac{1}{\lambda}$$

$$Var[X]=E[X^2]-(E[X])^2$$

$$=\frac{2}{\lambda^2}-\frac{1}{\lambda^2}$$

$$=\frac{1}{\lambda^2}$$

------

Exercise: 

$$X \sim \text{exp}(\lambda)$$

$$E[X^n]=\frac{n}{\lambda}E[X^{n-1}]$$ for $$n \geq 2$$

$$E[X^n]=\frac{n!}{\lambda^n}$$

------

#### Example

$$X \sim \text{exp}(\lambda)$$

waiting time until the arrival of the first customer at a store (time in seconds)

1. $$P(X>10)=1-P(X\leq 10)$$

   $$=1-F_X(10)$$

   $$=1-(1-e^{-\lambda 10})$$

   $$=e^{-\lambda 10}$$

2. Given that we have already waited for 2 seconds, what is the probability that we we will wait at least 10 seconds for the first customer?

   $$P(X\geq 12|X>2)=\frac{P(X\geq 12 \bigcap X>2)}{P(X>2)}$$

   $$=\frac{P(X\geq 12)}{P(X>2)}$$

   $$=\frac{P(X>12)+P(X=12)}{P(X>2)}$$

   $$=\frac{e^{-12 \lambda}}{e^{-2\lambda}}$$

   $$=e^{-10\lambda}$$

   

Suppose $$t>0, s>0$$

$$P(X>t+s|X>s)=\frac{P(X>t+s\bigcap X>s)}{P(X>s)}$$

$$=\frac{P(X>t+s)}{P(X>s)}$$

$$=\frac{e^{-\lambda (t+s)}}{e^{-\lambda s}}=e^{-\lambda t}$$

$$=P(X>t)$$

Property of $$X \sim \text{exp}(\lambda)$$

$$P(X>t+s|X>s)=P(X>t)$$

Memoryless property of exponential RVs

------

### Gaussian RV

Standard Gaussian / Standard Normal

$$Y \sim \mathcal{N}(0,1)$$

$$E[Y]=0$$

$$Var[Y]=1$$

$$f_Y(y)=\frac{1}{\sqrt{2 \pi}}e^{-\frac{y^2}{2}}$$

Gaussian RV with mean $$m$$, variance $$\sigma^2$$

$$X \sim \mathcal{N}(m, \sigma^2)$$

$$E[X]=m, Var[X]=\sigma^2$$

$$f_X(x)=\frac{1}{\sqrt{2 \pi \sigma^2}}exp(-\frac{(x-m)^2}{2\sigma^2})$$

------

$$X \sim \mathcal{N}(m, \sigma^2)$$

$$Z=\frac{X-m}{\sigma}$$

$$E[Z]=E[\frac{X-m}{\sigma}]$$

$$=E[\frac{X}{\sigma}-\frac{m}{\sigma}]$$

$$=\frac{1}{\sigma}E[X]-\frac{m}{\sigma}$$

$$=\frac{m}{\sigma}-\frac{m}{\sigma}=0$$

$$Var[Z]=E[(Z-0)^2]$$

$$=E[Z^2]$$

$$=E[\frac{(X-m)^2}{\sigma^2}]$$

$$=\frac{1}{\sigma^2}E[(X-m)^2]$$

$$=\frac{1}{\sigma^2} \sigma^2$$

$$=1$$

CDF of $$Z$$

$$F_Z(z)=P(Z \leq z)$$

$$=P(\frac{X-m}{\sigma} \leq z)$$

$$=P(X \leq m+ \sigma z)$$

$$=F_X(m+ \sigma z)$$



$$f_Z(z)=\frac{dF_Z(z)}{dz}=\frac{d}{dz}F_X(m+ \sigma z)$$

$$=f_X(m+\sigma z) \sigma$$

$$=\frac{1}{\sqrt{2 \pi \sigma^2}} exp (- \frac{(m+\sigma z -m)^2}{2 \sigma^2}) \sigma$$

$$=\frac{1}{\sqrt{2 \pi}}e^{-\frac{z^2}{2}}$$

Standard Normal Density



If $$X \sim \mathcal{N}(m, \sigma^2)$$ and $$Z=\frac{X-m}{\sigma}$$

then $$Z \sim \mathcal{N}(0,1)$$



$$Y \sim \mathcal{N}(0,1)$$

$$F_Y(y)=P(Y \leq y)=\int_{-\infty}^{y}\frac{1}{\sqrt{2 \pi}}e^{-\frac{t^2}{2}} dt$$

Denote by $$\phi (y)$$ : CDF of a standard normal RV evaluated at $$y$$



$$X \sim \mathcal{N}(m, \sigma^2)$$

$$F_X(x)=P(X\leq x)$$

$$=P(\frac{X-m}{\sigma} \leq \frac{x-m}{\sigma})$$

$$=P(Z \leq \frac{x-m}{\sigma})$$

$$=\phi(\frac{x-m}{\sigma})$$



$$P(a<X\leq b)=P(\frac{a-m}{\sigma}<\frac{X-m}{\sigma} \leq \frac{b-m}{\sigma})$$

$$=P(\frac{a-m}{\sigma}<Z \leq \frac{b-m}{\sigma})$$

$$=\phi(\frac{b-m}{\sigma})-\phi(\frac{a-m}{\sigma})$$

Recall: $$P(a<Y \leq b)=F_Y(b)-F_Y(a)$$



$$P(X>b)=P(\frac{X-m}{\sigma}>\frac{b-m}{\sigma})$$

$$=P(Z > \frac{b-m}{\sigma})$$

$$=1-\phi(\frac{b-m}{\sigma})$$

------

### Properties of $$\phi$$ (the standard Gaussian CDF)

$$\phi(y)=\int_{-\infty}^{y}\frac{e^{-\frac{t^2}{2}}}{\sqrt{2 \pi}}dt$$

![image-20241021132938545](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021132938545.png)

$$Q(y)=\int_{y}^{\infty}\frac{e^{-\frac{t^2}{2}}}{\sqrt{2 \pi}}dt$$

$$\phi(y)+Q(y)=1$$

![image-20241021133036692](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021133036692.png)

$$\phi(0)=Q(0)=1/2$$

$$\phi(-y)=Q(y)$$

------

### Cauchy RV

$$f_X(x)=\frac{1}{\pi} \frac{1}{1+x^2} , -\infty < x < \infty$$

==$$E[X]$$ is not defined==

![image-20241021133236587](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021133236587.png)

$$f_X(x)=f_X(-x)$$

$$E[X]=\int_{-\infty}^{\infty} x f_X(x)dx$$

$$=\int_{-\infty}^{0} \frac{1}{\pi} \frac{1}{1+x^2} dx+ \int_{0}^{\infty} \frac{1}{\pi} \frac{1}{1+x^2} dx$$

$$=- \int_{0}^{\infty} \frac{1}{\pi} \frac{1}{1+x^2} dx +\int_{0}^{\infty} \frac{1}{\pi} \frac{1}{1+x^2} dx$$

$$=-\infty + \infty \implies$$ UNDEFINED



$$\int_{0}^{\infty} \frac{1}{\pi} \frac{1}{1+x^2} dx$$

$$t=1+x^2, 2xdx=dt$$

$$=\frac{1}{\pi} \int_{1}^{\infty} \frac{dt}{2t}$$

$$=\frac{1}{2 \pi} \ln{t}|^{\infty}_{1}$$

$$=\infty$$

------

#### Example

$$X \sim \mathcal{N}(0,1)$$

$$Y =\begin{cases} -10 & \text{if\:} X \leq -1 \\ 0 & \text{if\:} -1<X<1 \\ 10 & \text{if\:} X \geq 1\end{cases}$$

PMF of Y in terms of the standard Gaussian CDF of $$\phi$$

$$P(Y=-10)=P(X \leq -1) = \phi(-1)$$

$$P(Y=0)=P(-1 < X <1)=\phi(1)-\phi(-1)$$

$$P(Y=10)=P(X \geq 1)= 1- \phi(1)$$

------

#### Example

$$X$$ is a continuous RV with PDF $$f_X$$ and CDF $$F_X$$

$$Y=aX+b$$

1. Case $$a>0$$

   $$F_Y(y)=P(Y \leq y)$$

   $$=P(aX+b \leq y)$$

   $$=P(X \leq \frac{y-b}{a})$$

   $$=F_X(\frac{y-b}{a})$$

   $$f_Y(y)=\frac{d}{dy}F_X(\frac{y-b}{a})=f_X(\frac{y-b}{a})\frac{1}{a}$$

2. Case $$a<0$$

   $$F_Y(y)=P(Y \leq y)$$

   $$=P(aX+b \leq y)$$

   $$=P(X \geq \frac{y-b}{a})$$

   $$=1-F_X(\frac{y-b}{a})$$

   $$f_Y(y)=\frac{d}{dy}F_Y(y)=-f_X(\frac{y-b}{a})\cdot \frac{1}{a}$$

Therefore, $$f_Y(y)=f_X(\frac{y-b}{a})\frac{1}{|a|}$$

==If $$Y=aX+b$$ and $$a \neq 0$$, then $$f_Y(y)=f_X(\frac{y-b}{a})\frac{1}{|a|}$$==



Theorem: 

Suppose $$X$$ is a continuous RV with PDF $$f_X$$

Let $$Y=g(x)$$ where $$g$$ is a continuous differential and strictly monotonic function

Recall that $$S_Y=$$ collection of all possible values of $$Y$$

For $$y \in S_Y$$

$$g^{-1}(y)=$$ value $$x$$ such that $$g(x)=y$$

Method for finding $$f_Y(y)$$ where $$y\in S_Y$$

Step 1. Find $$g^{-1}(y)$$ write $$f_X(g^{-1}(y))$$

Step 2. $$\frac{dg(x)}{dx}|_{x=g^{-1}(y)}$$

Theroem:

$$f_Y(y)=\frac{f_X(g^{-1}(y))}{|\frac{dg(x)}{dx}|_{x=g^{-1}(y)}}$$

whenever the denominator is non-zero

------

$$Y=g(x)=aX+b$$ where $$a \neq 0$$

$$f_Y(y)=\frac{f_X(g^{-1}(y))}{|a|}=\frac{f_X(\frac{y-b}{a})}{|a|}$$

------

#### Example

$$Y=e^x$$

$$X \sim \mathcal{N}(m, \sigma^2)$$

$$y=g(x)=e^x$$

$$S_Y=(0,\infty)$$
$$g^{-1}(y)=\ln(y)$$

$$\frac{dg(x)}{dx}|_{x=g^{-1}(y)}=e^x|_{x=g^{-1}(y)}=e^{\ln(y)}=y$$

For $$y \in (0,\infty)$$

$$f_Y(y)=\frac{f_X(\ln(y))}{y}$$

------

#### Example

$$Y=e^X$$

$$X \sim \mathcal{N}(m, \sigma^2)$$

$$F_Y(y)=P(Y \leq y)=P(e^X \leq y)$$

$$=P(X \leq \ln(y))$$

$$=F_X(\ln(y))$$

$$f_Y(y)=\frac{dF_Y(y)}{dy}=\frac{d}{dy} F_X(\ln(y))$$

$$=f_X(\ln(y))\cdot \frac{1}{y}$$



$$Z=e^{-X}$$

![image-20241021163034677](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021163034677.png)

$$S_Z=(0,\infty)$$ for $$z>0$$

$$F_Z(z)=P(Z \leq z)$$

$$=P(e^{-X} \leq z)$$

$$=P(X \geq - \ln(z))$$

$$=1-F_X(-\ln(z))$$

$$f_Z(z)=\frac{d}{dz}F_Z(z)=-f_X(-\ln(z))\cdot (-\frac{1}{z})$$

$$=\frac{-f_X(-\ln(z))}{z}$$

## Discussion 8

### Topics

1. Continuous Random variable

   1. Probability density function

   2. Expectation, variance, $$n^{th}$$ moment of a continuous RV

   3. Important families of continuous RV

      Gamma and Beta

   4. Some problems

2. Integration tricks

   1. Changing the order of integration in double integrals

### Continuous Random Variables (RV)

A RV $$X$$ is continuous if its range, $$S_X$$, consists of one or more intervals

==$$P[X=x]=0$$== This is always true

Note: No difference between open and closed intervals

![image-20241021164904556](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021164904556.png)

$$P[a \leq X \leq b]=P[a < X < b]$$

------



### Probability density function (PDF)

Similar to PMF is discrete case

But $$P[X=x]=0$$

CDF $$\rightarrow$$ PDF

$$f_X(x)=\frac{d}{dx}F_X(x)$$

Piecewise constant for discrete RV

Because $$F_X(x)=P[X \leq x]=\int_{-\infty}^{x}f_X(x)dx$$

------



### Expected Value

$$E[X]=\int_{-\infty}^{\infty}x f_X(x)dx= \mu_X$$

If $$Y=g(x):x \rightarrow$$  continuous RV

$$E[Y]=E[g(x)]=\int_{-\infty}^{\infty} g(x)f_X(x)dx$$

------



### Linearity Property

$$E[aX+b]=aE[X]+b$$

$$E[\cdot]$$ is a linear operator

------



### Variance

$$Var[X]=E[(X-E[X])^2]=\int_{-\infty}^{\infty} (X-\mu_X)^2 f_X(x)dx$$

Measures how spread-out on RV is around its mean

$$2^{nd}$$ moment: $$Var[X]=E[X^2]-(E[X])^2$$

$$1^{st}$$ moment: $$E[X]=\int_{-\infty}^{\infty}x f_X(x)dx= \mu_X$$

$$n^{th}$$ moment: $$E[X^n]=\int_{-\infty}^{\infty}x^n f_X(x)dx$$

------



### Common continuous RV's

1. Exponential RV

   $$X \sim \text{exp}(\lambda)$$ where $$\lambda$$ is the rate parameter

   $$E[X]=\frac{1}{\lambda}$$

   $$Var[X]=\frac{1}{\lambda^2}$$

   Exponential RV is a continuous version of geometric RV

   Continuous waiting time (packet inter-arrival time)

2. Gaussian RV

   $$X \sim \mathcal{N}(\mu, \sigma^2)$$

   $$f_X(x)=\frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{(x-\mu)^2}{2 \sigma^2}}$$

   $$F_X(x)=\phi(\frac{x-\mu}{\sigma^2})$$ is the standard normal CDF

   $$\phi(Z)=\int_{-\infty}^{\infty}\frac{1}{\sqrt{2 \pi}} e^{-\frac{w^2}{2}}dw$$

   noise modeling, linear systems, high dimension data analysis

3. Uniform RV

   $$X \sim \text{Uniform} (a,b)$$

   $$f_X(x)=\begin{cases}\frac{1}{b-a} &a \leq x \leq b \\ 0 & \text{otherwise}\end{cases}$$

4. Gamma RV

   $$\text{Gamma RV}=\begin{cases} \text{Exponential} \\ \text{Chi-squared} \\ \text{Erlang}\end{cases}$$

   $$X \sim \gamma(\alpha, \lambda)$$ (2-parametric RV)

   $$f_X(x)=\frac{1}{\Gamma(\alpha)}\lambda^{\alpha}x^{\alpha-1}e^{-\lambda x}, 0 \leq x\leq \infty$$

   $$\Gamma(\alpha)=\int_{0}^{\infty}x^{\alpha-1}e^{-x}dx$$

   $$\Gamma(n)=(n-1)!$$

   $$\Gamma(1/2)=\sqrt{\pi}$$

   $$\Gamma(\alpha+1)=\alpha \Gamma(\alpha)$$

   When $$\alpha=1$$

   $$X \sim \text{exp} (\lambda)$$

   ![image-20241021193348823](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021193348823.png)

4. Beta RV

   $$X \sim \text{Beta}(\alpha,\beta)$$

   $$f_X(x)=\begin{cases}\frac{1}{B(\alpha,\beta)}x^{\alpha-1}(1-x)^{\beta-1} &0 \leq x \leq 1 \\ 0 & \text{otherwise}\end{cases}$$

   $$B(\alpha,\beta)=\int_{0}^{1}x^{\alpha-1}(1-x)^{\beta-1}$$

   when $$\alpha=\beta=1$$

   $$X \sim \text{Uniform}(0,1)$$

   $$E[X]=\frac{\alpha}{\alpha+\beta}$$

   $$Var[X]=\frac{\alpha\beta}{(\alpha+\beta+1)(\alpha+\beta)^2}$$

Note: $$X_1, X_2, ... $$ Independent

$$X_i \sim \text{exp} (\lambda)$$

If $$Y=X_1+X_2+...+X_m$$

then $$Y \sim \text{Gamma} (m,\lambda)$$



![image-20241021195555202](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021195555202.png)

$$t_j \sim \text{Gamma} (j, \lambda)$$

$$\Delta t\sim \text{exp}(\lambda)$$

------

### Problem 6.1

Let $$X$$ be a continuous random variable representing the (exact) ligetime of a hard drive, measured in years. A simple model for $$X$$ is that is an Exponential $$(\lambda)$$ random variable. You may assume that your brand of hard drive has an average lifetime of 100 years.

Given:

$$X \sim \text{exp}(\lambda)$$

$$E[X]=100=\frac{1}{\lambda}$$

$$\lambda=1/100$$

(a) What is the probability that the drive fails before 1 year?

$$P[X<1]=\int_{-\infty}^{1}f_X(x)dx$$

$$=\int_{0}^{1}\lambda e^{-\lambda x}dx$$

$$=\int_{0}^{1}\frac{1}{100}e^{-\frac{x}{100}}dx$$

$$=-e^{-\frac{x}{100}}|_{0}^{1}$$

$$=1-e^{-\frac{1}{100}}$$

(b) What is the probability that it lasts less than 5 years?

Same

(c) Consider the event $$B ={X \geq y}$$ that your hard drive has already lasted y years. What is the conditional PDF $$f_{X|B}(x)$$? Interpret the intuition behind your formula.

PDF of event $$B$$

$$P[B]=P[X \geq y]=\int_{y}^{\infty}\frac{1}{100} e^{- \frac{x}{100}}dx$$

$$P[B]=e^{- \frac{y}{100}}$$

$$f_{X|B}(x)=\frac{f_X(x)}{P[B]}$$

$$=\frac{1/100 e^{-\frac{x}{100}}}{e^{-\frac{y}{100}}}$$

$$=\frac{1}{100} e^{- \frac{x-y}{100}}$$

conditioned on the fact that nothing has happened up to time $$y$$, it is as if we start with on entirely new exponential RV treating $$y$$ as time 0

memoryless property of exponential RV

(d) Say that your hard drive has already lasted $$y$$ years. What is the probability that it fails before $$y + 1$$ years?

$$P[X < y+1|X \geq y]=\int_{-\infty}^{y+1} f_{X|B}(x)dx$$

$$=\int_{y}^{y+1}\frac{1}{100} e^{- \frac{x-y}{100}}dx$$

------

### Question

A certain nonlinear circuit has random input $$X\sim \text{exp} (1)$$, and output $$Y=X^{1/4}$$ Find the second moment of the output.

$$E[Y^2]=E[(X^{1/4})^2]$$

$$=E[X^{1/2}]$$

$$=\int_{-\infty}^{\infty} X^{1/2} f_X(x)dx$$

$$E[Y^2]=\int_{0}^{\infty}X^{1/2}e^{-x}dx$$

$$=\int_{0}^{\infty} X^{3/2 -1}e^{-x}dx$$

Recall: $$\Gamma(\alpha)=\int_{0}^{\infty}x^{\alpha-1}e^{-x}dx$$

$$=\Gamma(3/2)=\Gamma(1+1/2)$$

Recall: $$\Gamma(\alpha+1)=\alpha \Gamma(\alpha)$$

$$=1/2\Gamma(1/2)$$

Recall: $$\Gamma(1/2)=\sqrt{\pi}$$

$$=\frac{\sqrt{\pi}}{2}$$

------

### Integration tricks

Claim:

For a non-negative RV, i.e., $$f_X(x)=0, \forall x <0$$

S.T. $$E[X]=\int_{0}^{\infty}(1-F_X(t))dt$$

Proof:

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx$$

$$=\int_{0}^{\infty} (\int_{t=0}^{x}1 dt)f_X(x)dx$$

$$=\int_{x=0}^{\infty} \int_{t=0}^{x}  dtf_X(x)dx$$

![image-20241021233219548](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021233219548.png)

$$D={(x,y): 0 \leq x \leq \infty, 0 \leq t \leq x}$$

$$D={(x,y): t \leq x \leq \infty, 0 \leq t \leq \infty}$$

$$=\int_{t=0}^{\infty} \int_{x=t}^{\infty}  f_X(x)dx dt$$

where $$ \int_{x=t}^{\infty}  f_X(x)dx=P[X > t]=1-F_X(t)$$

$$=\int_{t=0}^{\infty} (1-F_X(x)) dt$$

------

$$I=\int_{x=0}^{2} \int_{y=x^2}^{4}f(xy)dydx$$

![image-20241021233728313](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241021233728313.png)

$$D={(x,y): 0 \leq x \leq 2, x^2 \leq y \leq 4}$$

$$D={(x,y): 0 \leq x \leq \sqrt{y}, 0 \leq y \leq 4}$$

$$=\int_{y=0}^{4} \int_{x=0}^{\sqrt{y}}  f(xy)dx dy$$

## Week 9 Session 1

### Gaussian RV

If $X \sim \mathcal{N}(m,\sigma^2)$ and $$Z=\frac{X-m}{\sigma}$$ , then $$Z \sim \mathcal{N}(0,1)$$

$$F_X(x)=P(X \leq x)$$

$$=P(\frac{X-m}{\sigma}\leq \frac{x-m}{\sigma})$$

$$=P(Z \leq \frac{x-m}{\sigma})$$

$$=\phi(\frac{x-m}{\sigma})$$

where $$\phi$$ is the CDF of standard normal RV

------

### PDF of a function of a continuous RV

Theorem:

Suppose $$X$$ is a continuous RV with PDF $$f_X$$

Let $$Y=g(x)$$, where $$g$$ is a continuous, differentiable and strictly monotonic function

Then, for $$y \in S_Y$$

$$f_Y(y)=\frac{f_X(g^{-1}(y))}{|\frac{dg(x)}{dx}|_{x=g^{-1}(y)}}$$

whenever the denominator is non-zero

For $$y \notin S_Y, f_Y(y)=0$$

------

### Extension of the previous theorem

Thm:

Suppose $$X$$ is a continuous RV with PDF $$f_X$$ and range $$S_X$$

Let $$Y=g(X)$$

Suppose $$S_X$$ can be partitioned into finitely many intervals such that $$g(x)$$ is continuous, differentiable and strictly monotonic in each interval

$$S_X=(0,2\pi)$$
![image-20241023190700729](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241023190700729.png)

For $$y \in S_Y$$, let

$$g^{-1}(y)=\{\text{all values of }x \text{\: such that\:} g(x)=y\}=\{x_1,x_2,...x_n\}$$

Then 

$$f_Y(y)=\sum_{i=1}^{n}\frac{f_X(x_i)}{|\frac{dg(x)}{dx}|_{x=x_i}}$$

whenever the denominators are non-zero

$$f_Y(y)=0$$ for all $$y \notin S_Y$$

#### Example

$$X \sim \text{Uniform}(-1,1)$$
$$Y=X^2=g(X)$$

$$\frac{dg(x)}{dx}=2x$$
$$S_X=[0,1)$$

![image-20241023192102416](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241023192102416.png)

For $$y \in S_Y$$
$$g^{-1}(y)=\{\sqrt{y}, - \sqrt{y}\}$$

$$f_Y(y)=\frac{f_X(\sqrt{y})}{|\frac{dg(x)}{dx}|_{x=\sqrt{y}}}+\frac{f_X(-\sqrt{y})}{|\frac{dg(x)}{dx}|_{x=-\sqrt{y}}}$$

$$=\frac{f_X (\sqrt{y})}{2\sqrt{y}}+\frac{f_X (-\sqrt{y})}{2\sqrt{y}}$$

$$f_Y(y)=\begin{cases} \frac{f_X (\sqrt{y})}{2\sqrt{y}}+\frac{f_X (-\sqrt{y})}{2\sqrt{y}} & 0<y<1 \\ \text{undefined} &y=0 \\ 0 & y \notin S_Y \end{cases}$$

#### Method 2 CDF Method

$$Y=X^2$$
$$S_Y=[0,1]$$

$$F_Y(y)=P(Y \leq y)$$

$$\begin{cases} 0 & \text{if\:} y<0 \\ P(Y \leq 0)=P(Y=0)=P(X=0)=0 & \text{if\:} y=0\\P(Y\leq y) & \text{if\:} 0<y<1 \\ 1 & \text{if\:} y \geq 1 \end{cases}$$

$$P(Y \leq y)=P(X^2 \leq y)$$

$$=P(-\sqrt{y} \leq x \leq \sqrt{y})$$

$$=F_X(\sqrt{y})-F_X(-\sqrt{y})$$

$$F_Y(y)=\begin{cases}0 & \text{if\:} y \leq 0 \\ F_X(\sqrt{y})-F_X(-\sqrt{y}) & \text{f\:} 0<y<1 \\ 1 & \text{if\:} y \geq 1\end{cases}$$

$$f_Y(y)=\begin{cases}0 & \text{if\:} y \leq 0 \\ F_X(\sqrt{y}) \frac{1}{2\sqrt{y}}+F_X(-\sqrt{y})\frac{1}{2\sqrt{y}} & \text{f\:} 0<y<1 \\ 1 & \text{if\:} y \geq 1\end{cases}$$



#### Example

![image-20241024202735944](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024202735944.png)

Light source is pointing at a random angle $$\theta$$ from the vertical direction

$$\theta \sim \text{Uniform}(-\frac{\pi}{2},\frac{\pi}{2})$$

Find the CDF/PDF of $$X$$

$$X=g(\theta)=\tan{\theta}$$

<u>CDF method</u>

$$S_X=(-\infty,\infty)$$
$$P(X \leq x)=P(\tan{\theta} \leq x)$$

$$=P(\theta \leq \tan^{-1}{x})$$

$$=\int_{-\infty}^{\tan^{-1}{x}}f_{\theta}(t)dt$$

Tangent graph

![image-20241024203038760](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024203038760.png)

$$\theta \sim \text{Uniform}(-\frac{\pi}{2},\frac{\pi}{2})$$

$$f_\theta(t)=\begin{cases} \frac{1}{\pi} & -\frac{\pi}{2}< t< \frac{\pi}{2} \\ 0 & \text{othewise}\end{cases}$$

$$=\int_{-\frac{\pi}{2}}^{\tan^{-1}{x}}\frac{1}{\pi}dt$$

$$=\frac{1}{\pi}(\tan^{-1}{x}+\frac{\pi}{2})$$

$$\frac{dF_X(x)}{dx}=f_X(x)=\frac{1}{\pi}(\frac{1}{1+x^2})$$         - Cauchy Distribution

Density of $$X$$ using the theorem above

$$f_X(x)=\frac{f_\theta(g^{-1}(x))}{\frac{dg(\theta)}{d \theta}|_{\theta=g^{-1}(x)}}$$

$$X=g(\theta)=\tan{\theta}$$

$$g^{-1}(x)=\tan^{-1}(x)$$

$$\frac{dg(\theta)}{d \theta}=\frac{d \tan{\theta}}{d \theta}=\frac{1}{\cos^2{\theta}}$$

$$=\frac{f_\theta(\tan^{-1}(x))}{\frac{1}{\cos^2{\theta}}}|_{\theta=\tan^{-1}x}$$

$$=\frac{\frac{1}{\pi}}{\frac{1}{\cos^2{\theta}}}|_{\theta=\tan^{-1}x}$$

$$=\frac{1}{\pi \frac{1}{1+x^2}}$$



$$\theta=\tan^{-1}x$$

$$\tan{\theta}=x$$
$$\frac{\sin{\theta}}{\cos{\theta}}=x$$
$$\sin^2{\theta}+cos^2{\theta}=1$$

$$\frac{\sin^2{\theta}}{\cos^2{\theta}}+1=\frac{1}{\cos^2{\theta}}$$

$$x^2+1=\frac{1}{\cos^2{\theta}}$$

------

### Important Probability inequalities

1. Markov Inequality

   $$X$$ is a continuous RV which is non-negative

   $$P(X \geq a)=\int_{a}^{\infty}f_X(x)dx$$ where $$a>0$$

   we may only know the mean of $$X$$ but not its PDF

### Markov inequality

For a non-negative continuous RV $$X$$ and a positive number $$a$$

$$P(X \geq a) \leq \frac{E[X]}{a}$$

Proof:

$$P(X \geq a)=\int_{a}^{\infty}f_X(t)dt$$

$$E[X]=\int_{-\infty}^{\infty}xf_X(x)dx=\int_{0}^{\infty} x f_X(x)dx$$
$$=\int_{0}^{a} x f_X(x)dx+\int_{a}^{\infty} x f_X(x)dx \geq \int_{a}^{\infty} x f_X(x)dx$$

$$\geq \int_{a}^{\infty} a f_X(x)dx=aP(X \geq a)$$

$$P(X \geq a ) \leq \frac{E[X]}{a}$$



Markov Inequality

==For any non-negative RV $$X$$ and a positive number $$a$$==

==$$P(X \geq a ) \leq \frac{E[X]}{a}$$==



#### Example

1. Duration of a call at a cellphone base station is a continuous RV with mean 100 seconds. Find a bound on the probability that the call duration is $$\geq 150$$ seconds.

   $$P(D\geq 150) \leq \frac{E[D]}{150}=\frac{100}{150}$$

   $$P(D>150)=P(D\geq 150)$$

2. Number of simultaneous calls at this base station is a discrete RV with mean 100. Denote this RV by $$N$$

   $$P(N\geq 150) \leq \frac{E[N]}{150}=\frac{100}{150}$$

   $$P(N > 150)=P(N \geq 151) \leq \frac{E[N]}{151}$$

------

Proof of Markov Inequality for arbitrary non-negative RV $$X$$

$$Y=g(x)=\begin{cases} 1 &\text{if\:} X \geq a \\ 0 &\text{if\:} X<a\end{cases}$$

$$E[Y]=1 \cdot P(X \geq a) + 0 \cdot P(X \leq a)$$

$$=P(X \geq a)$$

$$Z=X -ag(X)$$

$$E[Z]=E[X-aY]$$
$$=E[X]-aP(X\geq a)$$

Claim: $$Z$$ is a non-negative RV 

Proof:

Suppose $$X$$ take the value $$x \geq 0$$

Case 1: $$x \geq a $$
$$Z=X-ag(X)$$

$$=x-a \geq 0$$

Case 2: $$x<a$$

$$Z=X-ag(X)$$

$$=x \geq 0$$

So claim so true

Because $$Z$$ is non-negatives

$$E[Z] \geq 0$$

$$E[x]-aP(X\geq a) \geq 0$$

$$\frac{E[X]}{a}\geq P(X \geq a)$$



#### Example

$$X$$ is a non-negative

$$E[X]=2$$

$$P(X\geq 1) \leq \frac{E[X]}{1}=2$$



### Chebyshev's Inequality

$$X$$ is any RV given the mean $$m$$ and its variance $$\sigma^2$$, $$a>0$$

$$P(|X-m| \geq a)=P((X-m)^2\geq a^2) \leq \frac{E[(X-m)^2]}{a^2}=\frac{\sigma^2}{a^2}$$

$$P(|X-m|\geq a) \leq \frac{\sigma^2}{a^2}$$ for $$a>0$$



#### Example

$$X \sim \mathcal{N}(m,\sigma^2)$$

$$k$$ is a positive number

$$P(|X-m| \geq k\sigma) \leq \frac{\sigma^2}{k^2 \sigma^2}=\frac{1}{k^2}$$

$$k=2$$

$$P(|X-m|\geq 2\sigma) \leq \frac{1}{4}$$
Exact calculation of probability

$$P(|X-m|\geq 2 \sigma)=1-P(|X-m|< 2\sigma)$$
$$=1-P(-2\sigma < X-m < 2 \sigma)$$
$$=1-P(-2 < \frac{X-m}{\sigma} <2)$$

where $$\frac{X-m}{\sigma}=\mathcal{N}(0,1)$$

$$=1-(\phi(2)-\phi(-2))$$

$$=0.0456$$



#### Example

$$X$$ is a discrete RV

$$P(X=c)=P(X=-c)=1/2$$
$$E[X]=0$$

$$Var[X]=E[X^2]-m^2=E[X^2]=c^2$$
$$P(|X-0|\geq c) \leq \frac{Var(X)}{c^2}=1$$
After exact calculation

$$P(|X|\geq c)=1$$

------

### Chernoff bound

Any RV 

For any $$a>0$$

$$P(X \geq a)$$
Consider any $$s \geq 0$$

$$\{X \geq a\}=\{e^{sX} \geq e^{sa}\}$$

$$P(X \geq a)=P(e^{sX} \geq e^{sa})$$
$$Z=e^{sX}$$ is a non-negative RV

$$P(Z \geq e^{sa}) \leq \frac{E[Z]}{e^{sa}}=\frac{E[e^{sX}]}{e^{sa}}$$

==$$P(X \geq a) \leq \min_{s \geq 0} \frac{E[e^{sX}]}{e^{sa}}$$==



#### Example

$$X \sim \text{exp}(1)$$
$$f_X(x) =\begin{cases} e^{-x} & \text{if\:} x \geq 0 \\ 0 & \text{if\:} x<0\end{cases}$$

$$P(X \geq 7) \leq \min_{s \geq 0} \frac{E[e^{sX}]}{e^{7s}}$$

$$E[e^{sX}]=\int_{0}^{\infty}e^{sx}e^{-x}dx$$

$$=\begin{cases} \frac{1}{1-s} & \text{if\:} 0 \leq s < 1\\ \infty & \text{if\:} s \geq 1\end{cases}$$

$$P(X \geq 7) \leq \min_{0 \leq s <1} \frac{\frac{1}{1-s}}{{e^{7s}}}$$

minimum is achieved at $$s=6/7$$

$$\frac{\frac{1}{1-6/7}}{{e^{7 \cdot 6/7}}}=7e^{-6}$$

Exact value of $$P(X \geq 7)$$

$$\int_{7}^{\infty} e^{-x}dx=$$ find this value and compare with upper bound above

------

## Week 9 Session 2

### Pair of random variables

Two random variable 

$$\Omega$$

$$X: \Omega \rightarrow \R$$

$$Y: \Omega \rightarrow \R$$
![image-20241024212440938](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024212440938.png)

#### Example

Roll a fair 6-sided die 3 times

$$\Omega=\{111,112,121,...\}$$

Equally likely

$$P(\{\Omega\})=\frac{1}{6^3}=\frac{1}{216}$$

$$X=$$ Number on the first roll

$$Y=$$ Sum of the numbers on 3 rolls

![image-20241024212806190](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024212806190.png)

$$P(X=1 \text{\:and\:} Y=3)=P(\{111\})=\frac{1}{216}$$

$$P(X=2 \text{\:and\:} Y=5)=P(\{212,221\})=\frac{2}{216}$$

$$P(X=2, Y=5)$$

$$P(Y-X \geq 2)=P(\Omega)=1$$

$$P(Y-X=2)=P(\{111,211,311,411,511,611\})=\frac{6}{216}$$

$$P(a \leq X \leq b, c \leq Y \leq d)$$

$$P((X,Y) \in \R)$$

![image-20241024213155661](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024213155661.png)

$$P(X \leq b, Y \leq d)$$

![image-20241024213317630](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024213317630.png)

$$P(Y \geq -X)$$

![image-20241024213333962](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024213333962.png)

$$P(Y \leq X^2)$$

![image-20241024213352240](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024213352240.png)

------

Two discrete RVs

$$X: S_Y=\{x_1,x_2,...x_m\}$$

$$Y: S_Y=\{y_1, ... ,y_n\}$$

Joint PMF of $$X$$ and $$Y$$

$$P_{XY}(x,y)=P(X=x \text{\: and \:} Y=y)$$

PMF: $$P_X(x)=P(X=x)$$

$$=P(\{X=x\} \bigcap \{Y=y\})$$

### Properties

1. $$ 0 \leq P_{XY}(x,y) \leq 1$$

2. $$\sum_{x \in S_X} \sum_{y \in S_Y}P_{XY} (x,y)=1$$

   $$\sum_{x \in S_X}P_X(x)=1$$

   $$A_{ij}=\{\omega \in \Omega: X(\omega)=x_i \text{\: and \:} Y(\omega)=y_j\}$$

   $$A_{11}, A_{12}, ... , A{mn}$$ - Partition of $$\Omega$$

   $$\sum_{i} \sum_{j} P(A_{ij})=1$$

   $$\sum_{i} \sum_{j} P_{XY}(x_i,y_j)=1$$

3. $$P(a \leq X \leq b, c \leq Y \leq d)$$

   $$\sum_{a \leq x \leq b} \sum_{c \leq y \leq d} P_{XY}(x,y)$$

   ![image-20241024214103116](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024214103116.png)

   $$P((X,Y) \in B)$$

   $$\sum_{(x,y)\in B} P_{XY} (x,y)$$

   ![image-20241024214135252](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024214135252.png)

#### Example

$$S_X=S_Y=\{0,1,2\}$$

$$P_{XY}(x,y)$$

| x\y  | 0    | 1    | 2    |
| ---- | ---- | ---- | ---- |
| 0    | 1/16 | 0    | 0    |
| 1    | 1/4  | 1/8  | 0    |
| 2    | 1/4  | 1/4  | 1/16 |

$$P(X+Y =2)=P_{XY}(1,1)+P_{XY}(0,2)+P_{XY}(2,0)$$

$$=1/8+0+1/4$$

$$P(Y>X)=P_{XY}(0,1)+P_{XY}(0,2)+P_{XY}(1,2)$$

$$=0+0+0$$

------

### Joint PMF to individual PMFs

$$P_X(x)=P(X=x)$$

$$=\sum_{y \in S_Y}P_{XY}(x,y)$$

$$P(X=x)=\sum_{y \in S_Y} P(X=x,Y=y )=\sum_{y \in S_Y} P_{XY}(x,y)$$

$$P_X(x)=\sum_{y \in S_Y} P_{XY} (x,y)$$

$$P_Y(y)=\sum_{x \in S_X} P_{XY} (x,y)$$

Marginal PMFs of $$X$$ and of $$Y$$



#### Example

Number of bytes is a RV $$N$$ with PMF

$$P_N(n)=(1-p) p^n$$

$$n=0,1,2,...$$

Bytes are grouped into packets

Two bytes are grouped to form 1 packet

$$N=4 \rightarrow$$ (_ _ _ _) $$=(P1, P2)$$ 

$$N=5 \rightarrow$$ (_ _ _ _ _) $$=(P1, P2, \_)$$ where the last byte is the leftover or remainder bytes

$$Q=$$ Number of packets formed 

$$R=$$ Number of remainder bytes

$$S_Q=\{0,1,2,...\}$$

$$S_R=\{0,1\}$$

Joint PMF of $$Q$$ and $$R$$
$$P_{QR}(q,r)=P(Q=q, R=r)$$

$$=P(N=2q+r)$$

$$=(1-p)p^{2q+r}$$



Marginal PMF of $$Q$$

$$P_Q(q)=\sum_{r=0}^{1}P_{QR}(q,r)$$
$$=(1-p)p^{2q}+(1-p)^{2q+1}$$

$$q=0,1,2,...$$



Marginal PMF of R

$$P_R(r)=\sum_{q=0}^{\infty}P_{QR}(q,r)$$

$=\sum_{q=0}^{\infty} (1-p)p^{2q+r}$

$$=(1-p)p^r \sum_{q \geq 0} p^{2q}$$

$$=(1-p)p^r \frac{1}{1-p^2}$$

$$P_R(0)+P_R(1)=1$$
$$P(Q \leq 2, R=0)=\sum_{0 \leq q \leq 2}P_{QR} (q,0)$$

------

CDF

$$F_X(x)=P(X \leq x)$$ defined for all RVs

Joint CDF of $$X$$ and $$Y$$

$$F_{XY}(x,y)=P(X \leq x \text{\: and \:}Y \leq y)$$

$$=P(X \leq x, Y \leq y)$$ can be defined for all pairs of RVs

### Properties of joint CDF

1. $$0 \leq F_{XY}(x,y) \leq 1$$

2. $$P(X \leq 1, Y \leq 2)=F_{XY}(1,2) \leq F_{XY}(5,8)=P(X \leq 5, Y \leq 8)$$

   If $$x_1 \leq x_2$$ and $$y_1 \leq y_2$$, then

   $$F_{XY}(x_1,y_1) \leq F_{XY} (x_2,y_2)$$

3. $$\lim_{y \rightarrow \infty}F_{XY}(x,y)$$

   $$\lim_{y \rightarrow \infty}P(X \leq x, Y \leq y)=P(X \leq x, y < \infty)$$

   $$=P(\{X \leq x\} \bigcap \{Y < \infty\})$$    where $$\{Y < \infty\}=\Omega$$

   $$=P(\{X \leq x\} \bigcap \Omega)$$

   $$=P(X \leq x)=F_X(x)$$

   $$\lim_{y \rightarrow \infty} F_{XY}(x,y)=F_X(x)$$

   $$\lim_{x \rightarrow \infty} F_{XY}(x,y)=F_Y(y)$$

4. $$\lim_{y \rightarrow \infty} \lim_{x \rightarrow \infty}F_{XY}(x,y)=1$$

   $$\lim_{x \rightarrow \infty, y \rightarrow \infty}P(X \leq x, Y \leq y)=P(X < \infty, Y < \infty)=1$$

   $$\lim_{y \rightarrow \infty}[\lim_{x \rightarrow \infty}F_{XY}(x,y)]=1$$

   $$\lim_{y \rightarrow \infty}[F_Y(y)]=1$$

5. $$\lim_{y \rightarrow -\infty}F_{XY}(x,y)=0$$

   $$\lim_{x \rightarrow -\infty}F_{XY}(x,y)=0$$

   $$\lim_{y \rightarrow -\infty}P(X \leq x, Y \leq y)=P(X \leq x, Y=-\infty)$$

   $$=P(\{X \leq x\}\bigcap \{Y=-\infty\})$$    where $$\{Y =-\infty\}=\phi$$

   $$=P(\phi)=0$$

6. $$\lim_{y \rightarrow -\infty} \lim_{x \rightarrow -\infty}F_{XY}(x,y)=0$$

7. Right continuity

   $$\lim_{h \downarrow 0}F_X(x+h)=F_X(x)$$

   $$\lim_{h \downarrow 0}F_{XY}(x+h,y)=F_{XY}(x,y)$$

   ![image-20241024221641303](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024221641303.png)

   $$\lim_{h \downarrow 0}F_{XY}(x,y+h)=F_{XY}(x,y)$$

8. $$P(x_1 < X \leq x_2, y_1 < Y \leq y_2)$$

   ![image-20241024221809036](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024221809036.png)

   $$P(x_1 < X \leq x_2)=F_X(x_2)-F_X(x_1)$$

   $$P(X \leq x_2, Y \leq y_2)=F_{XY}(x_2,y_2)$$

   $$F_{XY}(x_2,y_2)=P(A)+P(B)+P(C)+P(D)$$

   

   $$D=\{X \leq x_1, Y \leq y_1\}$$

   $$P(D)=P(X \leq x_1, Y \leq y_1)=F_{XY}(x_1,y_1)$$

   

   $$P(X \leq x_1, Y \leq y_2)=P(A)+P(D)$$

   $$F_{XY}(x_1,y_2)=P(A)+P(D)$$

   $$P(A)=F_{XY}(x_1,y_2)-F_{XY}(x_1,y_1)$$

   

   $$F_{XY}(x_2, y_1)=P(C)+P(D)$$

   $$P(C)=F_{XY}(x_2,y_1)-F_{XY}(x_1,y_1)$$

   

   ==$$P(B)=F_{XY}(x_2,y_2)+F_{XY}(x_1,y_1)-F_{XY}(x_1,y_2)-F_{XY}(x_2,y_1)$$==

   $$P(x_1< X \leq x_2, y_1< Y \leq y_2)$$

#### Example

$$F_{XY}(x,y)=\begin{cases} (1-e^{-\alpha x})(1-e^{-\beta y})& \text{if\:} x \geq 0, y \geq 0\\ 0 & \text{otherwise}\end{cases}$$

$$=\begin{cases}0 & \text{if\:} x<0 \\ 1-e^{-\alpha x} & \text{if\:} x \geq 0\end{cases}$$

$$F_Y(y)=\lim_{x \rightarrow \infty}F_{XY}(x,y)$$

$$=\begin{cases}0 & \text{if\:} y<0 \\ 1-e^{-\beta y} & \text{if\:} y \geq 0\end{cases}$$



#### Example

$$F_{XY}(x,y)=\begin{cases} 0 & \text{if\: } x<0, y\in \R\\ 0 & \text{if\: } y<0, x\in \R\\ xy & 0 \leq x \leq 1, 0\leq y \leq 1\\x & 0 \leq x \leq 1, y>1 \\ y & x>1, 0\leq y \leq 1\\ 1 & x\geq 1, y\geq 1\end{cases}$$

$$F_X(x)=\lim_{y \rightarrow \infty}F_{XY}(x,y)$$

$$=\begin{cases} 0 & x<0 \\ x & 0\leq x \leq 1\\ 1 & x>1\end{cases}$$

![image-20241024223530788](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024223530788.png)



#### Example

$$F_{XY}(x,y)=\begin{cases} (1-e^{-\alpha x})(1-e^{-\beta y})& \text{if\:} x \geq 0, y \geq 0\\ 0 & \text{otherwise}\end{cases}$$

![image-20241024224147353](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024224147353.png)

$$P(1<X\leq 2, 2<Y \leq 5)=F_{XY}(2,5)+F_{XY}(1,2)-F_{XY}(1,5)-F_{XY}(2,2)$$

$$C=\{X > x, Y >y\}$$

$$P(X>x, Y>y)=1-P(X\leq x, Y\leq y)$$

$$P(X> x, Y>y)=P(\{X >x\}\bigcap \{Y>y\})$$ where $$A=\{X >x\}$$ $$B= \{Y>y\}$$

$$P(A \bigcap B)=1-P(A^c \bigcup B^c)$$

$$=1-P(\{X \leq x\}\bigcup \{Y\leq y\})$$

$$=1-(P(X \leq x) +P(Y \leq y)-P(X\leq x, Y \leq y))$$

$$=1-F_X(x)-F_Y(y)+F_{XY}(x,y)$$

------

#### Example

![image-20241024224621991](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241024224621991.png)

$$X$$ takes when $$+1$$ or $$-1$$ with equal probability

$$N \sim \text{Uniform}[-2,2]$$
$$f_N(n)=\begin{cases} 1/4 & -2 \leq n \leq2 \\ 0 &\text{otherwise}\end{cases}$$

For any 2 numbers $$a,b$$, $$\{N \leq a\}$$ and $$\{X=b\}$$ are independent events

$$P(\{N \leq a\} \bigcap \{X=b\})=P(N\leq a)P(X=b)$$



$$F_N(n)=\int_{-\infty}^{n}f_N(t)dt$$

$$=\begin{cases} 0 & \text{if\:} n <-2 \\ \frac{n+2}{4} & \text{if\:} -2 \leq n \leq 2 \\ 1 & \text{if\:} n \geq 2\end{cases}$$

$$F_{XN}(-1,n)=P(X \leq -1, N \leq n)$$

$$=P(X=-1,N \leq n)$$

$$=P(X=-1)P(N \leq n)$$
$$=\frac{1}{2}F_N(n)$$



$$F_{XN}(1,n)=P(X \leq 1, N \leq n)$$

$$=P(\{X\leq 1\} \bigcap \{ N \leq n\})$$

$$=P(N\leq n)$$

$$=F_N(n)$$



$$P(X\leq 1, N\leq n)=P(\{X=-1, N \leq n\} \bigcup \{X=+1, N\leq n \})$$

$$=P(X=-1,N \leq n)+P(X=+1, N \leq n)$$

$$=\frac{1}{2}F_N(n)+\frac{1}{2}F_N(n)=F_N(n)$$



$$P(X=+1,Y \leq 0)=P(X=+1,X+N \leq 0)$$

$$=P(X=+1, 1+N \leq 0)$$

$$=P(X=+1,N \leq -1)$$

$$=P(X=+1)P(N \leq -1)$$

$$=\frac{1}{2}F_N(-1)$$



$$P(X=+1, Y\leq 0)=P(Y \leq 0|X=+1)P(X=+1)$$

$$=P(X+N \leq 0|X=+1)\frac{1}{2}$$

$$=P(N\leq -1|X=+1)\frac{1}{2}$$

$$=P(N\leq -1) \frac{1}{2}$$

$$=F_N(-1) \frac{1}{2}$$

## Discussion 9

### Topics

1. Key formulas for discrete and continuous random variables
2. Characteristic functions
   1. Definition
   2. Properties
   3. Some problems
3. Problems

### Overview of discrete and continuous RV's

|                | Discrete                                    | Continuous                                      |
| -------------- | ------------------------------------------- | ----------------------------------------------- |
| $$P_X(x)/S_X$$ | $$P(\{\omega: \forall X(\omega)=x\})$$      | $$P(\{\omega: a \leq X(\omega) < b\})$$         |
| $$E[X]$$       | $$\sum_{x \in S_X} xP_X(x)$$                | $$\int_{-\infty}^{\infty}x f_X(x)dx$$           |
| $$Var[X]$$     | $$\sum_{x \in S_X}(x-\mu_X)^2 P_X(x)$$      | $$\int_{-\infty}^{\infty}(x-\mu_X)^2 f_X(x)dx$$ |
| $$E[X^n]$$     | $$\sum_{x \in S_X} x^nP_X(x)$$              | $$\int_{-\infty}^{\infty}x^n f_X(x)dx$$         |
| $$F_X(x)$$     | $$F_X(x)=P(X \leq x)=\sum_{k=0}^{x}P[X=k]$$ | $$F_X(x)=\int_{0}^{x}f_X(x)dx$$                 |
| $$E[g(x)]$$    | $$\sum_{x \in S_X} g(x)P_X(x)$$             | $$\int_{-\infty}^{\infty}g(x)f_X(x)dx$$         |

### Characteristic functions

![image-20241026203533633](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241026203533633.png)

1. PMF/ PDF
2. $$E[X],E[X^n]$$
3. CDF

1. Transform RV to a different space
2. Prove in transform domain

Each type of RV (continuous/ discrete) has its own unique characteristic function

![image-20241026203652397](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241026203652397.png)

### Definition

$$\phi_X(\omega) := E[e^{j \omega X}]=\int_{-infty}^{\infty}e^{j \omega X }f_X(x)dx$$ where $$j=\sqrt{-1}$$

Note:

$$\phi_X(x)$$ is simply the Fourier transform of the PDF of a RV $$X$$

$$f_X(x)=\frac{1}{2 \pi}\int_{\omega} \phi_X(\omega)e^{-j \omega X}d \omega$$

### Properties

1. Characteristic function of a RV always exists

2. $$\phi_X(0)=1, |\phi_X(\omega) \leq 1|, \forall \omega \in \R$$ 

3. Let $$X_1,X_2,...X_n$$ are independent RVs

   If $$Y=a_1X_1+a_2X_2+...+a_nX_n$$

   $$a_1:$$ constant

   $$\phi_Y(\omega)=\phi_{a_1X_1+...+a_nX_n}(\omega)=\phi_{X_1}(a_1\omega) \phi_{X_2}(a_2\omega)...\phi_{X_n}(a_n \omega)$$

4. Two RVs $$X,Y$$ are independent if and only if

   $$\phi_{X,Y}(\omega,t)=\phi_{X}(\omega)\phi_Y(t)$$

### Moment theorem

The $$n^{th}$$ moment of a RV $$X$$ is given by

$$E[X^n]=\frac{1}{j^n} \frac{d^n}{d\omega^n} \phi_X(\omega)|_{\omega=0}$$

Proof Sketch:

$$\phi_X(\omega)=\int_{-\infty}^{\infty}e^{j \omega X}f_X(x)dx$$

where $$e^{j\omega X}$$ is the Taylor series expansion

$$\phi_X(\omega)=\int_{-\infty}^{\infty}f_X(x) [1+j\omega X + \frac{(j \omega)^2 X^2}{2!}+ ... + \frac{(j \omega)^n(X)^n}{n!}] dx$$

$$=1+j \omega E[X]+ \frac{(j \omega)^2}{2!}E[X^2]+...+\frac{(j \omega)^n}{n!}E[X^n]$$

$$\frac{d}{d\omega}\phi_X(\omega)|_{\omega =0} =j E[X]$$

$$E[X]=\frac{1}{j}\frac{d}{d \omega}\phi_{X} (\omega)|_{\omega=0}$$

$$\frac{d^n}{d\omega^n}\phi_X(\omega)|_{\omega =0} =j^n E[X^n]$$

### Problems

1. Find characteristic function of geometric RV

   $$P_X(x=k)=\begin{cases} (1-p)^k p & k \geq 1\\ 0 & \text{otherwise}\end{cases}$$

   $$\phi_X(\omega)=\sum_{k=0}^{\infty}(1-p)^k p e^{j \omega k}$$

   $$=p \sum_{k=0}^\infty ((1-p)e^{j \omega})^k$$

   $$\phi_X(\omega)=\frac{p}{1-(1-p)e^{j \omega}}$$

2. Find mean, variance and $$n^{th}$$ moment of exponential RV

   $$X \sim \text{exp}(\lambda)$$

   Find characterize function

   $$\phi_X(\omega)=\int_{0}^{\infty}e^{j \omega x} \lambda e^{-\lambda x}dx$$

   $$\phi_X(\omega)=\lambda \int_{0}^{\infty} e^{-(\lambda -j \omega)x}dx$$

   $$\phi_X(\omega)=\frac{\lambda}{\lambda-j\omega}$$

   From moment theorem

   $$E[X]=\frac{1}{j} \frac{d}{d\omega} \phi_X(\omega)|_{\omega=0}$$

   $$=\frac{1}{j}\frac{d}{d\omega} \frac{\lambda}{\lambda-j\omega}|_{\omega=0}$$

   $$=\frac{1}{j} \frac{\lambda j}{(\lambda-j\omega)^2}|_{\omega=0}=\frac{1}{\lambda}$$

   $$E[X]=\frac{1}{\lambda}$$

   $$E[X^2]=\frac{1}{j^2} \frac{d^2}{d \omega^2} \phi_X(\omega)|_{\omega =0}$$

   $$=\frac{1}{j^2} \frac{-2\lambda}{(X-j\omega)^3}|_{\omega=0}$$

   $$E[X^2]=\frac{2}{\lambda^2}$$

   $$Var[X]=E[X^2]-(E[X])^2$$

   $$=\frac{2}{\lambda^2}-(\frac{1}{\lambda})^2$$

   $$=\frac{1}{\lambda^2}$$

   $$Var[X]=\frac{1}{\lambda^2}$$

   $$n^{th}$$ moment

   $$E[X^n]=\frac{1}{j^n} \frac{d^n}{d\omega^n} \phi_X(\omega)|_{\omega=0}$$

   $$E[X^n]=\frac{n!}{\lambda^n}$$

### Problems

1. Find the CDF and PDF of $$Y=g(X)$$ if $$X \sim \text{Uniform}[0,4]$$ and 

   $$g(X)=\begin{cases} x & 0 \leq x <1 \\ 1 & 1 \leq x < 2\\ 3-x & 2 \leq x < 3\\0 & \text{otherwise}\end{cases}$$

   ![image-20241026210113406](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241026210113406.png)

   CDF of $$Y$$

   $$P[Y \leq y]=P[g(X) \leq y]$$

   $$=P[X \leq g^{-1}(y)]$$

   For $$y<0$$, $$P[Y \leq y]=0$$

   For $$y \geq 1$$, $$P[Y \leq y]=1$$

   For $$0 \leq y \leq 1$$

   $$P[Y \leq y]=P[X \leq g^{-1}(y)]$$

   $$=P[\{X \leq u\} \bigcup \{X \geq u\}]$$

   $$=P[X \leq y] +P[X \geq 3-y]$$

   Note that $$X \sim \text{Uni}[0,4]$$

   $$F_X(x)=\frac{x-a}{b-a}$$

   $$=\frac{y}{4}+ 1- P[X \leq 3-y]$$

   $$=\frac{y}{4} + 1 - \frac{3-y}{4}$$

   $$F_Y(y)=\frac {y}{2}+\frac{1}{4}, 0\leq y <1$$

   ![image-20241026221349259](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241026221349259.png)

   Note that CDF has discontinuous

   Find PDF

   We can still differentiate the CDF and represent discontinuities as delta functions

   $$f_Y(y)=\frac{d}{dy} (\frac {y}{2}+\frac{1}{4}) + \frac{1}{4} \delta(y) + \frac{1}{4} \delta(y-1)$$

   ### Problem 6.4

   RV $$X,Y$$ have the joint PDF

   $$f_{X,Y}(x,y)=\begin{cases} c & 0 \leq y < x <4 \\ 0 & \text{otherwise}\end{cases}$$

   Let $$A$$ be the event $$\{X \leq 1\}$$ and let $$B$$ be the event $$\{Y< 2-X\}$$

   (a) Are $$X$$ and $$Y$$ independent?

   ​       ![image-20241026222654298](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241026222654298.png)

   $$A \subset B$$

   $$f_{X,Y}(x,y) = f_X(x)f_Y(x)$$ if independent 

   Notice the range is not a rectangular region. So we cannot decompose $$f_{X,Y}(x,y)$$ into product of marginals

   $$f_Y(y)=\int_{y}^{4} f_{X,Y}(x,y)dy=\int_{y}^{4} c dy$$

   $$=c[4-y]$$

   $$f_X(x)=\int_{0}^{x}cdx=cx$$

   $$f_X(x)f_Y(y)=c^2 x [4-y] \neq f_{X,Y}(x,y)$$ 

   Therefore $$X,Y$$ are not independent

   (b) Calculate the appropriate value for the constant $$c$$. Set it to this values for the remainder of the problem

   $$\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f_{X,Y}(x,y) dxdy=1$$

   where $$f_{X,Y}(x,y)=c$$

   $$c\int_{-\infty}^{\infty} \int_{-\infty}^{\infty}  dxdy=c (\frac{1}{2} \times 4 \times 4)=8c=1$$

   $$c=\frac{1}{8}$$

   (c) Calculate the probability $$P[B|A]$$

   $$P[B|A]=\frac{P[A \bigcap B]}{P[A]}=\frac{P[A]}{P[A]}=1$$

   (d) Make a clearly labeled sketch of the conditional PDF $$f_{X|Y}(x|0.5)$$

   $$f_{X|Y}(x|0.5)=f_{X|Y}(x|y=0.5)$$

   $$f_{X|Y}(x|y)=\begin{cases} \frac{f_{X,Y}(x,y)}{f_Y(y)} & f_Y(y) >0\\0&\text{otherwise}\end{cases}$$

   $$f_{X|Y}(x|y)=\begin{cases} \frac{1}{4-y} & 0 \leq y<x<4 \\ 0 & \text{otherwise}\end{cases}$$

   $$f_{X|Y}(x|0.5)=\begin{cases} \frac{1}{4-\frac{1}{2}}=\frac{2}{7} & 0 \leq y<x<4 \\ 0 & \text{otherwise}\end{cases}$$

   ![image-20241027110149950](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241027110149950.png)

   (e) Evaluate the conditional expectation $$E[X|Y=0.5]$$ and the conditional variance $$Var[X|Y=0.5]$$

   $$f_{X|Y}(x|0.5)$$ is uniform

   $$E=\frac{a+b}{2}, Var=\frac{(b-a)^2}{12}$$

   $$E_{X|Y}(x|0.5)=\frac{0.5+4}{2}=\frac{9}{4}$$

   $$Var_{X|Y}(x|0.5)=\frac{(4-\frac{1}{2})^2}{12}=\frac{49}{48}$$

## Week 10 Session 1

### Two discrete RVs

$$X, S_X=\{x_1,x_2,...x_m\}$$

$$Y,S_Y=\{y_1,...,y_n\}$$

Joint PMF of $$X$$ and $$Y$$
$$P_{XY}(x,y)=P(X=x,Y=y)$$

------

$$P(a \leq X \leq b, c \leq Y \leq D)$$

![image-20241030145147925](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030145147925.png)

$$\sum_{a \leq X \leq b} \sum_{c \leq Y \leq d}P_{XY}(x,y)$$

![image-20241030145156936](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030145156936.png)

$$P((X,Y) \in B)=\sum_{(X,Y) \in B}P_{XY}(x,y)$$

------

Joint CDF of $$X$$ and $$Y$$ (any kind of RVs)

$$F_{XY}(x,y)=P(X\leq x, Y \leq y)$$

Probability of $$(X,Y)\in$$ Rectangle

$$P(x_1 < X \leq x_2, y_1 < Y \leq y_2)=F_{XY}(x_2,y_2)+F_{XY}(x_1,y_1)-F_{XY}(x_1,y_2)-F_{XY}(x_2,y_1)$$

------

### Jointly continuous RVs

Recall $$X$$ is continuous if

1. $$F_X$$ is continuous function
2. $$F_X(x)=\int_{-\infty}^{x}f_X(s)ds$$

Definition: $$X$$ and $$Y$$ are jointly continuous if

1. $$F_{XY}$$ is continuous function
2. $$F_{XY}(x,y)=\int_{-\infty}^x \int_{-\infty}^y f_{XY} (s,t)dtds$$

Joint probability density function of $$X$$ and $$Y$$

Properties

1. $$f_{XY}(x,y)=\frac{d}{dx}(\frac{d}{dy}F_{XY}(x,y))$$

   $$=\frac{d}{dy}(\frac{d}{dx}F_{XY}(x,y))$$

   whenever the derivative exist

2. Recall $$P(a < X \leq b)=\int_{a}^{b}f_X(s)ds$$

   $$P(a<X \leq b, c<Y \leq d)=\int_{c}^{d}\int_{a}^{b}f_{XY}(s,t)dsdt$$

   $$= \int_{a}^{b} \int_{c}^{d} f_{XY}(s,t)dtds$$

3. $$P((X,Y) \in B)=\int \int_{B} f_{XY}(s,t)dsdt$$

   ![image-20241030150032857](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030150032857.png)

4. $$\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f_{XY}(s,t)dsdt=P((X,Y)\in \R^n)=1$$

5. $$P(x<X \leq x+h,y<Y \leq y+h)$$

   ![image-20241030155311026](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030155311026.png)

   $$\int_{x}^{x+h}\int_{y}^{y+h} f_{XY}(s,t)dtds$$

   $$\approx \int_{x}^{x+h}f_{XY}(s,y)hds$$

   $$\approx f_{XY (x,y)} h \cdot h$$

   ==$$P(x <X \leq x+h, y<Y \leq y+h)\approx f_{XY}(x,y)h^2$$==

6. $$f_{XY}(x,y)$$

   PDF of $$X,f_X(x)$$ from the joint PDF

   $$P(x <X \leq x+h) \approx f_X(x)h$$

   $$P(x < X \leq x+h)=P(x<X \leq x+h, -\infty < Y<\infty)$$

   ![image-20241030183622075](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030183622075.png)

   $$\int_{x}^{x+h} \int_{-\infty}^{\infty}f_{XY}(s,t)dtds$$

   $$=\int_{-\infty}^{\infty}\int_{x}^{x+h}f_{XY}(s,t)dsdt$$

   $$\approx f_{XY}(x,t)h dt$$

   $$f_X(x)h=\int_{-\infty}^{\infty}f_{XY}(x,t)hdt$$

   ==$$f_X(x)=\int_{-\infty}^{\infty}f_{XY}(x,t)dt$$==

   

   Discrete Case

   $$P_X(x)=\sum_yP_{XY}(x,y)$$

   

   $$f_Y(y)=\int_{-\infty}^{\infty}f_{XY}(s,y)ds$$

   $$f_X(x)=\int_{-\infty}^{\infty}f_{XY}(x,t)dt$$

   $$f_Y(y)=\int_{-\infty}^{\infty}f_{XY}(s,y)ds$$

------

#### Example

$$X,Y$$ jointly continuous

$$f_{XY}(x,y)=\begin{cases} 1 & \text{if\:} 0 \leq x \leq 1, 0 \leq y \leq 1\\0 & \text{otherwise}\end{cases}$$

![image-20241030220341364](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030220341364.png)

$$F_{XY}(-2,-2)=\int_{-\infty}^{-2} \int_{-\infty}^{-2}f_{XY}(s,t)dsdt=0$$

$$F_{XY}(7,-1)=\int_{-\infty}^{7} \int_{-\infty}^{-1} f_{XY}(s,t)dtds=0$$

$$F_{XY}(x,y)=0$$ if $$x<0$$ or $$y<0$$

If $$0\leq x \leq 1, 0 \leq y \leq 1$$
$$F_{XY}(x,y)=\int_{-\infty}^{x} \int_{-\infty}^{y} f_{XY}(s,t)dtds$$

$$=\int_{0}^{x} \int_{0}^{y} f_{XY}(s,t)dtds$$

$$=\int_{0}^{x} \int_{0}^{y} 1 dtds$$

$$=xy$$

$$x=1/3, y=2$$
$$F_{XY}(1/3,2)=\int_{-\infty}^{1/3} \int_{-\infty}^{2}f_{XY}(s,t)dtds$$

$$=\int_{0}^{1/3} \int_{0}^{2}f_{XY}(s,t)dtds$$

$$=\int_{0}^{1/3} \int_{0}^{1}f_{XY}(s,t)dtds+\int_{0}^{1/3} \int_{1}^{2}f_{XY}(s,t)dtds$$

$$=\int_{0}^{1/3}\int_{0}^{1}1dtds +0$$
$$=1/3$$

If $$0 \leq x\leq 1$$ and $$y>1$$

$$F_{XY}(x,y)=x$$

If $$0 \leq y \leq 1$$ and $$x>1$$

$$F_{XY}(x,y)=\int_{-\infty}^{y} \int_{-\infty}^{x} f_{XY}(s,t)dsdt$$

$$=\int_{0}^{y} \int_{0}^{x} f_{XY} (s,t) dsdt$$
$$=\int_{0}^{y} \int_{0}^{1} f_{XY} (s,t) dsdt + \int_{0}^{y} \int_{1}^{x} f_{XY} (s,t) dsdt$$

$$=\int_{0}^{y} \int_{0}^{1} dsdt+0$$

$$=y$$
If $$x>1, y>1$$

$$F_{XY}(x,y)=\int_{-\infty}^{x} \int_{-\infty}^{y} f_{XY}(s,t) dtds$$

$$=\int_{0}^{x} \int_{0}^{y} f_{XY}(s,t)dtds$$

$$=\int_{0}^{x} \int_{0}^{1} f_{XY}(s,t)dtds+\int_{0}^{x} \int_{1}^{y} f_{XY}(s,t)dtds$$
$$=\int_{0}^{1} \int_{0}^{x} f_{XY}(s,t)dsdt$$

$$=\int_{0}^{1} \int_{0}^{1} 1dtds$$

$$=1$$

$$P(X \leq x, Y \leq y)=1$$

#### Example

$$f_{XY}(x,y)=\begin{cases} c &\text{if\:} 0 \leq y \leq x \leq 1\\0 & \text{otherwise}\end{cases}$$

![image-20241030221454225](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030221454225.png)

$$\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f_{XY}(s,t)dtds=\frac{1}{2}c=1$$

$$c=2$$
$$\int_{0}^{1} \int_{0}^{s} f_{XY}(s,t)dtds=\int_{0}^{1} \int_{0} ^{s} c dtds$$

$$=\int_{0}^{1}csds$$

$$=c \frac{s^2}{2}|_0^1=1$$

$$c=2$$



Marginal PDF of $$X$$
$$f_X(x)=\int_{-\infty}^{\infty}f_{XY}(x,t)dt$$

If $$0\leq x \leq 1$$

$$f_X(x)=\int_{-\infty}^{\infty}f_{XY}(x,t)dt$$

$$=\int_{0}^{x}2dt=2x$$

![image-20241030221945849](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030221945849.png)

If $$x>1$$

$$f_X(x)=\int_{-\infty}^{\infty} f_{XY} (x,t)dt=0$$

$$f_X(x)= \begin{cases}2x & 0 \leq x \leq 1 \\ 0 & \text{otherwise}\end{cases}$$ 

$$f_Y(y)=\int_{-\infty}^{\infty} f_{XY}(s,y)ds$$

If $$0 \leq y \leq 1$$
$$f_Y(y)=\int_{-\infty}^{\infty}f_{XY}(s,y)ds$$

$$=\int_{y}^{1}2ds=2(1-y)$$

$$f_Y(y)=\begin{cases} 2(1-y) & 0 \leq y \leq 1\\ 0 & \text{otherwise}\end{cases}$$



#### Example

$$f_{XY}(x,y)=\begin{cases} ce^{-x}e^{-y} & 0 \leq y \leq x < \infty \\ 0 & \text{otherwise}\end{cases}$$

![image-20241030222355902](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030222355902.png)

$$\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f_{XY}(s,t)dsdt=1$$

$$=\int_{0}^{\infty} \int_{0}^{s} f_{XY}(s,t) dtds$$

$$=\int_{0}^{\infty}\int_{0}^{s} ce^{-s}e^{-t}dtds$$

$$=c/2$$

$$c=2$$

$$f_X(x)=\int_{-\infty}^{\infty}f_{XY}(x,t)dt$$

$$=\int_{0}^{x }2e^{-x}e^{-t}dt $$       - if $$x \geq 0$$

$$=2e^{-x} \int_{0}^{x} e^{-t}dt$$

$$=2e^{-x} (1-e^{-x})$$

$$f_X(x)=\begin{cases} 2e^{-x}(1-e^{-x}) & x \geq 0 \\ 0 & \text{otherwise}\end{cases}$$

$$f_Y(y)=\int_{-\infty}^{\infty}f_{XY}(s,y)ds$$

$$=\begin{cases} \int_{y}^{\infty} 2e^{-s }e^{-y} ds=2e^{-2y} &  y \geq 0 \\0 & y<0 \end{cases}$$

$$P(X>10,Y>10)=\int_{10}^{\infty} \int_{10}^{\infty}f_{XY}(s,t)dtds$$

$$=\int_{10}^{\infty} \int_{10}^{\infty}2e^{-s}e^{-t} dtds$$

$$P(X^2+Y^2 \leq 1)=\int \int_{circle} f_{XY}(s,t)dtds$$

![image-20241030222946414](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030222946414.png)

$$f_{XY}(x,y)=\begin{cases} 2e^{-x}e^{-y} & 0\leq y \leq x < \infty\\0 & \text{otherwise}\end{cases}$$

![image-20241030223048642](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241030223048642.png)

$$P(X+Y \leq 1)=\int\int f_{XY} (s,t)dtds$$

$$=\int\int f_{XY}(s,t) dsdt$$

$$=\int_{0}^{1/2} \int_{t}^{1-t} 2e^{-s} e^{-t} dsdt$$

$$=\int\int_{triangle}f_{XY}(s,t)dtds$$

$$=\int_{0}^{1/2} \int_{0}^{s} f_{XY}(s,t)dtds+\int_{1/2}^{1} \int_{0}^{1-s} f_{XY}(s,t)dtds$$

------

Recall that every event $$C$$ and $$D$$ are independent if

$$P(C \bigcap D)=P(C)P(D)$$

Independent RVs:

Definition: Two RVs $$X$$ and $$Y$$ are independent if for all subset $$B_1,B_2$$ of $$\R$$ the events $$C=\{X \in B_1\}$$ and $$D=\{Y \in B_2\}$$ are independent 

$$P(X \in B_1, X \in B_2)=P(X \in B_1)P(Y \in B_2)$$ for all $$B_1,B_2$$ which hare subset of $$\R$$

Suppose $$X,Y$$ are independent RV

$$P(X \in (-\infty,a), Y\in (-\infty,b))=P(X \in (-\infty,a))P(Y \in (-\infty,b))$$

$$P(a < X \leq b, Y>d)=P(a<X \leq b)P(Y >d)$$

------

Two discrete RVs

Thm:

Two discrete RVs $$X$$ and $$Y$$ are independent if and only if 

$$P_{XY}(x,y)=P_X(x)P_Y(y)$$ for all $$x \in S_x, y \in S_y$$

Proof: 

Suppose $$X$$ and $$Y$$ are independent 

$$B_1=\{x\}, B_2=\{y\}$$

$$P(X\in B_1, Y \in B_2)=P(X \in B_1)P(Y \in B_2)$$

$$P(X=x,Y=y)=P(X=x)P(Y=y)$$

$$P_{XY}(x,y)=P_X(x)P_Y(y)$$

Suppose the joint PMF factorizes into individual PMF

Consider any subsets $$B_1,B_2$$ of $$\R$$

$$P(X \in B_1,Y\in B_2)=\sum_{x\in B_1, y \in B_2} P_{XY}(x,y)$$

$$=\sum_{y\in B_2} \sum_{x \in B_1}P_X(x)P_Y(y)$$

$$=\sum_{y\in B_2} P(X \in B_1)P_Y(y)$$

$$=P(X \in B_1)P(Y \in B_2)$$

## Week 10 Session 2

### Jointly Continuous RVs

Definition: $$X$$ and $$Y$$ are jointly continuous if:

1. $$F_{XY}$$ is continuous function

2. $$F_{XY}(x,y)= \int_{-\infty}^{x}\int_{-\infty}^{y} f_{XY}(s,t)dtds$$

   ![image-20241101212408325](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241101212408325.png)

   where $$f_{XY}(s,t)$$ is the joint probability density function of $$X$$ and $$Y$$

$$P((X,Y)\in B)=\int \int_{B}f_{XY}(s,t)dsdt$$

![image-20241101212356394](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241101212356394.png)

$$P(a<X \leq b, c <Y \leq d)=\int_{c}^{d} \int_{a}^{b} f_{XY}(s,t)dsdt$$

### Independent RVs

$$P(X \in B_1, Y \in B_2)=P(X \in B_1) P(Y \in B_2)$$ for all $$B_1, B_2$$ which are subsets of $$\R$$

Thm1:

Two discrete RVs $$X$$ and $$Y$$ are independent if and only if 

$$P_{XY}(x,y)=P_X(x)P_Y(y)$$ for all $$x \in S_X, y \in S_Y$$

------

$$X,Y$$ are independent

$$P(X =x|Y=y)=\frac{P(X=x,Y=y)}{P(Y=y)}$$

$$=\frac{P(X=x)P(Y=y)}{P(Y=y)}$$

$$=P(X=x)$$

$$P(X \leq 10 | 2 \leq Y \leq 4)=\frac{P(X \leq 10, 2 \leq Y \leq 4)}{P(2 \leq Y \leq 4)}$$

$$=P(X \leq 10)$$

------

#### Example

$$Q,R$$

$$S_Q=\{0,1,2,...\}$$

$$S_R=\{0,1\}$$

$$P_{QR}(q,r)=(1-p)p^{2q+r}$$

Are $$Q$$ and $$R$$ independent?

$$P_Q(q)=(1-p) (p^{2q+0}+p^{2q+1})$$

$$=(1-p)p^{2q}(1+p)$$

$$P_R(r)=\sum_{q \geq 0} (1-p) p^r p^{2q}$$

$$=(1-p) p^r \frac{1}{1-p^2}$$

$$=\frac{p^r}{1+p}$$

$$P_Q(q) P_R(r)=(1-p)p^{2q}(1+p) \frac{p^r}{1+p}$$

$$=(1-p)p^{2q+r}$$

$$=P_{QR}(q,r)$$

Therefore $$Q$$ and $$R$$ are independent

------

Thm 2:

For any RVs $$X,Y$$, two RVs are independent if and only if 

$$F_{XY}(x,y)=F_X(x)F_Y(y)$$ for all $$x \in \R, y \in \R$$

------

Thm 3:

Suppose $$X,Y$$ are jointly continuous RVs. $$X,Y$$ are independent if and only if

$$f_{XY}(x,y)=f_X(x) f_Y(y)$$ for all $$x\in \R, y \in \R$$

Proof of Thm3:

Suppose $$X,Y$$ are independent, jointly continuous RVs

$$F_{XY}(x,y)=F_X(x)F_Y(y)$$

$$f_{XY}(x,y)=\frac{d}{dx} (\frac{d}{dy} F_{XY}(x,y))$$

$$=\frac{d}{dx} \frac{d}{dy} F_X(x) F_Y(y)$$

$$=\frac{d}{dx} F_X(x) \frac{d}{dy} F_Y(y)$$

$$=f_X(x) f_Y(y)$$

Then, $$f_{XY}(x,y)=f_X(x) f_Y(y)$$



Suppose $$f_{XY}(x,y)=f_X(x) f_Y(y)$$ is true

$$F_{XY}(x,y)=\int_{-\infty}^{x} \int_{-\infty}^{y} f_{XY} (s,t)dtds$$

$$=\int_{-\infty}^{x} \int_{-\infty}^{y} f_X(s)f_Y(t)dtds$$

$$=\int_{-\infty}^{x}f_X(s)ds \int_{-\infty}^{y}f_Y(t)dt$$
$$=F_X(x)F_Y(y)$$

Therefore, $$X,Y$$ are independent

------

#### Example

$$f_{XY}(x,y)=\frac{1}{2 \pi} e^{-\frac{x^2+y^2}{2}}$$ for $$x \in \R, y \in \R$$

Are $$X,Y$$ independent?

$$f_X(x)=\int_{-\infty}^{\infty}f_{XY}(x,t)dt$$

$$=\frac{1}{2 \pi} \int_{-\infty}^{\infty}e^{-\frac{x^2}{2}} e^{-\frac{y^2}{2}} dt$$

Note that:

$$\mathcal{N}(0,1)$$

$$f_Y(y)=\frac{e^{-\frac{y^2}{x}}}{\sqrt{2 \pi}}=1$$

$$=\frac{1}{2 \pi} e^{-\frac{x^2}{2}}  \sqrt{2 \pi} \int_{-\infty}^{\infty} \frac{1}{\sqrt{2 \pi}}e^{-\frac{y^2}{2}} dt$$

$$=\frac{1}{\sqrt{2 \pi}} e^{-\frac{x^2}{2}} $$

$$f_Y(y)=\frac{1}{\sqrt{2 \pi}} e^{-\frac{y^2}{2}} $$

$$f_X(x) f_Y(y)=\frac{1}{2 \pi} e^{-\frac{x^2}{2}} e^{-\frac{y^2}{2}}=f_{XY}(x,y)$$

$$X,Y$$ are independent

$$X \sim \mathcal{N}(0,1)$$
$$Y \sim \mathcal{N}(0,1)$$

IID RVs (intendent and identically distributed RVs)

$$f_{XY}(x,y)=\frac{1}{2 \pi} e^{-\frac{x^2+y^2}{2}}$$



$$P(X > 0, Y < 0)$$

![image-20241101215656721](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241101215656721.png)

As $$X \sim \mathcal{N}(0,1)$$

![image-20241101215719437](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241101215719437.png)

$$P(X>0)=\frac{1}{2}$$

$$P(X > 0, Y < 0)=P(X>0)P(Y<0)=\frac{1}{2}\cdot \frac{1}{2}=\frac{1}{4}$$

#### Example

$$F_{XY}(x,y)=(1-e^{-\alpha x})(1-e^{-\beta y}), x, y \in \R, \alpha>0, \beta>0$$ and they are constants

Are $$X,Y$$ independent?

$$F_X(x)=\lim_{y \rightarrow \infty}F_{XY}(x,y)=1-e^{-\alpha x}$$

$$F_Y(y)=\lim_{x \rightarrow \infty}F_{XY}(x,y)=1-e^{-\beta y}$$

Note:

$$F_{XY}(x,y)=P(X \leq x, Y \leq y)$$

$$\lim_{y \rightarrow \infty}$$

$$F_X(x)=P(X \leq x)$$

$$F_{XY}(x,y)=F_X(x)F_Y(y)$$

------

#### Example

$$H, \Theta$$ are independent RVs

$$H \sim \text{Uniform}[0,\frac{1}{2}] \rightarrow f_{H}(h)=\begin{cases}2 & 0 \leq h \leq \frac{1}{2}\\ 0 & \text{otherwise}\end{cases}$$

$$\Theta \sim \text{Uniform}[0, \frac{\pi}{2}]\rightarrow f_{\Theta}(\theta)=\begin{cases}\frac{2}{\pi} & 0 \leq \theta \leq \frac{\pi}{2}\\ 0 & \text{otherwise}\end{cases}$$

$$f_{H \Theta}(h,\theta)=\begin{cases} \frac{4}{\pi} & 0\leq h \leq \frac{1}{2}, 0 \leq \theta \leq \frac{2}{\pi} \\ 0 & \text{otherwise}\end{cases}$$

$$P(H \leq \frac{\sin(\theta)}{2})=\int_{0}^{\frac{\pi}{2}} \int_{0}^{\frac{\sin{\theta}}{2}}f_{H\Theta}(h,\theta)dh d\theta$$

$$=\int_{0}^{\frac{\pi}{2}} \int_{0}^{\frac{\sin{\theta}}{2}}\frac{4}{\pi}dh d\theta$$

$$=\frac{4}{\pi} \int_{0}^{\frac{\pi}{2}} \frac{\sin{\theta}}{2}d\theta$$

$$=\frac{2}{\pi} (-\cos{\theta})|_0^{\frac{\pi}{2}}$$

$$=\frac{2}{\pi}$$

------

Theorem:

Suppose $$X,Y$$ are independent

$$Z=g(X)$$ and $$W=h(Y)$$

Then, $$Z,W$$ are independent

Proof:
$$P(Z \in B_1, W \in B_2)=P(g(X) \in B_1, h(Y) \in B_2)$$

$$g^{-1}(B_1)=\{x:g(x) \in B_1\}$$

$$h^{-1}(B_2)=\{y:g(y) \in B_2\}$$

$$=P(X \in g^{-1}(B_1), Y \in h^{-1}(B_2))$$

$$=P(X \in g^{-1}(B_1))P( Y \in h^{-1}(B_2))$$

$$=P(g(X)\in B_1)P(h(Y) \in B_2)$$

$$=P(Z \in B_1)P(H \in B_2)$$

Therefore, $$Z,W$$ are independent

Previous example

$$H, \Theta$$ are independent

$$W=\sin{\theta}$$

$$H,W$$ are independent

------

### Expected Value of functions of RVs

1. If $$X$$ is a discrete RV

   $$Z=g(X)$$

   $$E[Z]=\sum_{x \in S_X} g(X) P_X(x)$$

2. If $$X$$ is a continuous RV

   $$Z=g(X)$$

   $$E[Z]=\int_{-\infty}^{\infty}g(x)f_X(x)dx$$

3. $$X,Y$$ are discrete RVs

   $$Z=g(X,Y)$$

   $$E[Z]=\sum_{x \in S_X} \sum_{y \in S_Y} g(x,y) P_{XY} (x,y)$$

4. $$X,Y$$ are jointly continuous

   $$Z=g(X,Y)$$

   $$E[Z]=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} g(x,y)f_{XY}(x,y)dxdy$$

#### Example

$$X,Y \rightarrow f_{XY}$$

$$Z=aX+bY, a\in \R, b \in \R$$

$$E[Z]=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} (ax+by) f_{XY}(x,y) dxdy$$

$$=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} axf_{XY}(x,y)dydx + \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} byf_{XY}(x,y)dxdy$$

$$=\int_{-\infty}^{\infty} axf_X(x)dx+ \int_{-\infty}^{\infty}by f_Y(y)dy$$

$$=aE[X]+bE[Y]$$

$$E[aX+bY]=E[aX]+E[bY]=aE[X]+bE[Y]$$

Linearity Property

$$E[X^3+Y^2]=E[X^3]+E[Y^2]$$

$$E[g(X)+h(y)]=E[g(X)]+E[h(Y)]$$

------

### Independence and expectation

#### Example

$$X,Y$$ are independent 

$$f_{XY}$$
$$Z=XY$$
$$E[Z]=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} xy f_{XY}(x,y)dxdy$$

$$=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} xy f_X(x) f_Y(y)dxdy$$

$$=\int_{-\infty}^{\infty}y f_Y(y)E[X]dy$$

$$=E[X]E[Y]$$



Thm:

If $$X,Y$$ are independent RVs

1. $$E[XY]=E[X]E[Y]$$
2. $$E[g(X)h(Y)]=E[g(X)]E[h(Y)]$$

------

#### Example

$$X=R, Y=R+1$$

$$R \sim \mathcal{N}(0,1)$$

$$X,Y$$ not independent RVs

$$E[XY]=E[R(R+1)]=E[R^2+R]=E[R^2]+E[R]=1+0$$

$$E[X]=0,E[Y]=1$$

$$E[XY] \neq E[X]E[Y]$$

------

$$n^{th}$$ moment of $$X$$ : $$E[X^n]$$

$$(n,k)$$ moment of $$X,Y$$ : $$E[X^n \cdot Y^k]$$

Suppose $$X,Y$$ are discrete

$$E[X^n \cdot Y^k]=\sum_{x \in S_X} \sum_{y \in S_Y} x^n y^k P_{XY}(x,y)$$

If $$X,Y$$ are jointly continuous

$$E[X^n \cdot Y^k]=\int \int x^ny^k f_{XY}(x,y)dxdy$$

------

Definition: 

Correlation, Covariance, and Correlation Coefficient

correlation between $$X \&Y=E[XY]$$

Covariance between $$X\&Y=Cov(X,Y)=E[(X-m_X)(Y-m_Y)]$$

Correlation coefficient between $$X\&Y=\rho_{XY}=\frac{Cov(X,Y)}{\sigma_X \sigma_Y}$$

------

$$Cov(X,X)=Var(X)$$

$$E[(X-m_X)(Y-m_Y)]=E[XY-m_XY-m_YX+m_Xm_Y]$$

$$=E[XY]-m_XE[Y]-m_YE[X]+m_Xm_Y$$

$$=E[XY]-m_Xm_Y$$

$$Cov(X,Y)=E[XY]-m_Xm_Y$$

#### Example

$$X,Y$$ are independent

$$Cov(X,Y)=E[XY]-m_Xm_Y$$

$$=E[X]E[Y]-m_Xm_Y=0$$

If $$X,Y$$ are independent $$\implies Cov(X,Y)=0$$

#### Example

$$X - m_X, \sigma_X^2$$

$$Y=aX+b$$ where $$a \neq 0, b \in \R$$

Find $$Cov(X,Y), \rho_{XY}=\frac{Cov(X,Y)}{\sigma_X \sigma_Y}$$

Case 1: $$a>0$$

$$Var(Y)=\sigma_Y^2=E[(Y-m_Y)^2]$$

$$=E[(aX+b-am_X-b)^2]$$
$$=a^2 \sigma_X^2$$

$$Cov(X,Y)=E[(X-m_X)(Y-m_Y)]=E[(X-m_X)(aX-am_X)]$$

$$=a \sigma_X^2$$

$$\rho_{XY}=\frac{a \sigma_X^2}{\sigma_X \sigma_Y}=\frac{a \sigma_X^2}{\sigma_X a\sigma_X}=1$$

Case 2: $$a<0$$
$$\sigma_Y^2=a^2 \sigma_X^2$$

$$\sigma_Y=(-a)\sigma_X$$

Standard deviation = positive square root of variance

$$m_Y=am_X+b$$

$$\rho_{XY}=\frac{a \sigma_X^2}{\sigma_X \sigma_Y}=\frac{a \sigma_X^2}{\sigma_X (-a)\sigma_X}=-1$$

#### Example

$$X,Y$$

$$m_X=m_Y=0$$

$$\sigma_X^2=4, \sigma_Y^2=9$$

$$Z=2X-Y, W=X+Y$$

$$m_Z=m_W=0$$

$$Cov(Z,W)=0$$

$$E[ZW]=E[(2X-Y)(X+Y)]$$

$$=E[2X^2-YX+2XY-Y^2]$$

$$=2E[X^2]+E[XY]-E[Y^2]$$

$$0=2 \cdot 2^2 +E[XY]- 3^2$$

$$E[XY]=1$$

$$Cov(X,Y)=E[XY]=1$$

## Discussion 10

### Continuous Random Variable

1. Beta
   1. Uniform (Special Case) $$\alpha_1 \beta=1$$

2. Gaussian (Normal) Distribution
3. Gamma $$(\alpha, \gamma)$$
   1. Exponential $$(\lambda)$$ when $$\alpha=1$$
   2. Chi-squared
   3. Erlang

4. Cauchy [expectation and variance is not defined]

Conditional Probability Models:

1. Conditional PDF of $$X$$ (continuous RV) given event $$B$$

   Memoryless property of exponential RV 

   $$f_{X|B}(x)=\begin{cases} \frac{f_X(x)}{P[B]} & x \in B \\ 0 & \text{otherwise}\end{cases}$$

2. $$E[X|B]=\int_{-\infty}^{\infty} x f_{X|B}(x)dx$$

   $$E[g(X)|B]=\int_{-\infty}^{\infty}g(x)f_{X|B}(x)dx$$

### Functions of a continuous RV

$$Y:=g(X)$$ where $$X$$ is a continuous RV

$$Y$$ can be continuous, discrete or mixed RV depending on the properties of $$g(\cdot)$$

Case 1: When $$g(\cdot)$$ is a piecewise constant function

![image-20241102104958096](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102104958096.png)

- $$Y$$ is a discrete RV

- $$S_Y(\text{range})$$ is a list of values

- PMF of $$Y$$ for each $$Y \in S_Y$$

  $$P_Y(y)=\int_{A_Y}f_X(x)dx$$

  where $$A_Y=\{x:g(x)=y\}$$ 

Case 2: $$g(\cdot)$$ is continuous and its derivative $$g'(\cdot)$$ is not zero on any interval

![image-20241102105050076](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102105050076.png)

- $$Y$$ is a continuous RV

  $$P[g(x) \leq y]$$

  $$P[x \leq g^{-1}(y)]$$

- CDF

  $$F_Y(y)=P[Y \leq y]=P[g(X) \leq y]=\int_{B_Y}f_X(x)dx$$

  where $$B_Y=\{x:g(x) \leq y\}$$

  $$f_Y(y)=\frac{d}{dy}F_Y(y)$$

Case 2*: $$g(\cdot)$$ is strictly monotonically increasing or decreasing function

$$f_Y(y)=f_X(h(x))|\frac{d}{dy}h(y)|$$

$$h(y)=g^{-1}(y)$$

### Concentration inequalities

1. Markov's Inequality

   For any non-negative RV $$X$$ and constant $$a$$

   $$P[X \geq a] \leq \frac{E[X]}{a}$$

2. Chebyshev's Inequality

   For any RV $$X$$ and constant $$a$$
   $$P[|X-E[X]| \geq a] \leq \frac{Var[X]}{a^2}$$

### Problem 1

![image-20241102105715772](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102105715772.png)

$$X: $$ weight of almond

$$Y:$$ weight of cashew

![image-20241102105824197](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102105824197.png)

$$P[X + Y \leq 0.5] =\int_{y=0}^{1/2} \int_{x=0}^{1/2-y} f_{XY}(x,y)dxdy$$

$$=\int_{y=0}^{1/2} \int_{x=0}^{1/2-y} 24xy dxdy$$

$$=\frac{1}{16}$$

$$f_Y(y)=\int_{x=0}^{1-y} 24xy dx$$

$$=24y \frac{x^2}{2}|_{0}^{1-y}$$

$$=12y(1-y)^2, 0 \leq y \leq 1$$

### Problem 2

If $$X$$ is a RV such that $$E[X]=3,E[X^2]=13$$. Given lower bond for $$P(-2 < x <8)$$

$$P[-2 <x <8]=P[-2-3<x-3<8-3]$$

$$=P[-5<x-3<5]$$

$$=P[|x-3|<5]$$

$$=1-P[|x-3| \geq 5]$$

$$=1-P[|x-E[X]|\geq a]$$

$$\leq 1- \frac{Var[X]}{5^2}=\frac{21}{25}$$

$$Var[X]=E[X^2]-(E[X])^2=13-3^2=4$$

### Problem 3

If $$X$$ is an exponential RV with parameter $$\lambda=1$$ Compute the PDF of RV $$Y$$ defined by $$Y:=\log{X}$$

$$X \sim \text{exp}( \lambda=1)$$

$$f_X(x)=\begin{cases} e^{-x} & x>0 \\ 0 & \text{otherwise}\end{cases}$$

$$F_Y(y)=P[Y \leq y]=P[\log{X} \leq y]$$

$$=P[x \leq e^y]$$

$$F_Y(y)=F_X(e^y)$$



Find CDF of $$X$$

$$F_X(x)=\int_{0}^{x}f_X(x)dx=\int_{0}^{x}e^{-x}dx$$

$$F_X(x)=1-e^{-x}$$

$$F_Y(y)=1-e^{-e^y}$$

$$f_Y(y)=\frac{d}{dy}[1-e^{-e^{y}}]=e^ye^{-e^y}$$

$$f_Y(y)=e^ye^{-e^y}, -\infty \leq y \leq \infty$$

### Problem 4

![image-20241102111508466](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241102111508466.png)

$$X \sim \text{Uniform}(15,45)$$ is a RV for man's arrival

$$Y \sim \text{Uniform}(0,60)$$$ is a RV for women's arrival

$$f_X(x)=\begin{cases} \frac{1}{30} & 15 \leq x \leq 45\\0 & \text{otherwise}\end{cases}$$

$$f_Y(y)=\begin{cases} \frac{1}{60} & 0 \leq x \leq 60\\0 & \text{otherwise}\end{cases}$$

$$P[|X-Y|<5]$$ - Joint PDF

$$f_{XY}(x,y)=f_X(x) f_Y(y)=\frac{1}{1800}$$

$$f_{XY}(x,y)=\begin{cases} \frac{1}{1800} & 16 \leq x \leq 45, 0 \leq y \leq 60 \\ 0 & \text{otherwise}\end{cases}$$

$$P[|X-Y|<5]=P[-5<x-y <5]$$

$$=P[x-5 < y < x+5]$$

$$=\int_{x=15}^{45} \int_{y=x-5}^{x+5} f_{XY}(x,y)dxdy$$

$$=\frac{1}{6}$$

$$P[|X-Y|<5]=\frac{1}{6}$$

Probability that man arrives first

$$P[X <Y]=\int_{-\infty}^{\infty} \int_{x}^{\infty} f_{XY}(x,y)dxdy$$

$$=\int_{x=15}^{45} \int_{y=x}^{60} \frac{1}{1800} dxdy$$

$$=\frac{1}{2}$$

## Week 11 Session 1 (Only 1)

### Expected value of functions of RVs

$$X,Y$$ are discrete RVs

$$Z=g(X,Y)$$
$$E[Z]=\sum_{x \in S_X} \sum_{y \in S_Y}P_{XY}(x,y)$$

$$X,Y$$ are jointly continuous

$$Z=g(X,Y)$$

$$E[Z]=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} g(x,y)f_{XY}(x,y)dxdy$$

Thm: If $$X,Y$$ are independent RVs

1. $$E[XY]=E[X]E[Y]$$
2. $$E[g(X)h(Y)]=E[g(X)]E[h(Y)]$$

### Correlation, Covariance and Correlation coefficient

Correlation between $$X$$ and $$Y$$ : $$E[XY]$$

Covariance between $$X$$ and $$Y$$ : $$E[(X-m_X)(Y-m_Y)]=E[XY]-m_Xm_y$$

Correlation coefficient between $$X$$ and $$Y$$ : $$\rho_{XY}=\frac{\text{Cov}(X,Y)}{\sigma_X \sigma_Y}$$

------

#### Example

$$X - m_X, \sigma_X^2$$

$$Y - m_Y, \sigma_Y^2$$ 

$$\rho_{XY}$$

$$Z=(\frac{X-m_X}{\sigma_X})+(\frac{Y-m_Y}{\sigma_Y})$$

$$E[Z]=E[\frac{X-m_X}{\sigma_X}]+E[\frac{Y-m_Y}{\sigma_Y}]=0$$

$$E[Z^2]=Var[Z]$$

$$=E[(\frac{X-m_X}{\sigma_X}+\frac{Y-m_Y}{\sigma_Y})^2]$$

$$=E[(\frac{X-m_X}{\sigma_X})^2+(\frac{Y-m_Y}{\sigma_Y})^2+2\frac{X-m_X}{\sigma_X}\frac{Y-m_Y}{\sigma_Y}]$$

$$=E[\frac{(X-m_X)^2}{\sigma_X^2}]+E[\frac{(Y-m_Y)^2}{\sigma_Y^2}]+2E[\frac{(X-m_X)(Y-m_Y)}{\sigma_X\sigma_Y}]$$

$$=1+1+2 \rho_{XY}$$

$$=2+2 \rho_{XY}$$

$$=E[Z^2] \geq 0$$
==$$\rho_{XY} \geq -1$$==

$$W=(\frac{X-m_X}{\sigma_X})-(\frac{Y-m_Y}{\sigma_Y})$$

$$E[W^2] \geq 0$$
==$$\rho_{XY} \leq 1$$==

==For any 2 RVs $$X$$ and $$Y$$, $$-1 \leq \rho_{XY} \leq 1$$==

#### Example

$$X,Y$$ are independent

$$\rho_{XY}=\frac{\text{Cov}(X,Y)}{\sigma_X \sigma_Y}=\frac{E[XY]-m_Xm_Y}{\sigma_X \sigma_Y}=0$$

For independent RVs, $$\rho_{XY}=0$$

#### Example

$$\Theta \sim \text{Uniform} (0,2 \pi)$$

$$X= \cos{\theta}, Y=\sin{\theta}$$

$$\rho_{XY}=\frac{\text{Cov}(x,y)}{\sigma_X \sigma_Y}$$

$$\text{Cov} (X,Y)=E[XY]-m_Xm_Y$$

$$m_X=E[X]=E[\cos{\theta}]=\int_{0}^{2\pi} \cos{\theta} \frac{1}{2 \pi}d \theta=0$$

$$m_Y=E[Y]=E[\sin{\theta}]=\int_{0}^{2\pi} \sin{\theta} \frac{1}{2 \pi}d \theta=0$$

$$E[XY]=E[\cos{\theta}\sin{\theta}]$$

$$=\int_{0}^{2\pi} \cos{\theta} \sin{\theta} \frac{1}{2 \pi} d \theta$$

$$=\frac{1}{2} \int_{0}^{2 \pi} \sin{2 \theta} \frac{1}{2 \pi}d \theta$$
$$=\frac{1}{2} \frac{1}{2 \pi} \frac{-\cos{2 \theta}}{2}|_{0}^{2 \pi}=0$$

$$\implies \text{Cov}(X,Y)=0$$

$$\implies \rho_{XY}=0$$

$$X= \cos{\theta}, Y=\sin{\theta}$$

![image-20241122181439348](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241122181439348.png)

$$P(X>0.9, Y>0.9)=0$$

$$P(X>0.9) >0 , P(Y>0.9)>0$$

$$X^2+Y^2=1$$

$$\implies P(X>0.9,Y>0.9) \neq P(X>0.9)P(Y>0.9)$$

$$\implies$$ not indepdent!

Thm: If $$X,Y$$ are independent $$\rho_{XY}=0$$
But converse is not true

Definition: If $$X,Y$$ have $$\rho_{XY}=0$$, then we say they are uncorrelated.

### Conditional Probability

Case 1. $$X$$ is a discrete RV

$$P(Y \in B|X=x)=\frac{P(Y \in B, X=x)}{P(X=x)}$$ if $$P(X=x) \neq 0$$
Suppose $$Y$$ is also discrete RV

$$P(Y=y|X=x)=\frac{P(Y=y, X=x)}{P(X=x)}$$

$$=\frac{P_{XY}(x,y)}{P_X(x)}$$

$$=P_{Y|X}(y|x)$$  - conditional PMF of $$Y$$ given $$X=x$$

Conditional PMF behaves like regular PMF 

For example

$$\sum_{y \in S_Y}P_{Y|X}(y|x)=1$$

$$P(Y \in B|X=x)=\sum_{y \in B} P_{Y|X}(y|x)$$

$$\sum_{y \in S_Y} P_Y(y)=1$$
$$P(Y \in B)=\sum_{y \in B}P_Y(y)$$



Law of total probability

$$S_X=\{x_1,...,x_n\}$$

$$P(Y\in B)=\sum_{i=1}^{n} P(Y \in B, X=x_i)$$

$$=\sum_{i=1}^{n} P(Y \in B|X=x_i)P(X=x_i)$$

Chain Rule

$$P(A \bigcap B)=P(A|B)P(B)$$

$$P(Y=y)=\sum_{i=1}^{n}P(Y=y|X=x_i)P(X=x_i)$$

==$$P_Y(y)=\sum_{i=1}^{n} P_{Y|X}(y|x_i)P_X(x_i)$$==

Chain Rule

$$P_{XY}(x,y)=P(Y=y, X=x)$$

$$=P(Y=y|X=x)P(X=x)$$

==$$P_{XY}(x,y)=P_{Y|X}(y|x)P_X(x)$$==

$$P_Y(y)=\sum_{i=1}^{n}P_{XY}(x_i,y)$$

------

If $$X,Y$$ are independent

$$P_{Y|X}(y|x)=\frac{P_{XY}(x,y)}{P_X(x)}=\frac{P_X(x)P_Y(y)}{P_X(x)}=P_Y(y)$$

#### Example

Memory chip with a random number of defects

$$X=$$ Number of defects

$$X \sim \text{Poisson} (\alpha)$$
$$P_X(k)=\frac{e^{-\alpha}\alpha^k}{k!}, k=0,1,2...$$

Each defect has a probability of $$p$$ of failing in the region $$R$$ of the chip. The location of each defect is independent from the location of other defects.

![image-20241122182705576](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241122182705576.png)

$$Y=$$ Number of defects in region $$R$$

1. Given $$X=k$$, what is the conditional PMF of $$Y$$?

   $$P(Y=0|X=k)=(1-p)^{k}$$

   $$P(Y=k|X=k)=p^k$$

   $$P(Y=j|X=k)=\binom{k}{j}p^j (1-p)^{k-j}$$

   $$0 \leq j \leq k$$
   $$P_{Y|X}(j|k)=\binom{k}{j} p^j (1-p)^{k-j}, 0\leq j\leq k$$

   $$P(Y=k+5|X=k)=0$$

2. PMF of $$Y$$

   $$P_Y(y)=\sum_{x=0}^{\infty} P_{Y|X}(y|x)P_X(x)$$
   Consider $$y \geq 1$$
   $$=\sum_{x=0}^{y-1} P_{Y|X}(y|x)P_X(x)+ \sum_{x=y}^{\infty}P_{Y|X}(y|x)P_X(x)$$

   $$=0+ \sum_{x=y}^{\infty} \binom{x}{y} p^y (1-p)^{x-y} e^{-\alpha} \frac{\alpha_x}{x!}$$

   $$=\sum_{x=y}^{\infty} \frac{x!}{y! (x-y)!} p^y (1-p)^{x-y} e^{-\alpha} \frac{\alpha_x}{x!}$$

   $$=\frac{\alpha^x}{y!} p^y \alpha^y \sum_{x=y}^{\infty} \frac{(1-p)^{x-y}}{(x-y)!} \alpha^{x-y}$$

   $$m=x-y$$

   $$=\frac{e^{-\alpha}(\alpha p)^y}{y!} \sum_{m=0}^{\infty} \frac{(1-p)^{m}\alpha^m}{n!}$$

   Note:: $$e^x=\sum_{m=0}^{\infty} \frac{x^m}{m!}$$

   $$=\frac{e^{-\alpha}(\alpha p)^y}{y!} e^{\alpha (1-p)}$$

   $$=e^{-\alpha p} \frac{(\alpha p)^y}{y!}$$

   $$P(Y=y)=e^{-\alpha p} \frac{(\alpha p)^y}{y!}, y \geq 1$$

   $$P(Y=0)=\sum_{x=0}^{\infty} P_{Y|X}(0|x)P_X(x)$$

   $$=\sum_{x=0}^{\infty}(1-p)^{x} e^{-\alpha} \frac{\alpha^x}{x!}$$

   $$=e^{-\alpha p}$$

   $$P(Y=y)=e^{-\alpha p} \frac{(\alpha p)^y}{y!}, y=0,1,2,...$$

   $$Y \sim \text{Poisson} (\alpha p)$$

   $$P_Y(y)=\sum_{x \in S_X} P_{Y|X}(y|x) P_X(x)$$

   $$\sum_{x \in S_X} P_{XY}(x,y)=\sum_{x \in S_X}P_{Y|X}(y|x)P_X(x)$$

3. Are $$X$$ and $$Y$$ independent?

   $$P_{XY}(x,y)=P_X(x)P_Y(y)$$?

   $$P_{Y|X}(y|x), P_Y(y)$$

   $$y=x+5$$
   $$P_Y(x+5)>0$$

   $$P_{Y|X}(y=x+5|x)=0$$

   $$P_{Y|X}(y|x)\neq P_Y(y)$$

   $$\implies X,Y$$ are not independent

------

 Suppose $$X$$ is a discrete RV

Conditional CDF of $$Y$$ given $$X=x$$

$$F_{Y|X}(y|x)=P(Y \leq y|X=x)$$

$$Y$$ can be discrete / continuous

Conditional CDF with fixed $$x$$ have properties of CDF

E.g.

$$F_{Y|X}(5|x) \leq F_{Y|X}(10|x)$$

$$F_{Y|X}(y|x)$$ is non-decreasing function of $$y$$

$$\lim_{y \rightarrow \infty}F_{Y|X}(y|x)=1$$

------

Suppose $$F_{Y|X}(y|x)$$ is differentiable in $$y$$

$$f_{Y|X}(y|x)=\frac{dF_{Y|X}(y|x)}{dy}$$

conditional density of $$Y$$ given $$X=x$$

$$f_Y(y)=\frac{dF_Y(y)}{dy}$$

Recall that: $$f_Y(y) h  \approx P(y <Y \leq y+h)$$ for small $$h$$

$$f_{Y|X}(y|x) h \approx P(y< Y \leq y+h|X=x)$$

Conditional densities of $$Y$$ with a fixed $$X=x$$ behave like regular densities

$$\int_{-\infty}^{\infty}f_{Y|X}(y|x)dy=1$$

$$\int_{-\infty}^{\infty}f_Y(y)dy=1$$

$$P(Y\in B|X=x)=\int_{B}f_{Y|X}(y|x)dy$$

$$P(Y \in B)=\int_{B} f_Y(y)dy$$

#### Example

![image-20241123152908745](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241123152908745.png)

$$Y=X+N$$

$$N \sim \mathcal{N}(0,1)$$

$$X=+1$$ or $$-1$$ 

$$X,N$$ are independent RVs

Conditional CDF of $$Y$$ given $$X=+1$$

$$F_{Y|X}(y|+1)=P(Y \leq y|X=+1)$$
$$=P(X+N \leq y |X=+1)$$

$$=P(N \leq y-1|X=+1)$$

$$=P(N \leq y-1)$$

$$=\phi(y-1)$$

$$f_{Y|X}(y|+1)=\frac{d}{dy} F_{Y|X}(y|+1)=\frac{d}{dy} \phi (y-1)$$
$$=\phi'(y-1)=\frac{1}{\sqrt{2 \pi}} e^{-\frac{(y-1)^2}{2}}$$

where $$\phi'=\frac{d\phi}{dy}=$$ standard normal density

#### Example

Two fair, 6-sided dice are rolled. Each roll is independent of other roll.

$$X=$$ minimum of the number on 2 dice

$$Y=$$ maximum of the number on 2 dice

Conditional PMF of $$Y$$ given that $$X=4$$
$$P_{Y|X}(y|4)=P(Y=y|X=4)=\begin{cases} 0 & y=1,2,3\\ \frac{P(Y=4,X=4)}{P(X=4)}=\frac{1/36}{P(X=4)} & y=4 \\ \frac{P(Y=5,X=4)}{P(X=4)}=\frac{2/36}{P(X=4)} & y=5 \\ \frac{2/36}{P(X=4)} & y=6 \end{cases}$$

$$\sum_{y=1}^{6}P_{Y|X}(y|4)=1$$

$$\implies P(X=4)=5/36$$

## Discussion 11

### Outlines

1. Midterm problems
2. Covariance, correlation and correlation coefficient

------

### Question 2

The CDF of $$Y$$ is given as follows:

$$F_{Y}(y)=\begin{cases} \frac{7-2e^{-2y} -5e^{-3y}}{7} & \text{if\:} y \geq 0 \\ 0 & \text{otherwise}\end{cases}$$

and joint CDF of $$X$$ and $$Y$$ is given as follows

$$F_{XY}(x,y)=\begin{cases} \frac{2}{7}(1-e^{-2y}) & \text{if\:} 2 \leq x< 3, y \geq 0 \\ \frac{7-2e^{-2y} -5e^{-3y}}{7} & \text{if\:} x\geq 3, y \geq 0 \\ 0 & \text{otherwise}\end{cases}$$

(a) Find the expected value of $$e^Y$$

Find $$E[e^{Y}]$$

$$f_{Y}(y)=\frac{d}{dy}F_{Y}(y)=\begin{cases} \frac{1}{7} (4e^{-2y}+15e^{-3y}) & y \geq 0 \\ 0 & \text{otherwise}\end{cases}$$

$$E[e^Y]=\int_{y=0}^{\infty} e^{y} f_Y(y)dy$$

$$=\int_{y=0}^{\infty} \frac{e^{Y}}{7} (4e^{-2y}+15e^{-3y}) dy$$

$$=\frac{1}{7} [-4e^{-y}-\frac{15}{2} e^{-2y}]|_{y=0}^{\infty}$$

$$=\frac{23}{14}$$

(b) What is the PDF of $$e^{Y}$$

$$Z=e^{Y}$$

Find $$f_{Z}(z)$$

$$g(\cdot)$$ is continuous function and derivative $$g'(\cdot)$$ exists

$$Z$$ is also a continuous RV

$$P(Z \leq z)=P(e^{Y}\leq z)=P(Y \leq \ln(z))$$

$$P(Z \leq z)=F_{Y}(\ln(z))$$

Take the derivative with respect to $$z$$

$$f_{Z}(z)=\frac{d}{dz} F_{Y}(\ln(z)) \frac{d}{dz} \ln(z)$$

$$=f_{Y}(\ln(z))\frac{1}{z}$$

$$=\begin{cases} \frac{1}{7} (4e^{-2\ln(z)}+15e^{-3\ln(z)})\frac{1}{z} & \ln(z) \geq 0 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{Z}(z)=\begin{cases} \frac{1}{7z} (4e^{-2\ln(z)}+15e^{-3\ln(z)}) & z \geq 1 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{Z}(z)=\begin{cases} \frac{4z^{-3}+15z^{-4}}{7}  & z \geq 1 \\ 0 & \text{otherwise}\end{cases}$$

(c) Find the CDF of $$X$$. What kind of random variable is $$X$$? If it is discrete, find its PMF. If it is continuous, find its PDF.

 $$F_{X}(x)=\lim_{y \rightarrow \infty} F_{XY}(x,y)$$

$$=P(X \leq x, Y \leq y)$$

$$=P(X\leq x, Y \leq \infty)$$

$$=P(X \leq x)$$

$$F_{X}(x)=\begin{cases} 2/7 & 2 \leq x < 3 \\ 1 & x \geq 3 \\ 0 & \text{otherwise}\end{cases}$$

Note: CDF is piecewise constant function

$$X$$ is a discrete RV

![image-20241127215643405](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127215643405.png)

$$P_{X}(x)=\begin{cases} 2/7 & x=2  \\ 5/7 & x = 3 \\ 0 & \text{otherwise}\end{cases}$$

### Question 3

$$X$$ is the input to a communication channel. $$X$$ takes values $$+1$$ or $$-1$$ with probability $$p$$ and $$1-p$$, respectively. The received signal $$Y$$ is the sum of $$X$$ and noise $$N$$ which has a Gaussian distribution with zero mean and variance $$\sigma^2=0.25$$. $$X$$ and $$N$$ are independent random variables

(a) Find the probability $$P(X=j, Y \leq y)$$. Your answer should be in terms of the standard Gaussian CDF.

$$Y=X+N$$

$$N \sim \mathcal{N}(0,0.25)$$

$$X,N$$ are independent

$$P(X=j,Y \leq y)$$

Case: $$X=-1$$

$$P(X=-1,Y \leq y)=P(X=-1, X+N \leq y)$$

$$=P(X=-1,N\leq y+1)$$

$$=P(X=-1)P(N\leq y+1)$$

$$=(1-p)P(\frac{N-0}{2 \cdot 0.25} \leq \frac{y+1}{2 \cdot 0.25})$$

$$=(1-p)\phi(\frac{y+1}{0.5})$$

$$\phi:$$ CDF of standard normal

$$=(1-p)\phi(2y+2)$$

$$P(X=+1, Y \leq y)=p \phi(2y-2)$$

$$P(X=-1,Y \leq y)=(1-p)\phi(2y+2)$$

(b) Find the PDF of $$Y$$. 

Find $$f_{Y}(y)$$

$$Y=X+N$$

$$F_{Y}(y)=P(Y \leq y)$$

$$=P(Y \leq y|X=-1)P(X=-1)+P(Y \leq y|X=+1)P(X=+1)$$

$$=P(Y \leq y|X=-1)+P(Y\leq y, X=+1)$$

$$F_{Y}(y)=p\phi(2y-2)+(1-p)\phi(2y+2)$$

Differentiate with respect to y

$$f_{Y}(z)=2p \phi'(2y-2) +2(1-p)\phi'(2y+2)$$

$$\phi'$$ is the standard Gaussian PDF

(c) Let $$p=0.5$$. Find the conditional probability that $$X=+1$$ given that$$ Y>0$$. Your answer should be in terms of the standard Gaussian CDF. 

$$P(X=+1|Y>0)=\frac{P(X=+1,Y>0)}{P(Y>0)}$$

$$=\frac{P(X=+1,X+N>0)}{P(Y>0|X=+1)P(X=+1)+P(Y>0|X=-1)P(X=-1)}$$

$$=\frac{P(X=+1)P(N>-1)}{P(Y>0,X=+1)+P(Y>0,X=-1)}$$

$$=\frac{p P(\frac{N-0}{2 \cdot 0.25} >-2)}{p(1-\phi(-2)) +(1-p)(1-\phi(2))}$$

where $$P(\frac{N-0}{2 \cdot 0.25} >-2)=1-\phi(-2)$$

$$=\frac{1-\phi(-2)}{2-(\phi(-2)+\phi(2))}=\phi(2)$$

### Question 5

Let $$X, Y$$ be independent, non-negative random variables with the same mean $$m$$ and the same variance $$\sigma^2$$. Moreover, the two random variables have the same CDF, i.e., $$F_{X}(x)= F_Y(x)$$ for all $$x \in \R$$.

(a) Let$$Z=\frac{X+Y}{2}$$, Find the mean and variance of $$Z$$. 

$$E[Z]=\frac{1}{2} (E[X]+E[Y])$$

$$E[Z]=m$$

$$Var[Z]=E[Z^2]-(E[Z])^2$$

$$=E[Z^2]-m^2$$

$$=E[(\frac{X+Y}{2})^2]-m^2$$

$$=\frac{1}{4}E[X^2+Y^2+2XY]-m^2$$

$$E[X^2]=Var[X]+(E[X])^2=\sigma^2+m^2$$

$$=\frac{1}{4}(2 \sigma^2 +2 m^2)-m^2$$

$$=\frac{\sigma^2}{2}$$

(b) Find upper bounds on the following probabilities:

(i) $$P(Z>m+3\sigma)$$ 

$$Z$$ is a non-negative RV, so we are using Markov inequality

$$P[Z>m+3\sigma]\leq \frac{E[X]}{m+3 \sigma}=\frac{m}{m+3\sigma}$$

(ii) $$P(|Z-m|>3\sigma)$$

$$P(Z-m>3\sigma) \leq \frac{Var[Z]}{(3\sigma)^2}=\frac{\sigma^2}{2 \cdot 9 \sigma^2}=\frac{1}{18}$$

$$P(Z-m > 3 \sigma) \leq \frac{1}{18}$$

$$P(|Z-m|>3 \sigma)\leq \frac{1}{18}$$

(c) Let us define $$M := \max(X,Y)$$. Find the CDF of $$M$$.

$$F_{M}(m)=P(M \leq m)=P(\max(X,Y) \leq m)$$

$$=P(\{X \leq m\} \bigcap \{Y \leq m\})$$

$$=P(X \leq m)P(Y \leq m)$$

$$F_M(m)=(F_X(m))^2$$

------

Covariance, Correlation and correlation coefficient

$$X,Y$$ be two RVs

1. Correlation

   $$E[XY]$$

2. Covariance

   $$Cov(X,Y)=E[(X-E[X])(Y-E[Y])]$$

   $$Cov(X,Y)=E[XY]-E[X]E[Y]$$

   Intuition: capture how $$X,Y$$ vary together

   Note:

   $$Cov(aX+b,cY+d)=ac Cov(X,Y)$$

   $$Var[X+Y]=Var[X]+Var[Y]+2Cov(X,Y)$$

3. Correlation Coefficient

   $$\rho_{XY}=\frac{Cov(X,Y)}{\sqrt{Var[X]Var[Y]}}$$

   $$-1 \leq \rho_{XY} \leq 1$$

   "scale invarion" version of covariance

$$X,Y$$ are uncorrelated if $$Cov(X,Y)=0 (\rho_{XY}=0)$$

If $$X,Y$$ are uncorrelated 

$$Var[X+Y]=Var[X]+Var[Y]$$

$$E[XY]=E[X]E[Y]$$

Independence $$\implies$$ uncorrelotedness

Uncorrelatedness does not implies independence

$$X,Y$$ are orthogonal if $$E[XY]=0$$

$$E[(X+Y)^2]=E[X^2]+E[Y^2]$$

------

#### Example

$$X,Y$$ has joint PDF

$$f_{X,Y}(x,y)=12x(1-x)y, 0<x<1,0<y<1$$

Find correlation and covariance of $$X,Y$$ Determine whether $$X,Y$$ are independent or uncorrelated or orthogonal.

$$E[XY]=\int_{x=0}^{1} \int_{y=0}^{1}xy 12x(1-x)ydxdy$$

$$=\int_{x=0}^{1} \int_{y=0}^{1} 12x^2(1-x)y^2dydx$$

$$=\int_{x=0}^{1} 12x^2 (1-x) \frac{y^3}{3}|_{y=0}^{1}dx$$

$$=\frac{1}{3}$$

which is not orthogonal

$$Cov(X,Y)=E[XY]-E[X]E[Y]$$

$$f_{X}(x)=\int_{y=0}^{1} f_{XY}(x,y)dy$$

$$=6x(1-x)$$
$$f_{Y}(y)=\int_{x=0}^{1}12x(1-x)ydx$$
$$=2y$$

$$E[X]=\int_{0}^{1} 6x^2(1-x)dx=1/2$$

$$E[Y]=\int_{0}^{1}2y^2dy=2/3$$

$$Cov(X,Y)=1/3-1/2 \cdot 2/3=0$$

Therefore, they are uncorrelated

Notice, $$f_{XY}(x,y)=f_{X}(x)f_{Y}(y)$$

So they are independent

## Week 12 Session 1

### Conditional PMF

$$X,Y$$ - Discrete RVs

$$P_{Y|X}(y|x)=P(Y=y|X=x)$$

Other notation: $$P_{Y}(y|x)$$

Conditional PMF behaves like regular PMF

For example

$$\sum_{y \in S_Y}P_{Y|X}(y|x)=1$$

$$P(Y \in B |X=x)=\sum_{y \in B}P_{Y|X}(y|x)$$

Law of total probability

$$P_Y(y)=\sum_{x_i \in S_X} P_{Y | X} (y|x_i) P(x_i)$$

### Conditional CDF

Suppose $$X$$ is a discrete RV

Conditional CDF of $$Y$$ given $$X=x$$

$$F_{Y|X}(y|x)=P(Y \leq y | X=x)$$

$$Y$$ can be discrete/ continuous

------

Conditioning on a continuous RV $$X$$
$$P(Y \leq y|X=x)=\frac{P(Y \leq y,X=x)}{P(X=x)}$$

$$P(X=x)=0=\int_{x}^{x}f_X(t)dt$$ 

the previous equation is not well-defined as $$X$$ is continuous

Conditional CDF by a limiting procedure $$X,Y$$ are jointly continuous $$f_{XY}(x,y) \rightarrow $$Joint PDF

$$F_{Y|X}(y|x)=\lim_{h \downarrow 0} P(Y \leq y|x<X\leq x+h)$$

$$=\lim_{h \downarrow 0} \frac{P(Y \leq y, x<X \leq x+h)}{P(x<X \leq x+h)}$$

$$=\lim_{h \downarrow 0} \frac{\int_{-\infty}^{y} \int_{x}^{x+h} f_{XY}(s,t)dsdt}{\int_{x}^{x+h} f_X(s)ds}$$

$$=\lim_{h \downarrow 0} \frac{\int_{-\infty}^{y} f_{XY}(x,t)h dt}{f_X(x) h}$$

$$=\int_{-\infty}^{y} \frac{f_{XY}(x,t)}{f_X(x)}dt$$

where it is $$F_{Y|X}(y|x)$$ is the conditional PDF of $$Y$$given $$X$$
==$$F_Y(y)=\int_{-\infty}^{y}f_Y(t)dt$$==

$$f_{Y|X}(y|x)=\frac{f_{XY}(x,y)}{f_X(x)}$$

------

$$F_{Y|X}(y)=\int_{-\infty}^{y} \frac{f_{XY}(x,t)dt}{f_X(x)}$$

$$f_{Y|X}(y)=\frac{d F_{Y|X}(y)}{dy}=\frac{f_{XY}(x,y)}{f_X(x)}$$

Conditional PMF

$$P_{Y|X}(y|x)=\frac{P(X=x,Y=y)}{P(X=x)}=\frac{P_{XY}(x,y)}{P_X(x)}$$

------

$$f_{Y|X}(y|x)dy \approx P(y < Y \leq y+dy | X \approx x)$$

$$f_Y(y)dy \approx P(y <Y \leq y+dy)$$

Conditional densities have properties of regular PDF

$$\int_{-\infty}^{\infty}f_Y(y)dy=1$$

$$\int_{-\infty}^{\infty}f_{Y|X}(y|x)dy=1$$

$$P(Y \in B)= \int_{B} f_Y(t)dt$$

$$P(Y \in B|X=x)=\int_{B} f_{Y|X}(y|x)dy$$

------

$$f_{Y|X}(y|x)=\frac{f_{XY}(x,y)}{f_X(x)}$$ where $$f_X(x) >0$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}$$ where $$f_Y(y)>0$$

Chain Rule for densities

$$f_{XY}(x,y)=f_{Y|X}(y|x)f_X(x)=f_{X|Y}(x|y)f_Y(y)$$

$$P_{XY}(x,y)=P_{Y|X}(y|x)P_X(x)$$

------

#### Example

$$f_{XY}(x,y)=\begin{cases} \frac{e^{-y} e^{-\frac{x}{y}}}{y} & \text{if\:} 0<x< \infty, 0 <y< \infty \\ 0 & \text{otherwise\:} \end{cases}$$

$$f_Y(y)=\int_{-\infty}^{\infty} f_{XY}(x,y)dx$$

$$=\int_{0}^{\infty}\frac{e^{-\frac{x}{y}e^{-y}}}{y}dx $$    if $$y>0$$
$$=e^{-y}$$

$$f_Y(y)=\begin{cases} e^{-y} & \text{if\:} y>0 \\ 0 & \text{otherwise}\end{cases}$$

Fix $$y>0$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}$$

$$=\begin{cases} \frac{e^{-y} e^{-\frac{x}{y}}}{y e^{-y}}=\frac{e^{-\frac{x}{y}}}{y} & \text{if\:} x> 0\\ 0 & \text{if\:} x \leq 0\end{cases}$$

Fix $$y>0$$

$$P(X>1|Y=y)=\int_{1}^{\infty} f_{X|Y}(x|y)dx$$

$$=\int_{1}^{\infty} \frac{1}{y} e^{-\frac{x}{y}}dx$$

$$=e^{-\frac{1}{y}}$$

$$\text{exp} (\lambda)$$

$$P(X>1)=e^{-\lambda}$$

#### Example

Stick of length $$l$$
Break it at a point $$X \sim \text{uniform} (0,l)$$

Suppose $$X=x$$

![image-20241115190117956](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241115190117956.png)

Take the left part

Break it at point $$Y \sim \text{uniform}(0,x)$$

![image-20241115190157667](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241115190157667.png)

$$f_X(x)=\begin{cases} \frac{1}{l} & 0< x < l \\ 0 & \text{otherwise}\end{cases}$$

Suppose $$0<x < l$$

$$f_{Y|X}(y|x)=\begin{cases} \frac{1}{x} & 0<y<x \\ 0 & \text{otherwise}\end{cases}$$

$$f_{XY}(x,y)=f_{Y|X}(y|x)f_X(x)$$

$$=\begin{cases} \frac{1}{lx} & 0<y<x<l \\ 0 & \text{otherwise}\end{cases}$$

Density of $$Y$$

$$S_Y=(0,l)$$

$$0<y<l$$
$$f_Y(y)=\int_{-\infty}^{\infty} f_{XY}(x,y)dx =\int_{y}^{l} \frac{1}{lx} dx$$

$$=\frac{1}{l} (\log(l)-\log(y))$$

$$f_Y(y)=\begin{cases} \frac{1}{l} (\log(l)-\log(y)) & 0<y<l \\ 0 & \text{otherwise} \end{cases}$$
Fix $$0<y<l$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}$$

$$=\begin{cases} \frac{1}{x(\log(l)-\log(y))} & 0<y<x<l \\ 0 & \text{otherwise}\end{cases}$$

------

Thm: $$X,Y$$ are jointly continuous $$f_{XY}(x,y)$$

$$P(Y \in (a,b))=\int_{-\infty}^{\infty} P(Y \in (a,b)|X=x)f_X(x)dx$$

$$P(Y \in B)=\int_{-\infty}^{\infty} P(Y \in B|X=x)f_X(x)dx$$

Discrete

$$P(Y \in (a,b)=\sum_{x_i \in S_X} P(Y \in (a,b)|X=x_i)P(X=x_i))$$

Proof:

$$P(Y \in (a,b))=P(a<Y< b, -\infty < X < \infty)$$

$$=\int_{-\infty}^{\infty} \int_{a}^{b} f_{XY}(s,t)dtds$$

$$=\int_{-\infty}^{\infty} \int_{a}^{b} f_{Y|X}(t|s)f_X(s)dtds$$

$$=\int_{-\infty}^{\infty} (\int_{a}^{b} f_{Y|X}(t|s)dt) f_X(s)ds$$

$$=\int_{-\infty}^{\infty} (P(a<Y<b|X=s)) f_X(s)ds$$

$$=\int_{-\infty}^{\infty} (P(Y\in(a,b)|X=s)) f_X(s)ds$$

------

### Corollary

$$F_Y(y)=P(Y \leq y)=\int_{-\infty}^{\infty} P(Y \leq y |X=x)f_X(x)dx$$

$$=\int_{-\infty}^{\infty} F_{Y|X}(y|x)f_X(x)dx$$

#### Example

$$f_{XY}(x,y)=\begin{cases} 2e^{-x}e^{-y} & 0 \leq y \leq x \\ 0 & \text{otherwise}\end{cases}$$

$$f_X(x)=\begin{cases} 2e^{-x} (1-e^{-x}) & \text{if\:} x \geq 0 \\ 0 & \text{otherwise}\end{cases}$$

$$f_Y(y)=\begin{cases} 2 e^{-2y} & \text{if\:} y \geq 0 \\ 0 & \text{otherwise}\end{cases}$$

Fix $$y \geq 0$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}$$

$$=\begin{cases} \frac{2e^{-x} e^{-y} }{2e^{-2y}}=e^{-(x-y)} & \text{if\:} x \geq y\\ 0 & \text{otherwise}\end{cases}$$

Fix $$x \geq 0$$
$$f_{Y|X}(y|x)=\frac{f_{XY}(x,y)}{f_X(x)}$$

$$=\begin{cases} \frac{2e^{-x} e^{-y} }{2e^{-x}(1-e^{-x})} & \text{if\:} x \geq y\\ 0 & \text{otherwise}\end{cases}$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}=\begin{cases} \frac{2e^{-x} e^{-y} }{2e^{-2y}}=e^{-(x-y)} & x\geq y\\ 0 & \text{otherwise}\end{cases}$$

$$P(X \geq 2 | Y=1)=\int_{2}^{\infty}f_{X|Y}(x|1)dx$$

$$=\int_{2}^{\infty} e^{-(x-1)}dx$$

$$P(X \geq 2 |Y=3)=\int_{2}^{\infty} f_{X|Y} (x|3)dx$$

$$=\int_{2}^{\infty} e^{-(x-3)}dx$$

#### Example

$$X \sim \text{Uniform}(0,1)$$

Given that $$X=x, 0<x<1, Y \sim \text{Uniform}(0,x)$$

Find CDF of $$Y$$

$$0<y<1$$

$$S_Y=(0,1)$$

$$F_Y(y)=\begin{cases} 0 & y< 0\\ 1 & y \geq 1\end{cases}$$

$$F_Y(y)=P(Y \leq y)$$

$$=\int_{-\infty}^{\infty}P(Y \leq y|X=x)f_X(x)dx$$

$$=\int_{0}^{1}P(Y \leq y|X=x)dx$$

$$P(Y \leq y|X=x)$$

$$0<x<1$$
$$f_{Y|X}(y|x)=\begin{cases} \frac{1}{x} & 0< y< x \\ 0 & \text{otherwise}\end{cases}$$

$$P(Y \leq y|X=x)=\int_{-\infty}^{y} f_{Y|X}(t|x)dt$$

$$=\begin{cases} 0 & y\leq 0 \\ \frac{y}{x} & 0<y<x \\ \int_{0}^{x}f_{Y|X}(t|x)dt + \int_{x}^{y}f_{Y|X}(t|x)dt & y \geq x\end{cases}$$

$$0<y<1$$

$$F_Y(y)=\int_{0}^{1} P(Y \leq y|X=x)dx$$

$$=\int_{0}^{y}1dx+\int_{0}^{1}\frac{y}{x}dx$$

$$=y-y \log(y)$$            - $$0<y<1$$

$$F_Y(y)=\begin{cases} 0 & y\leq 0 \\ y-y \log(y) &0<y<1 \\ 1 & y \geq 1\end{cases}$$

$$f_Y(y)=\frac{dF_Y(y)}{dy}=\begin{cases} -\log(y) & 0<y<1 \\ 0 & \text{otherwise}\end{cases}$$

------

$$Y$$ - Continuous RV

$$E[Y]=\int_{-\infty}^{\infty}y f_Y(y)dy$$

$$X,Y$$ jointly continuous RV

$$f_{Y|X}(y|x)$$

Conditional expectation of $$Y$$ given $$X=x$$
$$E[Y|X=x]=\int_{-\infty}^{\infty} y f_{Y|X}(y|x)dy$$

Discrete case

$$E[Y]=\sum_{y \in S_Y} y P_Y(y)$$

$$E[Y|X=x]=\sum_{y \in S_Y}y P_{Y|X}(y|x)$$

------

Thm: Law of total expectatation

$$X,Y$$ are jointly continuous

$$E[Y]=\int_{-\infty}^{\infty} E[Y|X=x]f_X(x)dx$$

Proof: 

$$\int_{-\infty}^{\infty} E[Y|X=x]f_X(x)dx$$

$$=\int_{-\infty}^{\infty} (\int_{-\infty}^{\infty}yf_{Y|X}(y|x)dy) f_X(x)dx$$

$$=\int_{-\infty}^{\infty} \int_{\infty}^{\infty} y f_{Y|X}(y|x)f_X(x)dxdy$$

$$=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty}y f_{XY}(x,y)dxdy$$

$$=\int_{-\infty}^{\infty}y f_Y(y)dy$$
$$=E[Y]$$

Thm: $$X,Y$$ discrete

$$E[Y]=\sum_{x\in S_X}E[Y|X=x]P_X(x)$$

------

#### Example

Discrete $$X,Y$$

Joint PMF

| Y\X  | -1   | 0    | 1    |
| ---- | ---- | ---- | ---- |
| -1   | 0    | p    | 0    |
| 0    | p    | 0    | p    |
| 1    | 0    | p    | 0    |

$$p=\frac{1}{4}$$

$$E[Y|X=-1]=\sum_{y \in S_Y} y P_{Y|X}(y|-1)$$

$$P_{Y|X}(y|-1)=\frac{P_{XY}(-1,y)}{P_X(-1)}$$

$$=\begin{cases} 1 & y=0 \\ 0 & \text{otherwise}\end{cases}$$

$$E[Y|X=-1]=0$$
$$E[Y|X=0]=\sum_{y \in S_Y}y P_{Y|X}(y|0)$$

$$=(-1)P_{Y|X}(-1|0) + (0) P_{Y|X}(0|0)+(1)P_{Y|X}(1|0)$$

$$=0$$

#### Example

$$x>0$$
$$f_{Y|X}(y|x)=\begin{cases} \frac{1}{x} & 0<y<x \\ 0 & \text{otherwise}\end{cases}$$

$$E[Y|X=x]=\int_{-\infty}^{\infty} y f_{Y|X}(y|x)dy$$

$$=\int_{0}^{x} y \frac{1}{x}dy=\frac{x}{2}$$

$$f_X(x)=\begin{cases} 1 & 0< x<1 \\ 0 & \text{otherwise}\end{cases}$$

$$E[Y]=\int_{-\infty}^{\infty}E[Y|X=x]f_X(x)dx$$

$$=\int_{0}^{1}\frac{x}{2}dx=\frac{1}{4}$$

#### Example

$$X \sim \text{Posson} (\alpha)$$

$$E[Z]=\alpha$$

Given $$X=k, (k=0,1,2,...)$$

$$Y \sim \text{Binomial}(k,p)$$

Recall: $$E[Z]=np$$

$$E[Y]=\sum_{k \geq 0}E[Y|X=k]P_X(k)$$

$$=\sum_{k \geq 0} kp P_X(k)$$
$$=p \sum_{k \geq 0} k P_X(k)$$

$$=p \alpha$$

#### Example

$$X=+1 \rightarrow p=1/3$$

$$X=-1 \rightarrow p = 2/3$$

Given $$X=+1, Y \sim \mathcal{N}(1,1)$$

Given $$X=-1, Y \sim \mathcal{N}(-1,1)$$

$$E[Y]=\sum_{x \in S_X}E[Y|X=x]P_X(x)$$
$$=(1) \frac{1}{3} + (-1) \frac{2}{3}$$

## Week 12 Session 2

### Conditional PDF

$$f_{Y|X}(y|x)=\frac{f_{XY}(x,y)}{f_X(x)}$$ where $$f_X(x)>0$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}$$ where $$f_Y(y)>0$$

------

Thm:

$$X,Y$$ are jointly continuous with $$f_{XY}(x,y)$$

$$P(Y \in (a,b))=\int_{-\infty}^{\infty}P(Y \in (a,b)|X=x)f_X(x)dx$$

$$P(Y \in B)=\int_{-\infty}^{\infty}P(Y \in B|X=x)f_X(x)dx$$

------

Thm: Law of total expectation

$$X,Y$$ are jointly continuous

$$E[Y]=\int_{-\infty}^{\infty}E[Y|X=x]f_X(x)dx$$

$$X$$ is continuous, $$Y$$ is discrete

$$E[Y]=\int_{-\infty}^{\infty}E[Y|X=x]f_X(x)dx$$

------

Thm:

$$X,Y$$ discrete

$$E[Y]=\sum_{x\in S_X} E[Y|X=x]P_X(x)$$
$$X$$ discrete, $$Y$$ continuous

$$E[Y]=\sum_{x \in S_X}E[Y|X=x]P_X(x)$$

------

### Functions of 2 RVs

$$Z=X+Y$$

$$E[Z]=E[X]+E[Y]$$

$$Z=g(X,Y)$$

$$E[Z]=\int_{-\infty}^{\infty} \int_{\infty}^{\infty} g(x,y)f_{XY}(x,y)dxdy$$
$$Z=X+Y$$

$$F_Z(z)=P(Z \leq z)=P(X+Y \leq z)$$

$$=\int_{\infty}^{\infty} \int_{-\infty}^{z-s}f_{XY}(s,t)dtds$$

![image-20241116163202929](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241116163202929.png)

------

$$Z=X+Y$$

$$F_Z(z)=P(Z \leq z)$$

$$=\int_{-\infty}^{\infty}P(Z \leq z | X=x)f_X(x)dx$$
$$=\int_{-\infty}^{\infty}F_{Z|X}(z|x)f_X(x)dx$$

$$F_{Z|X}(z|x)=P(Z \leq z | X=x)$$
$$=P(X+Y \leq z | X=x)$$

$$=P(Y \leq z-x|X=x)$$

$$=\int_{-\infty}^{z-x}f_{Y|X}(t|x)dt$$

==$$F_{Z}(z)=\int_{-\infty}^{\infty} \int_{-\infty}^{z-x}f_{Y|X}(t|x)dt f_X(x)dx$$==

------

$$Z=g(X,Y)$$

$$F_{Z}(z)=P(g(X,Y) \leq z)$$
![image-20241116163602580](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241116163602580.png)

$$F_Z(z)=\int_{-\infty}^{\infty}F_{Z|X}(z|x)f_X(x)dx$$

Differentiate with respect to $$z$$

$$f_{Z}(z)=\int_{-\infty}^{\infty}f_{Z|X}(z|x)f_X(x)dx$$
Lemma: If $$X,Y,Z$$ are jointly continuous RVs and $$Z=g(X,Y)$$

==$$f_{Z}(z)=\int_{-\infty}^{\infty} f_{Z|X}(z|x)f_X(x)dx$$==

------

#### Example

$$X,Y$$ are independent exponential RVs with parameter $$\lambda=1$$
$$f_{X}(x)=\begin{cases} e^{-x} & x>0 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{Y}(y)=\begin{cases} e^{-y} & y>0 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{XY}(x,y)=f_X(x)f_Y(y)$$        - independence

$$=\begin{cases} e^{-x}e^{-y} & x>0,y>0 \\ 0 & \text{otherwise}\end{cases}$$

1. $$W=\frac{X}{3}=g(X)$$

   $$w=g(x)=\frac{x}{3}$$

   $$g^{-1}(w)=3w$$

   $$f_W(w)=\frac{f_X(g^{-1}(w))}{|\frac{dg(x)}{dx}|_{x=g^{-1}(w)}}$$

   ==$$f_W(w)=3f_X(3w)$$==

2. $$Z=\frac{X}{Y}$$

   $$f_Z(z)=\int_{-\infty}^{\infty}f_{Z|Y}(z|y)f_Y(y)dy$$

   ==$$f_Z(z)=\int_{0}^{\infty}f_{Z|Y}(z|y)e^{-y}dy$$==

Consider$$Y=y, 0< y < \infty$$

$$Z=\frac{X}{Y}=\frac{x}{y}$$
Given $$Y=y, Z=\frac{x}{y}$$ which is a linear function of $$X$$

$$f_{Z|Y}(z|y)=\frac{f_X(g^{-1}(z))}{|\frac{dg(x)}{dx}|_{x=g^{-1}(z)}}$$

$$Z=\frac{x}{y}$$

$$z=g(x)=\frac{x}{y}$$

$$g^{-1}(z)=yz$$

$$\frac{dg(x)}{dx}=\frac{1}{y}$$
$$f_{Z|Y}(z|y)=yf_X(yz)$$

$$f_Z(z)=\int_{0}^{\infty}yf_X(yz)e^{-y}dy$$

$$=\begin{cases} \int_{0}^{\infty}y e^{-yz}e^{-y}dy & z>0 \\ 0 & z\leq 0\end{cases}$$

------

$$Z_1=g_1(X,Y),Z_2=g_2(X,Y)$$

$$F_{Z_1Z_2}(z_1,z_2)=P(Z_1 \leq z_1, Z_2 \leq z_2)$$

$$=P(g_1(X,Y) \leq z_1, g_2(X,Y) \leq z_2)$$

$$=\int\int_{A}f_{XY}(s,t)dsdt$$

![image-20241116165146641](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241116165146641.png)

$$A=\{(x,y):g_1(x,y) \leq z_1, g_2(x,y) \leq z_2\}$$

------

#### Example

$$X,Y \rightarrow F_{XY}$$

$$Z= \max(X,Y), W=\min(x,y)$$

$$F_{ZW}(2,1)=P(Z \leq 2, W \leq 1)$$

$$=P(\max(X,Y) \leq 2, \min(X,Y) \leq 1)$$

![image-20241116165512237](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241116165512237.png)

$$P(\text{Red region})=F_{XY}(2,2)-P(R)$$

$$=F_{XY}(2,2)-[F_{XY}(2,2)+F_{XY}(1,1)-F_{XY}(2,1)-F_{XY}(1,2)]$$
$$=F_{XY}(2,1)+F_{XY}(1,2)-F_{XY}(1,1)$$

$$Z=\max(X,Y), W=\min(X,Y)$$

$$F_{ZW}(1,2)=P(Z \leq 1, W \leq 2)$$

$$=P(\max(X,Y)\leq 1, \min(X,Y)\leq 2)$$

$$=P(\max(X,Y) \leq 1)$$

$$=P(X\leq 1, Y \leq 1)= F_{XY}(1,1)$$

------

Linear function of 2 RVs

$$X,Y \rightarrow f_{XY}(x,y)$$
$$V=aX+bY, W=cX+dY$$

$$\begin{bmatrix} V \\ W \end{bmatrix}=\begin{bmatrix} a & b \\ c& d\end{bmatrix}\begin{bmatrix} X \\ Y \end{bmatrix}$$

$$\begin{bmatrix} V \\ W \end{bmatrix}=A\begin{bmatrix} X \\ Y \end{bmatrix}$$

Thm: Assume that $$A$$ is invertible

The joint PDF of $$V$$ and $$W$$ is given as

==$$f_{VW}=\frac{f_{XY}(A^{-1}\begin{bmatrix} V \\ W \end{bmatrix})}{|A|}$$==

------

#### Example

$$X,Y$$ independent and standard normal

$$V=X+Y, W=X$$
$$\begin{bmatrix} V \\ W \end{bmatrix}=\begin{bmatrix} 1 & 1 \\ 1& 0\end{bmatrix}\begin{bmatrix} X \\ Y \end{bmatrix}$$

$$A^{-1}=\begin{bmatrix} 0 & 1 \\ 1& -1\end{bmatrix}$$

$$f_{VW}(v,w)==\frac{f_{XY}(A^{-1}\begin{bmatrix} V \\ W \end{bmatrix})}{|A|}$$

$$=f_{XY}(w,v-w)$$

$$=f_X(w)f_Y(v-w)$$

$$=\frac{1}{\sqrt{2 \pi}} e^{-\frac{w^2}{2}} \cdot \frac{1}{\sqrt{2 \pi}} e^{-\frac{(v-w)^2}{2}}$$

#### Example

$$V=X+Y,W=X-Y$$

Find $$f_{VW}(v,w)$$

------

### Random Vector

$$\underline{X}=\begin{bmatrix}X_1 \\X_2 \\... \\X_n \end{bmatrix} $$ is a random vector

$$\underline{X}=\begin{bmatrix}X_1 \\X_2 \end{bmatrix}$$

![image-20241116170551843](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241116170551843.png)

$$P(\max(X_1, ... X_n)\leq 1)$$

$$P(X_1^2+X_2^2+... +X_n^2 \leq 1)$$

------

Joint CDF of $$\underline{X}=\begin{bmatrix}X_1 \\X_2 \\... \\X_n \end{bmatrix} $$

$$F_{XY}(x,y)=P(X \leq x ,Y \leq y)$$

$$F_{X_1,X_2,...,X_n}(x_1,...x_n)$$

$$F_{\underline{X}}(x_1, ..., x_n)=P(X_1 \leq x_n ... X_n \leq x_n)$$
$$\lim_{x_n \rightarrow \infty}F_{X_1...X_n}(x_1, ...x_n)$$

$$=\lim_{x_n \rightarrow \infty}P(X_1 \leq x_1, ... X_n \leq x_n)$$

$$=P(X_1 \leq x_1 ... X_{n-1}\leq x_{n-1}, X_n < \infty)$$

$$=P(X_1 \leq x_1 ... X_{n-1} \leq x_{n-1})$$

$$=F_{X_1...X_{N-1}} (x_1...x_{n-1})$$

$$\lim_{y \rightarrow \infty} F_{XY}(x,y)=P(X \leq x, Y < \infty)$$

$$=P(X \leq x)$$

$$=F_X(x)$$
$$\lim_{x_2, x_3, x_n \rightarrow \infty} F_{X_1...X_n}(x_1... x_n)=F_{X_1}(x_1)$$

$$\lim_{x_1\rightarrow \infty, x_4 \rightarrow \infty}F_{X_1X_2X_3X_4}(x_1,x_2,x_3,x_4)=F_{X_2X_3}(x_2, x_3)$$

------

### Joint PMF

$$X_1,...X_n$$ discrete RVs

$$P_{X_1...X_n}(x_1...x_n)=P(X_1=x_1...X_n=x_n)$$

$$P_{XY}(x,y)=P(X=x,Y=y)$$

$$\sum_{x_1 \in S_{X_1}} \sum_{x_2 \in S_{X_2}} ...\sum_{x_n \in S_{X_n}}  P_{X_1...X_n}(x_1...x_n)=1$$

$$P(\underline{X} \in B)=\sum_{(x_1...x_n)\in B}P_{X_1...X_n}(x_1...x_n)$$

$$B$$ is a subset of $$\R^n$$

#### Example

3 fair 6-sided dice

$$X_i=$$ Number obtained when I throw the $$i^{th}$$ dice

$$P_{X_1X_2X_3}(x_1,x_2,x_3)=\frac{1}{216}$$

$$P_{X_2X_3}(x_2,x_3)=P(X_2=x_2,X_3=x_3)$$

$$=P(X_1 \in S_X, X_2=x_2, X_3=x_3)$$

$$=\sum_{x_1 \in S_{X_1}}P_{X1X2X3}(x_1,x_2,x_3)$$

------

### Properties of Joint PMF

1. $$P_X(x)=\sum_{y \in S_Y} P_{XY}(x,y)$$

   $$P_{X_2...X_n}(x_2...x_n)=\sum_{x_1 \in S_{X_1}}P_{X_1X_2...X_n}(x_1,...,x_n)$$

2. $$P_{X_n}(x_n)=\sum_{x_1 \in S_{X_1}} ... \sum_{x_n \in S_{X_n}} P_{X_1...X_n}(x_1,...,x_n)$$

3. $$P_{X|Y}(x|y)=P(X=x|Y=y)$$

   $$P_{X_n|X_{n-1}...X_n}(x_n|x_{n-1}...x_1)=P(X_n=x_n|X_{n-1}...X_1=x_1)$$

   $$=\frac{P(X_n=x_n...X_1=x_1)}{P(X_{n-1}=x_{n-1}...X_1=x_1)}$$

   $$=\frac{P_{X_1...X_n}(x_1...x_n)}{P_{X_1...X_{n-1}(x_1...x_{n-1})}}$$

4. $$P(X_2=x_2,X_1=x_1)=P(X_2=x_2|X_1=x_1)P(X_1=x_1)$$
   $$P(X_3=x_3,X_2=x_2,X_1=x_1)=P(X_3=x_3|X_2=x_2,X_1=x_1)P(X_2=x_2|X_1=x_1)$$

   $$=P_{X_3|X_2X_1}(x_3|x_2x_1)P_{X_2|X_1}(x_2|x_1)P_X(x_1)$$

------

#### Example

$$P_{X_1X_2X_3}(x_1,x_2,x_3)$$

$$x_i \in \{1,2,...n\}$$

$$P(X_1>X_3)=\sum_{x_1,x_3=1, x_1>x_3}P_{X_1X_3}(x_1,x_3)$$

$$P_{X_1X_2X_3}(x_1,x_2,x_3)=\frac{1}{216}$$ for all $$x_i \in \{1,2,...6\}$$

$$P_{X_2|X_1X_3}(6|1,1)=P(X_2=6|X_1=1,X_3=1)$$

$$=\frac{P(X_2=6,X_1=1,X_3=1)}{P(X_1=1,X_3=1}$$

$$=\frac{\frac{1}{216}}{\sum_{x_2=1}^6P_{X_1X_2X_3}(1,x_2,1)}=\frac{\frac{1}{216}}{\frac{1}{36}}=\frac{1}{6}$$

------

### Jointly continuous Random vector

$$\underline{X}$$ is jointly continuous if 

$$P(\underline{X}\in B)=\int\int_{B} f_{X_1...X_n}(x_1...x_n)dx_1...dx_n$$

where $$B \subset \R^n$$, $$f_{X_1...X_n}(x_1...x_n)$$ is the joint density of $$X_1,...X_n$$

$$F_{X_1...X_n}(x_1...x_n)=P(X_1 \leq x_1 ... X_n \leq x_n)$$

$$=\int_{-\infty}^{x_n} ... \int_{-\infty}^{x_1}  f_{X_1...X_n}(s_1...s_n)ds_1...ds_n$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}$$

$$f_{X_n|X_{n-1}...X_1}(x_n|x_{n-1}...x_1)=\frac{f_{X_1...X_n}(x_1...x_n)}{f_{X_1...X_{n-1}(x_1...x_{n-1})}}$$

#### Example

$$X_1 \sim \text{Uniform} (0,1)$$
Given $$X_1=X_2$$ 

$$X_2 \sim \text{Uniform} (0,X_1)$$

$$0<x_1<1$$

Given $$X_2=x_2,X_1=x_1$$

$$X_3 \sim \text{Uniform} (0,X_2)$$

$$0<x_2<1$$

$$f_{X_1}(x_1)=\begin{cases}1 & 0< x_1<1 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{X_2|X_1}(x_2|x_1)=\begin{cases} \frac{1}{x_1} & 0< x_2 < x_1\\ 0 & \text{otherwise}\end{cases}$$

$$f_{X_3|X_2X_1}(x_3|x_2x_1)=\begin{cases} \frac{1}{x_2} & 0< x_3 < x_2\\ 0 & \text{otherwise}\end{cases}$$

$$f_{X_1X_2X_3}(x_1,x_2,x_3)=f_{X_3|X_2X_1}(x_3|x_2x_1)f_{X_2|X_1}(x_2|x_1)f_{X_1}(x_1)$$

$$=\begin{cases} \frac{1}{x_2} \frac{1}{x_1} 1 & 0<x_1<1, 0<x_2<x_1, 0<x_3<x_3 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{X_2X_3}(x_2,x_3)=\int_{-\infty}^{\infty}f_{X_1X_2X_3}(x_1,x_2,x_3)dx_1$$

where $$0<x_3<x_2<x_1<1$$
$$=\int_{x_2}^{1}\frac{1}{x_2} \frac{1}{x_1} dx_1$$

## Discussion 12

### Outlines

Problems

1. Joint PMF, PDF
2. Uncorreloteness of RVs

------

### Question 1

$$X,Y$$ are independent Poisson RV's with parameters $$\lambda_1, \lambda_2$$

Define $$Z:=X+Y$$

(a) Joint PMF of $$X$$ and $$Z$$

$$X \sim \text{Poisson} (\lambda_1), Y \sim \text{Poisson} (\lambda_2)$$

$$P(X=k)=\frac{e^{-\lambda_1} \lambda_1^k}{k!}, P(Y=k)=\frac{e^{-\lambda_2} \lambda_2^k}{k!}$$

$$Z:=X+Y$$

For (a), we want to get $$P_{XZ}(x,z)$$

$$P(X=x, Z=z)=P(X=x, X+Y=z)$$

$$=P(X=x, Y=z-X)$$

$$=P(X=x)P(Y=z-X)$$     - Independence

For $$X>z$$

$$P(X=x, Z=z)=0$$
For $$X \leq z$$

$$P(X=x,Z=z)=\frac{e^{-\lambda_1} \lambda_1^x}{x!} \frac{e^{-\lambda_2} \lambda_2^{(z-x)}}{(z-x)!}$$

$$P(X=x,Z=z)=\begin{cases} 0 & x>z \\ \frac{e^{-\lambda_1} \lambda_1^x}{x!} \frac{e^{-\lambda_2} \lambda_2^{(z-x)}}{(z-x)!} & z \geq x\end{cases}$$

(b) Marginal PMF of $$Z$$

For (b), we want to $$P_{Z}(z)$$

we know that joint PMF of $$X, Z$$ and PMF of $$X$$

$$P_{Z}(z)=\sum_{x \in S_X} P(Z|X)P(X=x)$$       - Total Probability

$$=\sum_{x \in S_X} P(X=x,Z=z)$$

$$=\sum_{0}^{z} P(X=x,Z=z)$$

$$P_{Z}(z)=\sum_{x=0}^{z} \frac{e^{-\lambda_1} \lambda_1^x}{x!} \frac{e^{-\lambda_2} \lambda_2^{(z-x)}}{(z-x)!}$$

(c) Show that $$Z \sim \text{Poisson} (\lambda_1+\lambda_2)$$

$$Z:=X+Y$$

$$X \sim \text{Poisson} (\lambda_1), Y \sim \text{Poisson} (\lambda_2)$$

$$P(Z=k)=P(X+Y = k)$$

$$=\sum_{i=0}^{k}P(X+Y=k |X) P(X=i)$$

$$=\sum_{i=0}^{k} P(Y=k-i, X=i)$$

since $$X,Y$$ are independent

$$=\sum_{i=0}^{k}P(Y=k-i)P(X=i)$$

$$=\sum_{i=0}^{k} \frac{e^{-\lambda_2} \lambda_2^{(k-i)}}{(k-i)!} \frac{e^{-\lambda_1} \lambda_1^i}{i!}$$

$$=e^{- (\lambda_1+\lambda_2)} \sum_{i=0}^{k} \frac{\lambda^{k-i} \lambda_1^i}{(k-i)! i!}$$

$$=\frac{e^{- (\lambda_1+\lambda_2)}}{k!} \sum_{i=0}^{k} \frac{k!}{(k-i)! i!} \lambda^{k-i} \lambda_1^i$$ 

where $$\frac{k!}{(k-i)! i!}=\binom{k}{i}$$

$$=\frac{e^{- (\lambda_1+\lambda_2)}}{k!} \sum_{i=0}^{k} \binom{k}{i} \lambda^{k-i} \lambda_1^i$$

where $$\sum_{i=0}^{k} \binom{k}{i} \lambda^{k-i} \lambda_1^i = (\lambda_1+\lambda_2)^k$$

$$=\frac{e^{- (\lambda_1+\lambda_2)}}{k!} (\lambda_1+\lambda_2)^k $$

$$P(Z=k)=\frac{e^{- (\lambda_1+\lambda_2)}(\lambda_1+\lambda_2)^k}{k!}$$

$$\implies Z \sim \text{Poisson} (\lambda_1+\lambda_2)$$  

### Question 2

Let $$X$$ and $$Y$$ be the jointly Gaussian random variables with $$X \sim \mathcal{N}(m_1, \sigma_1),Y \sim \mathcal{N}(m_2, \sigma_2)$$

(a) Show that $$X$$ and $$Y$$ are independent if and only if $$\rho=0$$

Independence $$\implies$$ Uncorrelatedness 

Uncorrelatedness $$\implies$$ Independence (True only for Gaussian RVs)

$$f_{XY}(x,y)=\frac{exp(\frac{-1}{2 (1-\rho_{XY}^2)}((\frac{x-m_1}{\sigma_1})^2+(\frac{y-m_2}{\sigma_2})^2-2\rho_{XY}(\frac{x-m_1}{\sigma_1})(\frac{y-m_2}{\sigma_2})))}{2 \pi \sigma_1 \sigma_2 \sqrt{1-\rho_{XY}^2}}$$

If uncorrelated, i.e., $$\rho_{XY}=0$$

$$f_{XY}(x,y)=\frac{exp(\frac{-1}{2}((\frac{x-m_1}{\sigma_1})^2+(\frac{y-m_2}{\sigma_2})^2)))}{2 \pi \sigma_1 \sigma_2 }$$

$$e^{-(a+b)}=e^{-a}e^{-b}$$

$$=\frac{1}{\sqrt{2 \pi \sigma_1}}  exp(\frac{-1}{2} (\frac{x-m_1}{\sigma_1})^2)   \frac{1}{\sqrt{2 \pi \sigma_2}}exp(\frac{-1}{2} (\frac{y-m_2}{\sigma_2})^2)$$

where $$f_{X}(x)=\frac{1}{\sqrt{2 \pi \sigma_1}}  exp(\frac{-1}{2} (\frac{x-m_1}{\sigma_1})^2), f_{Y}(y)=\frac{1}{\sqrt{2 \pi \sigma_2}}exp(\frac{-1}{2} (\frac{y-m_2}{\sigma_2})^2)$$

$$f_{XY}(x,y)=f_{X}(x)f_{Y}(y)$$

(b) Suppose $$\rho=0$$, find $$P(XY>0)$$

$$-\infty \leq x \leq \infty, -\infty \leq y \leq \infty$$

![image-20241125220732812](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241125220732812.png)

$$P(XY>0)=P(X,Y \text{have the same sign})$$

$$P(XY>0)=\int_{x^{+}} \int_{y^{+}} f_{XY}(x,y)dxdy + \int_{x^{-}} \int_{y^{-}} f_{XY}(x,y)dxdy$$

Since $$\rho_{XY}=0$$

$$X,Y$$ are independent

$$X,Y$$ are Gaussian RVs

$$=\int_{x=0}^{\infty} f_{X}(x)dx \int_{y=0}^{\infty} f_{Y}(y)dy + \int_{-\infty}^{0} f_{X}(x)dx \int_{-\infty}^{0} f_Y(y)dy$$

Observe

$$\int_{0}^{\infty} \frac{1}{\sqrt{2 \pi}} exp(-\frac{(x-m_1)^2}{2 \sigma_1^2}) dx = \int_{x=-\frac{m_1}{\sigma_1}}^{\infty} exp(-\frac{t^2}{2}) dt =Q(-\frac{m_1}{\sigma_1})$$

Then

$$P(XY>0)=Q(-\frac{m_1}{\sigma_1}) Q(-\frac{m_2}{\sigma_2}) +(1-Q(-\frac{m_1}{\sigma_1}))(1-Q(-\frac{m_2}{\sigma_2}))$$

### Question 3

 Show that $$Var[X+Y]=Var[X]+Var[Y]$$ if $$X$$ and $$Y$$ are independent

$$Var[X+Y]=E[(X+Y)^2]-(E[X+Y])^2$$

Consider

$$(E[X+Y])^2=E[X+Y]E[X+Y]$$

$$=E[X]E[X+Y]+E[Y]E[X+Y]$$         - Linearity property

$$=E[E[X](X+Y)]+E[E[Y](X+Y)]$$        - $$E[a(X+Y)]=aE[X+Y]$$

Here $$E[X]$$ is a constant

$$=E[XE[X]+YE[X]]+E[XE[Y]+YE[Y]]$$

where $$E[XE[X]]=E[X]E[X]$$

$$=(E[X])^2+2E[X]E[Y]+(E[Y])^2$$

$$Var[X+Y]=E[X^2]+E[Y^2]+2E[XY]-(E[X])^2-(E[Y])^2-2E[X]E[Y]$$

$$=Var[X]+Var[Y]$$

Due to independence, $$E[XY]=E[X]E[Y]=0$$

### Question 4

A dart is equally likely to land at any point $$(X,Y)$$ inside a circular target of unit radius. Let $$R,\theta$$ be radius and angle of the point $$(X,Y)$$ from origin.

If $$(X,Y)$$ are jointly Gaussian RVs. Find $$P(X^2+Y^2 < R^2)$$ when $$\rho=0$$

![image-20241127191817501](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127191817501.png)

$$P(X^2+Y^2 < R^2)=\int\int_{x^2+y^2 < r^2} f_{XY}(x,y)$$

$$=\int\int_{x^2+y^2 < r^2} \frac{1}{ 2 \pi \sigma^2} exp(-\frac{(x^2+y^2)}{2 \sigma^2}) dxdy$$

$$r^2 \cos^2(\theta) +r^2 \sin^2(\theta)=r^2$$

$$x=r\cos(\theta), y=r \sin(\theta)$$

$$=\int_{\theta=0}^{2 \pi} \int_{r=0}^{R} \frac{1}{2 \pi \sigma^2} exp(-\frac{r^2}{2 \sigma^2}) dr \cdot rd \theta$$

$$=\frac{1}{2 \pi \sigma^2} 2 \pi \int_{r=0}^{R} r exp(-\frac{r^2}{2 \sigma^2}) dr d \theta$$

$$=1-exp(-\frac{R}{2\sigma^2})$$

$$P(X^2+Y^2<R^2)=1-exp(-\frac{R}{2\sigma^2})$$

### Question 5

At even time instants, a robot moves either $$+\Delta$$ cm or $$-\Delta$$ cm in the x-direction according to the outcome of a coin flip; at odd time instants, a robot moves similarly according to another coin flip in the y-direction. Assuming that the robot begins at the origin, let $$X$$ and $$Y$$ be the coordinates of the location of the robot after $$2n$$ time instants. Determine whether $$X$$ and $$Y$$ are independent RVs

$$S_{X,Y}=\{(k_1,k_2):0 \leq k_1\leq n, 0 \leq k_2 \leq n\}$$

where

$$(N_1=k_1):\#$$ of heads in even time instants

$$(N_2=k_2):\#$$ of heads in odd time instants

$$X= \Delta N_1-\Delta(n-N_1)=2 \Delta N_1-n \Delta$$

$$Y= \Delta N_2-\Delta(n-N_2)=2 \Delta N_2-n \Delta$$

![image-20241127193319782](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127193319782.png)

$$P_{X,Y}(x,y)=P(X=(2k-n)\Delta, Y=(2j-n)\Delta)$$

Since $$X,Y$$ depend on coin flip and assuming same coin (pair) is used for both directions

$$=P(X=(2k-n)\Delta)P(Y=(2j-n)\Delta)$$

$$=\binom{n}{2k-n} p^k (1-p)^{n-k} \binom{n}{2j-n}p^j (1-p)^{n-j}$$

$$X,Y$$ are independent

## Week 13 Session 1

### Random Vector

$$X_1,X_2, X_3...X_n$$

$$\underline{X}=\begin{bmatrix} X_1 \\ X_2 \\ ... \\X_n \end{bmatrix} \rightarrow $$ Random Vector

### Joint CDF

$$F_{\underline{X}}(x_1,...x_n)=P(X_1 \leq x_1, ... X_n \leq x_n)$$

$$\lim_{x_n \rightarrow \infty}F_{X_1... X_n}(x_1, ..., x_n)=F_{X_1,...,X_{n-1}}(x_1...x_{n-1})$$

### Joint PMF

$$X_1,...X_n$$ discrete RVs

$$P_{X_1...X_n}(x_1...x_n)=P(X_1=x_1...X_n=x_n)$$

$$\sum_{x_1 \in S_{X_1}} \sum_{x_2 \in S_{X_2}} ... \sum_{x_n \in S_{X_n}} P_{X_1 ... X_n}(x_1 ... x_n)=1$$

$$P(\underline{X} \in B)=\sum_{(x_1 ... x_n) \in B}P_{X_1 ... X_n}(x_1 ... x_n)$$

$$B$$ is a subset of $$\R^n$$

$$P_{X_2...X_n}(x_2 ... x_n)=\sum_{x_1 \in S_{X_1}}P_{X_1 ... X_n}(x_1 ... x_n)$$

### Jointly Continuous Random Vector

$$P(\underline{X} \in B)=\int ... \int_{B} f_{X_1 ... X_n}(x_1 ... x_n) dx_1...dx_n$$

where $$B \subset \R^n$$ , $$f_{X_1 ... X_n}(x_1 ... x_n)$$ is the joint density of $$X_1...X_n$$

$$\int_{-\infty}^{\infty} ... \int_{-\infty}^{\infty} f_{X_1X_2...X_n}dx_1 dx_2 ...dx_n=1$$

$$\int_{-\infty}^{\infty} f_{X_1 ... X_n}(x_1 ... x_n)dx_1=f_{X_2...X_n}(x_2 ... x_n)$$

------

### Conditional density

$$f_{X_n|X_1... X_{n-1}}(x_n|x_1 ... x_{n-1})=\frac{f_{X_1 ... X_n(x_1 ... x_n)}}{f_{X_1 ... X_{n-1}(x_1 ... x_{n-1})}}$$

$$f_{X|Y}(x|y)=\frac{f_{XY}(x,y)}{f_Y(y)}$$

$$f_{X_1X_2|X_3X_4}(x_1,x_2|x_3,x_4)=\frac{f_{X_1X_2X_3X_4(x_1 ... x_4)}}{f_{X_3X_4}(x_3,x_4)}$$

Chain Rule

$$f_{X_1...X_n}(x_1 ... x_n)=f_{X_n|X_1 ... X_{n-1}}(x_n|x_1 ... x_{n-1})f_{X_1 ... X_{n-1}}(x_1 ... x_{n-1})$$

------

Gaussian density $$m,\sigma^2$$

$$\frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{(x-m)^2}{2 \sigma^2}}$$

#### Example

$$f_{X_1X_2X_3}(x_1, x_2,x_3) =\frac{e^{(-x_1^2+x_2^2-\sqrt{2}x_1x_2+\frac{x_3^2}{2})}}{2 \pi \sqrt{\pi}}$$

$$x_1,x_2,x_3 \in \R$$

Joint PDF of $$X_1$$ and $$X_3$$

$$f_{X_1X_3}(x_1,x_3)=\int_{-\infty}^{\infty} f_{X_1X_2X_3}(x_1x_2x_3)dx_2$$

$$=\frac{e^{-x_1^2 }e^{-\frac{x_3^2}{2}}} {2 \pi \sqrt{\pi}} \int_{-\infty}^{\infty} e^{-(x_2^2-\sqrt{2}x_1x_2)}dx_2$$

$$x_2^2 -\frac{2\sqrt{2}}{2}x_1x_2+\frac{x_1^2}{2}-\frac{x_1^2}{2}$$

$$=\frac{e^{-x_1^2 }e^{-\frac{x_3^2}{2}}} {2 \pi \sqrt{\pi}} \int_{-\infty}^{\infty} e^{-(x_2-\frac{x_1}{\sqrt{2}})^2} e^{\frac{x_1^2}{2}}dx_2$$

$$=\frac{e^{-x_1^2 }e^{-\frac{x_3^2}{2}}} {2 \pi \sqrt{\pi}} \sqrt{2 \pi \frac{1}{2}}\int_{-\infty}^{\infty}  \frac{1}{\sqrt{2 \pi \frac{1}{2}}}e^{-\frac{(x_2-\frac{x_1}{\sqrt{2}})^2}{2 \cdot \frac{1}{2}}}dx_2$$

$$\int_{-\infty}^{\infty}  \frac{1}{\sqrt{2 \pi \frac{1}{2}}}e^{-\frac{(x_2-\frac{x_1}{\sqrt{2}})^2}{2 \cdot \frac{1}{2}}}dx_2=1$$

$$\int_{-\infty}^{\infty} \frac{e^{-\frac{(x_2-m)^2}{2\sigma^2}}}{\sqrt{2 \pi \sigma^2}}dx_2$$

$$=\frac{e^{-\frac{x_1^2}{2} }e^{-\frac{x_3^2}{2}}} {\sqrt{2\pi} \sqrt{2\pi}} $$

$$f_{X_1X_3}(x_1x_3)=\frac{e^{-\frac{x_1^2}{2}} }{\sqrt{2\pi}} \frac{e^{-\frac{x_3^2}{2}}}{\sqrt{2\pi}}$$

$$f_{X_1}(x_1)=\frac{e^{-\frac{x_1^2}{2}} }{\sqrt{2\pi}}, f_{X_3}(x_3)=\frac{e^{-\frac{x_3^2}{2}} }{\sqrt{2\pi}}$$

Independent $$X_1$$ and $$X_3$$

$$f_{X_1}(x_1)=\frac{e^{-\frac{x_1^2}{2}} }{\sqrt{2\pi}}\int_{-\infty}^{\infty} \frac{e^{-\frac{x_3^2}{2}} }{\sqrt{2\pi}} dx_3$$

$$=\frac{e^{-\frac{x_1^2}{2}} }{\sqrt{2\pi}}$$

$$X_1 \sim \mathcal{N}(0,1)$$

$$X_3 \sim \mathcal{N}(0,1)$$

------

#### Example

$$X,Y,Z$$

$$f_{XYZ}(x,y,z)=\begin{cases} \frac{3 z^2}{7 \sqrt{2 \pi}} e^{-2y} e^{-\frac{(x-y)^2}{2z^2}} & y \geq 0, 1 \leq z \leq 2, x \in \R \\ 0 & \text{otherwise}\end{cases}$$

For $$y \geq 0, 1 \leq z \leq 2$$

$$f_{YZ}(y,z)=\int_{-\infty}^{\infty} f_{XYZ}(xyz)dx$$

$$=\frac{3 z^2}{7 \sqrt{2 \pi}}  e^{-2y} \sqrt{2 \pi z^2} \int_{-\infty}^{\infty} \frac{1}{\sqrt{2 \pi z^2}}e^{-\frac{(x-y)^2}{2z^2}}dx$$

$$\int_{-\infty}^{\infty} \frac{1}{\sqrt{2 \pi z^2}}e^{-\frac{(x-y)^2}{2z^2}}dx$$ is $$\mathcal{N}(y,z^2)$$

$$f_{YZ}(y,z)=\begin{cases} \frac{3}{7} z^3 e^{-2y} & y \geq 0, 1 \leq z \leq 2 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{Z}(z)=\begin{cases} \int_{0}^{\infty} \frac{3}{7} z^3 e^{-2y}dy & 1\leq z \leq 2 \\ 0 & \text{otherwise}\end{cases}$$

$$\frac{3}{7} z^2 \int_{0}^{\infty} z e^{-2y}dy$$

$$f_Z(z)=\begin{cases} \frac{3}{7} z^2 & 1 \leq z \leq 2\\ 0 & \text{otherwise}\end{cases}$$

------

$$y \geq0, 1 \leq z \leq 2$$

$$f_{X|Y,Z}(x|y,z)=\frac{f_{XYZ}(x,y,z)}{f_{YZ}(y,z)}$$

$$=\frac{1}{\sqrt{2 \pi z^2}} e^{-\frac{(x-y)^2}{2z^2}}$$

$$\mathcal{N}(y,z^2)$$

Conditioned on $$Y=y,Z=z ,(y \geq 0, 1 \leq z \leq 2), X \sim \mathcal(y,z^2)$$

$$E[X|Y=y,Z=z]=y$$

$$E[X^2|Y=y,Z=z]=z^2+y^2$$

$$X \sim \mathcal{N}(m,\sigma^2)$$

$$E[X^2]=m^2+\sigma^2$$

$$P(X \leq 0|Y=y, Z=z)=\phi(-\frac{y}{z})$$

$$X \sim \mathcal{N} (m,\sigma^2)$$

$$P(X \leq 0)=P(\frac{X-m}{\sigma} \leq \frac{-m}{\sigma})=\phi(\frac{-m}{\sigma})$$

------

Independence of $$X_1,...X_n$$

Definition: $$X_1, ... X_n$$ are independent if

$$P(X_1 \in B_1, X_2 \in B_2... X_n \in B_n)=P(X_1 \in B_1) P(X_2 \in B_2) ... P(X_n \in B_n)$$ for all $$B_1, B_2, ... , B_n$$ which are subsets of $$\R$$

Thm: 

1. $$X_1, ... , X_n$$ are independent if and only if $$F_{X_1 ... X_n}(x_1 ... x_n)=F_{X_1}(x_1) ... F_{X_n}(x_n)$$ for all $$x_i \in \R, i= 1, ... , n$$

2. If $$X_1 ... X_n$$ are discrete RVs, then $$X_1, ... , X_n$$ are independent if and only if 

   $$P_{X_1 ... X_n}(x_1 ... x_n)=P_{X_1}(x_1) ... P_{X_n}(x_n)$$ for all $$x_i \in \R, i=1, ... ,n$$

3. If $$X_1 ... X_n$$ are jointly continuous RVs, then $$X_1 ... X_n$$ are independent if and only if

   $$f_{X_1 ... X_n}(x_1 ... x_n)=f_{X_1}(x_1) ... f_{X_n}(x_n)$$ for all $$x_i \in \R, i=1,...,n$$

#### Example

$$f_{X_1 ... X_n} (x_1, ... , x_n)=\frac{e^{- \frac{(x_1^2 + x_2^2 + ... + x_n^2)}{2}}}{(2\pi)^{\frac{n}{2}}}$$ for all $$x_i \in \R, i=1,... ,n$$

$$f_{X_1}(x_1)=\int ... \int f_{X_1, ..., X_n}(x_1 , ... , x_n)dx_2 dx_3 ... dx_n$$

$$=\int...\int \frac{e^{- \frac{(x_1^2 + x_3^2 + ... + x_n^2)}{2}}}{(2\pi)^{\frac{n-1}{2}}} \int_{-\infty}^{\infty}\frac{e^{- \frac{x_2^2}{2}}}{\sqrt{2 \pi}} dx_2 dx_3 ... dx_n$$

$$f_{X_1}(x_1)=\frac{e^{- \frac{x_1^2}{2}}}{\sqrt{2 \pi}}$$

$$f_{X_i}(x_i)=\frac{e^{- \frac{x_i^2}{2}}}{\sqrt{2 \pi}}, i=1,...,n$$

$$f_{X_1...X_n}(x_1 ... x_n)=f_{X_1}(x_1)...f_{X_n}(x_n)$$

$$\implies$$ Independent

$$X_i \sim \mathcal{N}(0,1)$$

IID RVs (Independent and identically distributed)

$$P(X_1 > 2|X_3 > 10)=\frac{P(X_1 > 2, X_3>10)}{P(X_3 > 10)}$$

Independence

$$=\frac{P(X_1>2)P(X_3>10)}{P(X_3>10)}=P(X_1 >2)=1-\phi(2)$$

For event, pairwise does not imply mutual independence

$$X_1, X_2$$ - Independence

$$X_2, X_3$$ - Independence

$$P(X_1 \in B_1, X_2 \in B_2)=P(X_1 \in B_1)P(X_2 \in B_2)$$

$$P(X_2 \in B_2, X_3 \in B_3)=P(X_2 \in B_2)P(X_3 \in B_3)$$

Does not imply

$$X_1 \in B_1, X_2 \in B_2, X_3 \in B_3$$ are mutually independent

Pairwise independent of RVs does not imply mutual independence

------

#### Example

$$X_1, ... X_n, f_{X_1... X_n}$$ 

$$Z_i=a_i X_i + b_i, i=1,...,n$$

Joint CDF of $$Z_1, ... Z_n$$

$$F_{Z_1, ... Z_n}(z_1 ... z_n)=P(Z_1 \leq z_1, ... Z_n \leq z_n)$$

$$=P(a_1X_1+b_1 \leq z_1, ... a_nX_n+b_n \leq z_n)$$

$$=P(X_1 \leq \frac{z_1-b_1}{a_1} ... X_n \leq \frac{z_n-b_n}{a_n})$$

$$=F_{X_1 ... X_n}(\frac{z_1-b_1}{a_1} ...  \frac{z_n-b_n}{a_n})$$

$$f_{Z_1 ... Z_n}(z_1 ... z_n)=\frac{\partial}{\partial z_1} \frac{\partial}{\partial z_2} ... \frac{\partial}{\partial z_n} F_{X_1 ... X_n}(x_1... x_n)$$

$$f_{XY}(x,y)=\frac{\partial^2}{\partial x \partial y}F_{XY}(x,y)$$

$$=\frac{\partial}{\partial z_1} \frac{\partial}{\partial z_2} ... (\frac{\partial F_{X_1...X_n}}{\partial x_n}|_{x_n = \frac{z_n-b_n}{a_n}} \frac{1}{a_n})$$

$$=\frac{1}{a_1 ... a_n} f_{X_1... X_n} (\frac{z_1-b_1}{a_1}, ... \frac{z_n-b_n}{a_n})$$

$$\frac{d}{dx} F(g(x))=\frac{dF}{dy}|_{y=g(x)}\frac{dg(x)}{dx}$$

$$\frac{\partial}{\partial z_1} \frac{\partial}{\partial z_2} ... \frac{\partial}{\partial z_n}  F_{X_1...X_n}()=f_{X_1 ... X_n}()$$

$$F_Z(z)=F_X(\frac{z-b}{a})$$

$$\frac{dF_Z(z)}{dz}=\frac{dF_X}{dz}(\frac{z-b}{a})$$

$$=\frac{dF_X}{dz}|_{x=\frac{z-b}{a}} \frac{d}{dz}(\frac{z-b}{a})$$

$$=\frac{dF_X}{dx}|_{x=\frac{z-b}{a}} \frac{1}{a}$$

$$=f_{X}(\frac{z-b}{a})\frac{1}{a}$$

$$F_{Z_1 ... Z_n}(z_1 ... z_n)=F_{X_1 ... X_n}(\frac{z_1 - b_1}{a_1} ... \frac{z_n-b_n}{a_n})$$

$$\frac{d}{dz_n}F_{Z_1 ... Z_n}(z_1 ... z_n)=\frac{d}{dz_n}F_{X_1 ... X_n}(\frac{z_1 - b_1}{a_1} ... \frac{z_n-b_n}{a_n})$$

$$=\frac{d}{dz_n}F_{X_1 ... X_n}(\frac{z_1 - b_1}{a_1} ... x_n)|_{x_n=\frac{z_n-b_n}{a_n}} \frac{d}{dz_n}(\frac{z_n-b_n}{a_n})$$

$$=\frac{d}{dx_n}F_{X_1 ... X_n}(\frac{z_1 - b_1}{a_1} ... x_n)|_{x_n=\frac{z_n-b_n}{a_n}} \frac{1}{a_n}$$

after $$n$$ fold differentiation

$$=\frac{d}{dx_1} \frac{d}{dx_2} ... \frac{d}{dx_n} F_{X_1, ..., X_n}(x_1, ... x_n)|_{x_i =\frac{z_i-b_i}{a_i}} \frac{1}{a_1 ... a_n}$$

$$=f_{X_1, ..., X_n}(x_1, ... x_n)|_{x_i =\frac{z_i-b_i}{a_i}} \frac{1}{a_1 ... a_n}$$

$$=f_{X_1, ..., X_n}(\frac{z_1-b_1}{a_1}, ... \frac{z_n-b_n}{a_n}) \frac{1}{a_1 ... a_n}$$

------

#### Example

IID RVs $$X_1, ... X_n \rightarrow f_{X_i}$$

$$Z=\min{(X_1, ... X_n)}$$

$$F_Z(z)=P(Z \leq z)$$

$$=P(\min{(X_1, ... X_n)} \leq z)$$

$$=1- P(\min{(X_1, ... X_n)} > z)$$

$$=1-P(X_1> z, X_2> z... X_n > z)$$

$$=1- P(X_1 >z)P(X_2 > z) ... P(X_n >z)$$

$$=1-[(1-F_{X_1}(z)) (1-F_{X_2}(z)) ... (1-F_{X_n}(z))]$$

differentiate with respect to $$z$$

$$X_i \sim \text{exp}(1)$$

$$F_{X_i}(z)=1-e^{-z}$$

------

### PDF of Transformation of RV

$$X_1, X_2$$

$$Z_1 =g_1(X_1, X_2)$$

$$Z_2=g_2(X_1, X_2)$$

$$\underline{Z}=\underline{g}(\underline{X})$$

Assumptions

1. $$g_1, g_2$$ are differentiable
2. For each $$\binom{z_1}{z_2}$$, there is at most one vector $$\binom{x_1}{x_2}$$ such that $$\underline{g} \binom{x_1}{x_2} = \binom{z_1}{z_2}$$

Under these assumptions

$$f_{Z_1Z_2}(z_1,z_2)=\frac{f_{X_1X_2}(x_1,x_2)}{|J(x_1, x_2)|}|_{ \binom{x_1}{x_2} |_\underline{g}^{-1} \binom{z_1}{z_2}}$$

Absolute value of determinant of the denominator is the Jacobian of the transformation

$$J(x_1, x_2)=\begin{bmatrix} \frac{\partial g_1}{\partial x_1} &  \frac{\partial g_1}{\partial x_2} \\  \frac{\partial g_2}{\partial x_1} &  \frac{\partial g_2}{\partial x_2}\end{bmatrix}$$

------

#### Example

$$X_1, X_2, f_{X_1X_2}$$

$$Z_1=X_1+X_2$$
$$Z_2=\frac{X_1}{X_1+X_2}$$

$$z_1=x_1+x_2$$

$$z_2=\frac{x_1}{x_1+x_2}$$

$$\underline{g}^{-1} \binom{z_1}{z_2}=\binom{z_1z_2}{z_1-z_1z_2}$$

$$J(x_1, x_2)=\begin{bmatrix} \frac{\partial g_1}{\partial x_1} &  \frac{\partial g_1}{\partial x_2} \\  \frac{\partial g_2}{\partial x_1} &  \frac{\partial g_2}{\partial x_2}\end{bmatrix}$$

$$=\begin{bmatrix} 1 &  1\\  \frac{x_2}{(x_1+x_2)^2} &  \frac{-x_1}{(x_1+x_2)^2}\end{bmatrix}$$

$$|J(x_1,x_2)|=\frac{1}{|x_1+x_2|}$$

$$f_{Z_1Z_2}(z_1,z_2)=\frac{f_{X_1X_2}(x_1,x_2}{|J(x_1,x_2)|}|_ { \binom{x_1}{x_2} = \binom{z_1z_2}{z_1-z_1z_2}}$$

$$=\frac{f_{X_1X_2(z_1z_2, z_1-z_1z_2)}}{|\frac{1}{z_1}|}$$

#### Example

$$X_1,X_2,X_3, f_{X_1X_2X_3}$$

$$Z_1=X_1$$

$$Z_2=X_1+X_2$$

$$Z_3=X_1+X_2+X_3$$

$$z_1=x_1$$

$$z_2=x_1+x_2$$

$$z_3=x_1+x_2+x_3$$

$$\underline{g}^{-1} \pmatrix{z_1\\z_2\\z_3}=\pmatrix{z_1\\z_2-z_1\\z_3-z_2}$$

$$J(x_1 x_2 x_3)=\begin{bmatrix} \frac{\partial z_1}{\partial x_1} &  \frac{\partial z_1}{\partial x_2} & \frac{\partial z_1}{\partial x_3} \\  \frac{\partial z_2}{\partial x_1} &  \frac{\partial z_2}{\partial x_2} & \frac{\partial z_2}{\partial x_3} \\ \frac{\partial z_3}{\partial x_1} &  \frac{\partial z_3}{\partial x_2} & \frac{\partial z_3}{\partial x_3} \end{bmatrix}= \begin{bmatrix} 1 & 0 & 0 \\ 1 & 1 & 0 \\ 1 & 1 & 1\end{bmatrix}$$

$$|J(x_1 x_2x_3)|=1$$

$$f_{Z_1Z_2Z_3}(z_1 z_2 z_3)=\frac{f_{X_1X_2X_3}(x_1x_2x_3)}{1}|_{\pmatrix{x_1\\x_2\\x_3}=\underline{g}^{-1} \pmatrix{z_1\\z_2\\z_3}}$$

$$=f_{X_1X_2X_3}(z_1,z_2-z_1,z_3-z_2)$$

------

### Expectation

1. $$z=g(X,Y)$$

   $$E[Z]=\begin{cases} \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} g(x,y)f_{XY}(x,y)dxdx & \text{Continuous} \\ \sum_{x \in S_X} \sum_{y \in S_Y} g(x,y)P_{XY}(x,y) & \text{Discrete} \end{cases}$$

   $$Z=g(X_1,...,X_n)$$

   $$E[Z]=\begin{cases} \int_{-\infty}^{\infty} ... \int_{-\infty}^{\infty} g(x_1 ... x_n) f_{X_1... X_n}(x_1 ... x_n)dx_1 ... dx_n\\ \sum ... \sum g(x_1 ... x_n)P_{X_1 ... X_n}(x_1 ... x_n)\end{cases}$$

2. Recall that if $$X,Y$$ are independent

   $$E[XY]=E[X]E[Y]$$

   Similarly, if $$X_1, ... X_n$$ are independent, then

   $$E[X_1... X_n]=E[X_1] ... E[X_n]$$

3. $$X_1, X_2 , ... X_n$$ are independent

   $$Z_1=g_1(X_1)$$

   $$Z_2=g_2(X_2)$$

   $$...$$

   $$Z_n=g_n(X_n)$$

   Then, $$Z_1, ... Z_n$$ are also independent

## Week 13 Session 2

1. $$Var(aX)=a^2 Var(X)$$

2. $$Var(X+a)=Var(X)$$

3. Independent $$X,Y, Cov(X,Y)=0$$

   $$Cov(X,Y)=E[XY]-m_Xm_Y$$

   $$=m_Xm_Y-m_Xm_Y=0$$

4. Independent $$X,Y$$

   $$Var(X+Y)=Var(X)+Var(Y)$$

   $$E[X+Y]=m_Xm_Y$$

   $$Var(X+Y)=E[(X+Y-m_X-m_Y)^2]$$

   $$=E[(X-m_X)^2+ (Y-m_Y)^2+2(X-m_X)(Y-m_Y)]$$

   $$=Var(X)+Var(Y)+2Cov(X,Y)$$

   $$=Var(X)+Var(Y)$$

------

### Random Vectors

$$\underline{X}=\pmatrix{X_1\\X_2\\...\\X_n}$$

Mean Vector

$$E[\underline{X}]=\pmatrix{E[X_1]\\E[X_2]\\...\\E[X_n]}$$

$$E[\underline{X}]$$ is the same notation as $$m_{\underline{X}}$$

$$\underline{X} \cdot \underline{X}^T= \pmatrix{X_1\\X_2\\...\\X_n} \pmatrix{X_1 & X_2 & ...&X_n}$$

$$\underline{X} \cdot \underline{X}^T= \begin{bmatrix} X_1^2 & X_1X_2 & X_1X_3 & ... & X_1X_n \\ X_2X_1 & X_2^2 & ... & ... & ...\\ ... & ...& ... & ... & ...\\ X_nX_1 & ... & ... & ... & X_n^2  \end{bmatrix}$$

### Correlation Matrix

$$R_X=E[\underline{X} \cdot \underline{X}^T]=\begin{bmatrix} E[X_1^2] & E[X_1X_2] & E[X_1X_3] & ... & E[X_1X_n] \\ E[X_2X_1] & E[X_2^2] & ... & ... & ...\\ ... & ...& ... & ... & ...\\ E[X_nX_1] & ... & ... & ... & E[X_n^2]  \end{bmatrix}$$

is a symmetric matrix

$$(R_X)_{ij}=(R_X)_{ji}$$

$$A$$ is $$n \times n$$ square matrix

Covariance Matrix $$K_X$$

$$K_{\underline{X}} = E[(\underline{X}-m_{\underline{X}})(\underline{X}-m_{\underline{X}})^T]$$

$$=E\begin{bmatrix} (X_1-m_{X_1})^2 & (X_1-m_{X_1})(X_2-m_{X_2}) & ... & (X_1-m_{X_1})(X_n-m_{X_n})\\ ... & ... & ... & ...\\ (X_n-m_{X_n})(X_1-m_{X_1}) & ... & ... & (X_m-m_{X_m})^2  \end{bmatrix}$$

$$=\begin{bmatrix} Var(X_1) & Cov(X_1X_2) & ... & Cov(X_1X_n)\\ ... & ... & ... & ...\\ Cov(X_nX_1) & ... & ... & Var(X_n)  \end{bmatrix}$$

$$K_X$$ is a square $$n \times n$$, symmetric matrix

------

$$K_{\underline{X}} = E[(\underline{X}-m_{\underline{X}})(\underline{X}-m_{\underline{X}})^T]$$

$$=E[(\underline{X}-m_{{X}})(\underline{X}^T-m_{{X}})^T]$$

$$=E[\underline{X} \cdot \underline{X}^T-m_X\underline{X}^T-\underline{X}m_X^T+m_Xm_X^T]$$

$$=R_X-m_XE[X^T]-E[X]m_X^T+m_Xm_X^T$$

$$=R_X-m_Xm_X^T-m_Xm_X^T+m_Xm_X^T$$

$$=R_X-m_Xm_X^T$$

==$$K_X=R_X -m_Xm_X^T$$==

$$Var(X)=E[X^2]-(m_X)^2$$

$$Cov(X,Y)=E[XY]-m_Xm_Y$$

#### Example

$$X_1,X_2$$ are RV with mean 0, variance 1 and $$Cov(X_1,X_2)=\frac{-1}{\sqrt{2}}$$

$$\underline{X}=\binom{X_1}{X_2}$$

$$m_{\underline{X}}=\binom{0}{0}$$

$$K_{\underline{X}}=\begin{pmatrix} Var(X_1) & Cov(X_1,X_2) \\ Cov(X_2, X_1) & Var(X_2)\end{pmatrix}$$

$$=\begin{pmatrix} 1 & \frac{-1}{\sqrt{2}} \\ \frac{-1}{\sqrt{2}} & 1\end{pmatrix}$$

$$X_3$$ which mean 0, variance 1, independent of $$X_1$$ and $$X_2$$

$$\underline{Y}=\begin{pmatrix}X_1 \\ X_2 \\ X_3 \end{pmatrix}$$

$$m_{\underline{Y}}=\begin{pmatrix} 0 \\ 0 \\ 0 \end{pmatrix}$$

$$K_Y=\begin{pmatrix} 1 & \frac{-1}{\sqrt{2}} & 0 \\ \frac{-1}{\sqrt{2}} & 1 & 0 \\ 0 & 0& 1 \end{pmatrix}$$

------

$$\underline{X}=\begin{pmatrix} X_1 \\ ... \\X_n \end{pmatrix}$$

$$A=\begin{pmatrix} a_{11} & a_{12 } & ... & a_{1n} \\ a_{21} & ... & ... & a_{2n} \\ ... & ... & ... & ... \\ a_{m_1} & ... & ... & a_{mm}\end{pmatrix}$$

$$A$$ is fixed matrix (not random)

$$\underline{Y}=A\underline{X}$$

$$\underline{Y}=\begin{pmatrix} Y_1 \\ ... \\Y_n \end{pmatrix}=\begin{pmatrix} a_{11} & a_{12 } & ... & a_{1n} \\ a_{21} & ... & ... & a_{2n} \\ ... & ... & ... & ... \\ a_{m_1} & ... & ... & a_{mm}\end{pmatrix}\begin{pmatrix} X_1 \\ ... \\X_n \end{pmatrix}$$

$$Y_1=\sum_{j=1}^{n}a_{ij}X_{j}$$

$$Y_i=\sum_{j=1}^{n}a_{ij}X_j$$

$$E[Y_i]=E[\sum_{j=1}^{n}a_{ij}X_j]$$

$$=\sum_{j=1}^{n}a_{ij}E[X_j]$$

==$$m_{Y_i}=\sum_{j=1}^{n}a_{ij}m_{X_j}$$==

$$m_{\underline{Y}}= \begin{pmatrix} mY_1 \\ ... \\mY_n \end{pmatrix}=A\begin{pmatrix} mX_1 \\ ... \\mX_n \end{pmatrix}$$

$$m_{\underline{Y}}=Am_{\underline{X}}$$

Lemma: If $$\underline{Y}=A\underline{X}$$

then $$m_{\underline{Y}}=A m_{\underline{X}}$$

$$Y=aX$$

$$E[Y]=aE[X]$$

Linearity of Expectation

1. $$E[aX]=aE[X]$$

2. $$E[A\underline{X}]=A E[\underline{X}]$$

3. $$E[\underline{X}^T B]=E[\underline{X}^T]B$$

   $$B$$ is a constant matrix

4. $$E[A \underline{X} B]=AE[\underline{X}]B$$

------

$$\underline{Y}=A \underline{X}$$

$$m_{\underline{Y}}=A m_{\underline{X}}$$

$$K_{\underline{Y}}=E[(\underline{Y}-m_{\underline{Y}})(\underline{Y}-m_{\underline{Y}})^T]$$

$$=E[(AX-Am_X)(AX-Am_X)^T]$$

$$=E[A(X-m_X)(X-m_X)^TA^T]$$

$$=AE[(X-m_X)(X-m_X)^T]A^T$$

$$=AK_XA^T$$

Lemma: If $$\underline{Y}=A \underline{X}$$, then $$m_{\underline{Y}}=A m_{\underline{X}}$$

$$K_Y=AK_XA^T$$

Scalar Case:

$$Y=aX$$

$$m_Y=am_X$$

$$Var(Y)=a^2Var(X)$$

------

Cross-covariance between $$\underline{X}$$ and $$\underline{Y}$$

$$\underline{X} \in n$$ and $$\underline{Y} \in m$$

$$K_{\underline{X} \underline{Y}}=E[(\underline{X}-m_{\underline{x}})(\underline{Y}-m_{\underline{Y}})^T]$$

$$K_{\underline{X} \underline{Y}}$$ is $$n \times m$$ matrix

$$K_{\underline{Y} \underline{X}}=E[(\underline{Y}-m_{\underline{y}})(\underline{X}-m_{\underline{x}})^T]$$

$$K_{\underline{Y} \underline{X}}$$ is $$m \times n$$ matrix

$$(K_{\underline{X} \underline{Y}})^T=(E[(\underline{X}-m_{\underline{x}})(\underline{Y}-m_{\underline{Y}})^T])^T$$

$$=E[\{(\underline{X}-m_{\underline{x}})(\underline{Y}-m_{\underline{Y}})^T\}^T]$$

$$=E[(Y-m_Y)(X-m_X)^T]$$

$$=K_{\underline{Y} \underline{X}}$$

#### Example

$$\underline{Y}=A \underline{X}$$

$$K_{XY}=E[(X-m_X)(Y-m_Y)^T]$$

$$=E[(X-m_X)(AX-Am_X)^T]$$

$$=E[(X-m_X)(A(X-m_X))^T]$$

$$=E[(X-m_X)(X-m_X)^TA^T]$$

$$=K_XA^T$$

$$K_{\underline{Y} \underline{X}}= (K_X A^T)^T=A K_X^T=Ak_X$$

#### Example

$$\underline{X}=\begin{pmatrix}X_1 \\ X_2 \\X_3\end{pmatrix}$$

$$K_X=\begin{pmatrix} 1 & \frac{-1}{\sqrt{2}} & 0 \\ \frac{-1}{\sqrt{2}} & 1 & 0 \\ 0 & 0 & 1\end{pmatrix}$$

$$\underline{Y}= \begin{pmatrix} \frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} & 0 \\ \frac{-1}{\sqrt{2}} & \frac{1}{\sqrt{2}} & 0 \end{pmatrix}\underline{X}$$

$$Var(Y_1)$$

$$Cov(Y_1,Y_2)$$

------

Jointly Gaussian Random Vector

For a single Gaussian random variable

$$f_X(x)=\frac{1}{\sqrt{2 \pi \sigma^2}} exp(-\frac{(x-m)^2}{2 \sigma^2})$$

Definition: $$\underline{X}=\begin{pmatrix} X_1 \\ ... \\ X_n \end{pmatrix}$$ is a jointly Gaussian random vector if

$$f_{X_1 ... X_n}(x_1 ... x_n) =\frac{exp(-\frac{1}{2} (\underline{x} - \underline{m})^T K^{-1} (\underline{x}-\underline{m}))}{(2 \pi)^{\frac{n}{2}} |K|^{\frac{1}{2}}}$$

$$\underline{x}=\begin{pmatrix} x_1 \\ ... \\x_n\end{pmatrix}$$

$$\underline{m}=$$ mean vector

$$\underline{K}=$$ covariance matrix

$$n=1$$

$$\underline{m}=m$$

$$K= \sigma^2$$

$$\frac{exp(-\frac{1}{2} (\underline{x} - \underline{m})^T K^{-1} (\underline{x}-\underline{m}))}{(2 \pi)^{\frac{n}{2}} |K|^{\frac{1}{2}}}$$

$$\frac{exp(-\frac{1}{2} \frac{(x-m)^2}{\sigma^2})}{\sqrt{2 \pi \sigma^2}}$$

Properties of Gaussian Random vector

1. The joint PDF of $$X_1 ... X_n$$ is completely determined by mean vector and covariance matrix

2. $$\underline{x}=\begin{pmatrix} x_1 \\ ... \\x_n\end{pmatrix}$$ is Gaussian vector

   $$f_{X_1X_2}(x_1,x_2) \rightarrow$$ is going to a jointly Gaussian density

Lemma: Any marginal density of a jointly Gaussian density is itself a jointly Gaussian density

#### Example

$$\underline{X}=\begin{pmatrix}X_1 \\ X_2 \\X_3\end{pmatrix}$$

Gaussian vector

$$\underline{m}=\begin{pmatrix} 1 \\ 2 \\ 3 \end{pmatrix}$$

$$K= \begin{pmatrix} 1 & a  & b \\ a & 1 & c \\ b & c & 1\end{pmatrix}$$

$$f_{X_1X_2X_3}(x_1x_2x_3)=\frac{exp(-\frac{1}{2} (\underline{x} - \underline{m})^T K^{-1} (\underline{x}-\underline{m}))}{(2 \pi)^{\frac{3}{2}} |K|^{\frac{1}{2}}}$$

Marginal density of $$X_1$$

$$f_{X_1}(x_1)=\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f_{X_1X_2X_3}(x_1x_2x_3)dx_2dx_3$$

where $$f_{X_1}(x_1)$$ is a Gaussian density

$$\frac{1}{\sqrt{2 \pi \sigma^2}}exp(-\frac{(x-m)^2}{2 \sigma^2})$$

$$f_{X_1}(x_1)=\mathcal{N}(1,1)=\frac{1}{\sqrt{2 \pi}} exp(-\frac{(x-1)^2}{2})$$

Joint density of $$X_1$$ and $$X_2$$

$$f_{X_1X_2}(x_1x_2)=\int_{-\infty}^{\infty} f_{X_1X_2X_3}(x_1x_2x_3)dx_3$$

$$\frac{exp(-\frac{1}{2} (\binom{x_1}{x_2}-\binom{m_1}{m_2})^T K^{-1} (\binom{x_1}{x_2}-\binom{m_1}{m_2})}{\text{constant}}$$

$$\binom{m_1}{m_2}=\binom{1}{2}$$

$$\hat{K}=\begin{pmatrix} Var(X_1) & Cov(X_1,X_2) \\ Cov(X_2, X_1) & Var(X_2)\end{pmatrix}=\begin{pmatrix} 1 & a \\ a & 1 \end{pmatrix}$$

------

#### Example

$$\underline{X}=\begin{pmatrix}X_1 \\ X_2 \end{pmatrix}$$

Gaussian vector

$$\underline{m}=\begin{pmatrix} 0 \\ 0 \end{pmatrix}$$

$$K=\begin{pmatrix} 1 & p \\ p & 1 \end{pmatrix}$$

Correlation coefficient $$(X_1,X_2)=\frac{Cor(X_1,X_2)}{\sigma_{X_1} \sigma_{X_2}}=p$$

$$|K|=1-p^2$$

$$K^{-1}=\frac{1}{1-p^2} \begin{pmatrix} 1 & -p \\ -p & 1 \end{pmatrix}$$

$$f_{X_1X_2}(x_1x_2)= \frac{exp(-\frac{1}{2} \begin{pmatrix}(x_1 & x_2)\end{pmatrix} K^{-1} \begin{pmatrix}x_1 \\x_2\end{pmatrix}}{(2 \pi) \sqrt{1-p^2}}$$

$$=\frac{1}{2 \pi \sqrt{1-p^2}} exp(\frac{-1}{2 (1-p^2)} (x_1^2-2px_1x_2+x_2^2))$$

------

$$\underline{X}=\begin{pmatrix} X_1 \\ ... \\X_n\end{pmatrix}$$ is a Gaussian vector

$$\underline{m} = \begin{pmatrix} m_1 \\ ... \\ m_n \end{pmatrix}$$

$$K=\begin{pmatrix} \sigma_1^2 & 0 & ... & 0 \\ 0 & \sigma_2^2 & ... & 0 \\ ... & ... & ... & ... \\ 0 & ... & 0 & \sigma_n^2\end{pmatrix}$$

$$|K|=\sigma_1^2 ... \sigma_n^2$$

$$K^{-1}=\begin{pmatrix} \frac{1}{\sigma_1^2} & 0 & ... & 0 \\ 0 & \frac{1}{\sigma_2^2} & ... & 0 \\ ... & ... & ... & ... \\ 0 & ... & 0 & \frac{1}{\sigma_n^2}\end{pmatrix}$$

$$Var(X_i)=\sigma_i^2$$

$$Cov(X_i, X_j)=0, i \neq j$$

Is is true that $$X_1... X_n$$ are independent? 

i.e., $$f_{X_1 ... X_n} (x_1 ... x_n) =f_{X_1}(x_1) ... f_{X_n}(x_n)$$ ??? 

$$exp(-\frac{1}{2} (\underline{x} - \underline{m})^T \begin{pmatrix} \frac{1}{\sigma_1^2} & 0 & ... & 0 \\ 0 & \frac{1}{\sigma_2^2} & ... & 0 \\ ... & ... & ... & ... \\ 0 & ... & 0 & \frac{1}{\sigma_n^2}\end{pmatrix} (\underline{x}-\underline{m}))$$

$$exp(-\frac{1}{2} \begin{pmatrix}x_1-m_1 & x_2-m_2 & ... & x_n-m_n\end{pmatrix} \begin{pmatrix} \frac{1}{\sigma_1^2} & 0 & ... & 0 \\ 0 & \frac{1}{\sigma_2^2} & ... & 0 \\ ... & ... & ... & ... \\ 0 & ... & 0 & \frac{1}{\sigma_n^2}\end{pmatrix} \begin{pmatrix}x_1-m_1 \\ x_2-m_2 \\ ... \\ x_n-m_n\end{pmatrix}$$

$$exp(-\frac{1}{2} (\frac{(x_1-m_1)^2}{\sigma_1^2})+\frac{(x_2-m_2)^2}{\sigma_2^2})+...+\frac{(x_n-m_n)^2}{\sigma_n^2}))$$

$$exp(-\frac{1}{2} (\frac{(x_1-m_1)^2}{\sigma_1^2})) exp(-\frac{1}{2} (\frac{(x_2-m_2)^2}{\sigma_2^2}))+...+exp(-\frac{1}{2} (\frac{(x_n-m_n)^2}{\sigma_n^2}))$$

$$f_{X_1 ... X_n} (x_1 ... x_n)=\prod_{i=1}^{n} f_{X_i}(x_i)$$

$$f_{X_1}(x_1)...f_{X_n}(x_n)$$

$$\implies X_1 ... X_n$$ are independent

Lemma: $$\underline{X}$$ is Gaussian vector and $$K$$ is a diagonal matrix. Then, $$X_1 ... X_n$$ are independent random variables

#### Example

$$\underline{X}=\begin{pmatrix}X_1 \\ X_2 \end{pmatrix}$$ is a Gaussian vector

$$Cov(X_1,X_2)=0$$

$$K_X=\begin{pmatrix} Var(X_1) & 0 \\ 0 & Var(X_2)\end{pmatrix}$$

$$\implies X_1,X_2$$ are independent

Recall: 

1. If $$X_1, X_2$$ are independent, then $$Cov(X_1,X_2)=0$$
2. In general, $$Cov(X_1,X_2)=0$$ does not imply $$X_1,X_2$$ independent
3. If $$\underline{X}=\begin{pmatrix}X_1 \\ X_2 \end{pmatrix}$$ is Gaussian vector, and $$Cov(X_1X_2)=0$$, then $$X_1,X_2$$ are independent

Theorem: 

If $$\underline{X}=\begin{pmatrix} X_1 \\ ... \\X_n\end{pmatrix}$$ is jointly Gaussian vector

$$\underline{Y}=A \underline{X}$$

Then $$\underline{Y}$$ is also a jointly Gaussian vector

$$m_{\underline{Y}}=A m_{\underline{X}}$$

$$K_Y=AK_XA^T$$

#### Example

$$X_1,X_2,X_3$$ are jointly Gaussian

$$Y=a_1X_1+a_2X_2+a_3X_3$$

$$Y=\begin{pmatrix} a_1 & a_2 & a_3 \end{pmatrix} \begin{pmatrix} X_1 \\ X_2 \\ X_3\end{pmatrix}$$

$$\implies Y$$ is a Gaussian random variable

$$m_Y=A \begin{pmatrix} m_1 \\ m_2 \\ m_3\end{pmatrix}=a_1m_1+a_2m_2+a_3m_3$$

$$\sigma_Y^2=AK_XA^T$$

$$=\begin{pmatrix} a_1 & a_2 & a_3 \end{pmatrix} K_X \begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix}$$

## Discussion 13

### Outlines

1. Problems

   Vector Random Variables

   Transformation of vector RVs

2. Application of Leibniz integral role

------

### Question 1

The point $$\bold{X}=(X,Y, Z)$$is uniformly distributed inside a sphere of radius 1 about the origin. Find the probability of the following events:(a) $$\bold{X}$$ is inside a sphere of radius $$r,r>0$$

![image-20241125143050610](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241125143050610.png)

$$\underline{X}=(X,Y,Z)$$

$$P(X^2+Y^2+Z^2 \leq r^2 |X^2+Y^2+Z^2 \leq 1)$$

Event $$A: X^2+Y^2+Z^2\leq r^2$$

Event $$B: X^2+Y^2+Z^2 \leq 1$$

$$A \subset B$$

$$P(B|A)=\frac{P(A \bigcap B)}{P(A)}$$

$$=\frac{P(X^2+Y^2+Z^2 \leq r^2)}{P(X^2+Y^2+Z^2 \leq 1)}$$

$$=\frac{4/3 \pi r^3}{ 4/3 \pi 1^3}=r^3$$

(b) $$\bold{X}$$ is inside a cube of length $$2/\sqrt3$$ centered about the origin.

![image-20241125143514031](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241125143514031.png)

The cube is centered at the origin, with side length $$\frac{2}{\sqrt{3}}3$$, meaning each side extends from $$-\frac{1}{\sqrt{3}} \text{\:to\:} \frac{1}{\sqrt{3}}$$

$$P(|X| \leq \frac{1}{\sqrt{3}}) \bigcap  |Y| \leq \frac{1}{\sqrt{3}}) \bigcap |Z| \leq \frac{1}{\sqrt{3}}) |X^2+Y^2+Z^3 <1)$$

$$=\frac{\text{Volume of inner cube}}{\text{Volume of the sphere}}$$

$$=\frac{ \frac{2}{\sqrt{3}} \frac{2}{\sqrt{3}} \frac{2}{\sqrt{3}} }{4/3 \pi r^3}$$

$$=\frac{2}{\sqrt{3} \pi}$$

(c) All components of $$\bold{X}$$ are positive.

$$P(X>0 \bigcap Y>0 \bigcap Z>0 | X^2+Y^2+Z^2 \leq 1)$$

$$=\frac{\text{Volume of positive octont}}{\text{Volume of the sphere}}$$

| X    | Y    | Z    |
| ---- | ---- | ---- |
| +    | +    | +    |
| +    | +    | -    |
| +    | -    | +    |
| +    | -    | -    |
| -    | +    | +    |
| -    | +    | -    |
| -    | -    | +    |
| -    | -    | -    |

$$=\frac{1/8 \cdot 4/3 \pi 1^3}{4/3 \pi 1^3}=1/8$$

(d) $$Z$$ is negative.

$$P(Z<0|X^2+Y^2+Z^2 \leq 1)$$

$$=\frac{\text{Volume of semisphere}}{\text{Volume of the sphere}}$$

$$=\frac{1/2 (4/3 \pi 1^3)}{4/3 \pi 1^3}=1/2$$

------

### Question 2

A random sinusoid signal is given by $$X(t)= A \sin(t)$$ where $$A$$ is a uniform random variable in the interval $$[0, 1]$$.Let $$\bold{X}=(X(t_1), X(t_2), X(t_3))$$ be samples of the signal taken attimes $$t_1 , t_2, \text{and\:} t_3$$.

(a) Find the joint CDF of $$\bold{X}$$ in terms of the CDF of $$A$$ if $$t_1=0, t_2=\pi/2, t_3=\pi$$ Are $$X(t_1), X(t_2), X(t_3)$$ independent random variables?

![image-20241125192827648](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241125192827648.png)

$$X(t)= A \sin(t)$$

$$A \sim \text{Uniform} [0,1]$$

$$\underline{X}=(X(t_1), X(t_2), X(t_3))$$

$$F_{\underline{X}}(X(t_1), X(t_2), X(t_3))=P(X(t_1) \leq x_1,  X(t_2) \leq x_2, X(t_3) \leq x_3)$$

$$X(t_1)=X(0)=0, X(t_2)=X(\pi/2)=A, X(t_3)=X(\pi)=0$$

$$\underline{X}=(0, A, 0)$$

$$P(0 \leq x_1, A \leq x_2, 0 \leq x_3)$$

the conditions $$x_1 \geq 0, x_3 \geq 0$$ is always true, because $$X(t_1)=X(t_3)=0$$

$$A \sim \text{Uniform}[0,1]$$

$$P(A \leq x_2) = \begin{cases} 0 & x_2< 0 \\ x_2 & 0 \leq x_2 \leq 1 \\ 1 & x_2> 1 \end{cases}$$

------

### Question 3

A radio transmitter sends a signal $$s>0$$ to a receiver using three paths. The signals that arrive at the receiver along each path are:

$$X_1=s+N_1$$ ,$$X_2=s+N_2$$, $$X_3=s+N_3$$ where $$N_1, N_2, N_3$$ are independent Gaussian random variables with zero mean and unit variance.

(a) Find the joint pdf of $$\bold{X}=(X_1,X_2,X_3)$$.  Are $$X_1, X_2 \text{\:and\:} X_3$$ independent random variables?

$$X_1, X_2, X_3$$

$$N_1,N_2,N_3 \sim \mathcal{N}(0,1)$$

Identically distributed and independent

$$F_{\underline{X}}(x_1,x_2,x_3)=P(X_1 \leq x_1, X_2 \leq x_2, X_3 \leq x_3)$$
$$=P(s+N_1 \leq x_1, s+N_2 \leq x_2,  s+N_3 \leq x_3)$$

$$=P(N_1 \leq x_1-s, N_2 \leq x_2-s, N_3 \leq x_3-s)$$

$$=P(N_1 \leq x_1-s)P(N_2 \leq x_2 -s )P(N_3 \leq x_3-s)$$

Since $$N_1,N_2,N_3 \sim \mathcal{N}(0,1)$$

$$f_{\underline{X}}(x_1,x_2,x_3)=f_{N_1}(x_1-s) f_{N_2}(x_2-s)f_{N_3}(x_3-s)$$

$$=\frac{1}{\sqrt{2} \pi} exp(-\frac{(x_1-s)^2}{2}) \frac{1}{\sqrt{2} \pi} exp(-\frac{(x_2-s)^2}{2}) \frac{1}{\sqrt{2} \pi} exp(-\frac{(x_3-s)^2}{2}) $$

(b) Find the probability that the minimum of all three signals is positive. 

$$P(\min(X_1,X_2,X_3)>0)$$ since $$\min$$ is $$>0$$

$$=P(X_1 >0, X_2>0, X_3>0)$$

$$=P(N_1 \geq -s, N_2 \geq -s, N_3 \geq -s)$$

Because of independence

$$=P(N_1 \geq -s)P(N_2 \geq -s)P(N_3 \geq -s)$$

$$N_1, N_2, N_3$$ are identically distributed

$$=(P(N \geq -s))^3$$

$$=(1-F_N(-s))^3$$

(c) Find the probability that a majority of the signals are positive.

Majority $$\implies $$ exactly 3 signals are positive or 2 signals are positve

$$P(X_1 >0, X_2>0, X_3>0)+P(X_1 \leq 0, X_2 >0, X_3>0)+P(x_1 >0, X_2 \leq 0, X_3>0) +P(X_1>0, X_2>0, X_3 \leq 0)$$

$$=(1-F_N(-s))^3+3 F_{N}(-s) (1-F_N(-s))^2$$

------

### Question 4

Use auxiliary variables to find the pdf of $$Z=X_1X_2X_3$$ where the $$X_i$$ are independent random variables that are uniformly distributed in $$[0, 1]$$

$$X_i \sim \text{Uniform}[0,1]$$

$$Z =g(X_1,X_2,X_3) :=X_1X_2X_3$$

$$f_{X_1X_2X_3}(x_1,x_2,x_3)=f_{X_1}(x_1) f_{X_2}(x_2) f_{X_3}(x_3)$$

$$f_{X_i}(x_i)=\begin{cases} 1 & 0 \leq x_i \leq 1 \\ 0 & \text{otherwise}\end{cases}$$

$$f_{X_1X_2X_3}(x_1,x_2,x_3)=\begin{cases} 1 & 0 \leq x_1, x_2 , x_3 \leq 1 \\ 0 & \text{otherwise}\end{cases}$$

Transformation

Let $$U=X_2, V=X_3$$ (auxiliary RVs)

$$Z:= XUV$$

Find PDF of $$Z$$

$$f_{Z,U,V}(z,u,v)=\frac{f_{X,U,V}(x,u,v)}{J_{X_1X_2X_3}}$$

$$J_{X_1X_2X_3}=det \begin{bmatrix} \frac{\partial Z}{\partial X_1} & \frac{\partial Z}{\partial X_2} & \frac{\partial Z}{\partial X_3} \\ \frac{\partial U}{\partial X_1} & \frac{\partial U}{\partial X_2} & \frac{\partial U}{\partial X_3} \\ \frac{\partial V}{\partial X_1} & \frac{\partial V}{\partial X_2} & \frac{\partial V}{\partial X_3}\end{bmatrix}$$

$$=det \begin{bmatrix} x_2x_3 & x_1x_3 & x_1x_2 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{bmatrix}$$

$$=x_2x_3$$

$$f_{Z,U,V}(z,u,v)=\begin{cases} \frac{1}{UV} & 0 \leq \frac{Z}{UV} \leq 1, 0 \leq U \leq 1, 0 \leq V \leq 1 \\ 0 & \text{otherwise}\end{cases}$$

$$V \geq \frac{Z}{U} \rightarrow \frac{Z}{UV} \leq 1, U \geq Z$$

$$f_{Z}(z)=\int_{U=Z}^{1} \int_{V= \frac{Z}{U}}^{1} f_{Z,U,V}(z,u,v)dUdV$$

 $$f_{Z}(z)=\int_{V=Z}^{1} \int_{V=\frac{Z}{U}}^{1} \frac{1}{UV} dUdV$$

$$=\frac{1}{Z} (\ln(Z))^2$$

------

### Leibniz Integral Rule

$$f_{U}(u)$$ marginal PDF

$$F_{XY}(u,v)$$ Joint CDF

Joint CDF $$\rightarrow$$ Marginal CDF $$\rightarrow$$ Marginal PDF

$$F_{XY}(U,V)=\int_{y} \int_{x} f_{XY}(x,y)dydx$$

$$=\int_{y} g(u,y) dy$$

$$f_U(u)=\frac{d}{dU} \int_{y} g(u,y)dy$$

Differential under integral sign

$$\frac{d}{dU} \int_{y= P(U)}^{q(U)} g(u,y) dy= g(U, q(U)) \frac{d}{dU} q(U) - g(U,p(U))\frac{d}{dU}p(U)+\int_{P(U)}^{q(U)}\frac{\partial}{\partial U} g(U,y)dy$$

If the integral limits are constants

$$\frac{d}{dU} \int_{y=0}^{c} g(u,y)dy=\int_{y=0}^{c}\frac{\partial}{\partial U} g(U,y)dy$$

## Week 14 Session 1 (Only 1)

### Limit Theorem

IID sequence of Random Variables $$X_1,X_2,X_3, ... $$

Independent

Identically distributed: same CDF/ same PMF / same PDF

$$E[X_i]=\mu$$

$$Var[X_i]=\sigma^2$$

$$\mu,\sigma^2$$ are finite numbers

$$S_n=\sum_{i=1}^{n}X_i$$        - Sum of $$X_1,...,X_n$$

$$M_n=\frac{S_n}{n}=\frac{\sum_{i=1}^{n}X_i}{n}$$ - Sample mean of $$X_1,...,X_n$$

$$E[S_n]=E[\sum_{i=1}^{n}X_i]=\sum_{i=1}^{n}E[X_i]=n \mu$$
$$Var[S_n]=Var[\sum_{i=1}^{n}X_i]=n \sigma^2$$

$$Var[S_n]=E[(S_n-n \mu)^2]$$

$$=E[(\sum_{i=1}^{n}(X_i-\mu))^2]$$

$$=E[\sum_{i=1}^{n} (X_i-\mu)^2 + \sum_{i=1}^{n} \sum_{j=1, j \neq i}^{n} (X_i-\mu)(X_j-\mu)]$$

$$=\sum_{i=1}^{n} Var[X_i] + \sum \sum_{i \neq j} Cov(X_i, X_j)$$

where $$Cov(X_i,X_j)=0$$
$$=n \sigma^2$$

$$E[M_n]=E[\frac{S_n}{n}]=\frac{1}{n} E[S_n]=\mu$$

$$Var[M_n]=Var[\frac{S_n}{n}]=\frac{1}{n^2} Var[S_n]=\frac{n \sigma^2}{n^2} =\frac{\sigma^2}{n}$$

------

$$X_1,...,X_n$$ IID RVs with finite mean and finite variance

Unknown $$\mu$$

Estimate for $$\mu \rightarrow$$ Sample mean $$M_n$$

$$M_n=\frac{\sum_{i=1}^{n}X_i}{n}$$

Consider a $$\epsilon >0$$

$$P(|M_n-\mu| \geq \epsilon)$$

Using Chebyshev Inequality

$$P(|M_n-\mu| \geq \epsilon) \leq \frac{Var[M_n]}{\epsilon^2}=\frac{\sigma^2}{n \epsilon^2}$$

$$X_1, X_2...$$ continuous with PDF $$f$$

$$M_1=\frac{X_1}{1}=X_1$$

![image-20241127204856606](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127204856606.png)

$$M_{10}=\frac{X_1 + ... + X_10}{10} $$

![image-20241127204919974](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127204919974.png)

$$M_{100}$$

![image-20241127205003662](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127205003662.png)

The shadow area shrinks

#### Example

Measure an unknown voltage $$v$$ using a noisy sensor

$$X_i=v+N_i$$      - $$i^{th}$$ measurement

$$M_n=\frac{X_1+...X_n}{n}$$ 

$$N_1, N_2... $$ IID RVs with 0 mean and variance 1

How man measurement should I take to get $$M_n$$ and $$v$$ within 1 unit distance with probability at least 0.99?

$$X_1, X_2, ... X_n$$ are IID RVs

$$E[X_i]=E[v+N_i]=v$$

$$Var[X_i]=Var[v+N_i]=1$$

$$P(|M_n-v|<1) \geq 0.99 \implies P(|M_n-v|\geq 1)\leq 0.01$$

$$P(|M_n-v|\geq 1)\leq 0.01 \leq \frac{\sigma^2}{n \cdot 1}=\frac{1}{n}$$

Pick $$n$$ such that $$\frac{1}{n} \leq 0.01$$
$$n\geq 100$$

------

### Weak Law of Large Numbers

If $$X_1, X_2, ... $$ is IID sequence of RVs with finite mean $$\mu$$, finite variance $$\sigma^2$$. Then for all $$\epsilon >0$$

$$\lim_{n \rightarrow \infty} P(|M_n-\mu|\geq \epsilon)=0$$

$$\lim_{n \rightarrow \infty} P(|M_n-\mu|< \epsilon)=1$$

#### Example

Coin with unknown probability of heads $$0\leq p \leq 1$$

Toss the coin $$n$$ times, tosses are independent

$$X_i=\begin{cases} 1 & \text{if\:} i^{th} \text{\:toss is H} \\ 0 &  \text{if\:} i^{th} \text{\:toss is T} \end{cases}$$

$$E[X_i]=p$$

$$Var[X_i]=E[X_i^2]-p^2$$

$$=p-p^2=p(1-p)$$

$$M_n=\frac{\sum_{i=1}^{n}X_i}{n}$$

$$P(|M_n-p|\geq 0.1) \leq \frac{Var[X_i]}{n \cdot 0.1^2}=\frac{p(1-p)}{n \cdot 0.01}$$

![image-20241127210517466](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127210517466.png)

Function of $$p(1-p)$$, max at $$1/4$$

$$P(|M_n-p|\geq 0.1) \leq \frac{1/4}{n \cdot 0.01}=\frac{25}{n}$$

If $$n=250$$

$$P(|M_n-p|\geq 0.1) \leq \frac{1}{10}$$

Equivalently, $$P(|M_n-p| < 0.1) \geq 0.9$$

------

### Strong Law of Large Numbers

If $$X_1, X_2, ... $$ is IID sequence of RVs with finite mean $$\mu$$, finite variance $$\sigma^2$$.

Sequence if sample means

$$M_1=\frac{X_1}{1}=X_1$$

$$M_{2}=\frac{X_1  + X_2}{2} $$

$$M_{n}=\frac{X_1 + ... + X_n}{n} $$

$$\epsilon=\{M_n \text{converges to} \mu, \text{i.e.,} \lim_{n \rightarrow \infty} M_n=\mu \}$$

Strong law of large number states that $$\epsilon$$ has probability 1

------

Example

6-sided die with unknown probabilities for each side. Would like to estimate probabilities of an even number showing up.

Roll the die $$n$$ times. Rolls are independent. Calculate the relative frequency of even numbers.

Relative frequency= $$\frac{\text{Total number of rolls with even number}}{n}$$

$$X_i=\begin{cases} 1 & \text{if even number shows on\:} i^{th} \text{\: roll} \\ 0 & \text{otherwise}\end{cases}$$

$$\frac{\sum_{i=1}^{n}X_i}{n}=$$ Relative frequency of even number

Strong law

$$\frac{\sum X_i}{n} \rightarrow E[X_i]$$ as $$n \rightarrow \infty=P(\text{even number})$$ 

Sample mean, True mean

Sum $$S_n=\sum_{i=1}^{n}X_i$$

------

### Central Limit Theorem

$$X_1,X_2...$$ IID sequence with finite mean $$\mu$$ and finite variance $$\sigma^2$$

$$E[S_n]=n \mu$$

$$Var[S_n]=n \sigma^2$$
$$Y_n=\frac{S_n - E[S_n]}{\sqrt{Var(S_n)}}$$

$$E[Y_n]=E[\frac{S_n - E[S_n]}{\sqrt{Var(S_n)}}] =0$$

$$Var[Y_n]=Var(\frac{S_n - E[S_n]}{\sqrt{Var(S_n)}})$$

$$=\frac{1}{\sqrt{Var(S_n}} Var(S_n)=1$$

CDF of $$Y_1$$
$$Y_1=\frac{S_1-E[S_1]}{\sqrt{Var(S_1)}}$$

$$S_1=X_1$$

$$Y_1=\frac{X_1-\mu}{\sigma}$$

$$F_{Y_1}(y)=P(Y_1 \leq y)$$

$$=P(\frac{X_1-\mu}{\sigma}\leq y)$$

$$=P(X_1 \leq \mu+\sigma y)$$

$$=F_{X_1}(\mu+\sigma y)$$

CDF of $$Y_2$$

$$P(Y_2 \leq y)=P(\frac{S_2-2\mu}{\sigma \sqrt{2}} \leq y)$$

$$=P(S_2 \leq 2 \mu + \sigma \sqrt{2} y)$$

$$=(X_1+X_2 \leq 2 \mu + \sigma \sqrt{2} y)$$

![image-20241127212010791](C:\Users\Levi\AppData\Roaming\Typora\typora-user-images\image-20241127212010791.png)

$$P(Y_n \leq y)$$

$$P(S_n \leq \text{threshold})$$

------

### Central Limit Theorem

$$X_1,X_2...$$ IID sequence with finite mean $$\mu$$ and finite variance $$\sigma^2$$

$$Y_n=\frac{S_n - E[S_n]}{\sqrt{Var(S_n)}}$$

$$\lim_{n \rightarrow \infty}F_{Y_n}(y)=\phi(y)$$ for all $$y \in \R$$ where $$\phi$$ is the CDF of standard normal distribution

#### Example

Continuous IID RV with mean $$\mu$$ and variance $$\sigma^2$$

$$X_1,X_2, ...$$

$$P(\sum_{i=1}^{n}X_i >t)=P(S_n >t)$$

$$=P(\frac{S_n-E[S_n]}{\sqrt{Var(S_n)}} > \frac{t-n \mu}{\sigma \sqrt{n}})$$

$$=P(Y_n > \frac{t- n \mu}{\sigma \sqrt{n}})$$

$$=1-F_{Y_n}(\frac{t-n \mu}{\sigma \sqrt{n}})$$

$$\approx 1- \phi(\frac{t-n \mu}{\sigma\sqrt{n}})$$

#### Example

$$n$$ independent coin tosses

Probabilities of $$H=p$$

$$X_i=\begin{cases} 1 & \text{if\:} H \text{ on\:} i^{th} \text{\: toss} \\ 0 & \text{otherwise}\end{cases}$$

$$k$$ is some positive integer

$$P(\sum_{i=1}^{n} X_i > k)=P(\sum_{i=1}^{n} X_i > k+0.5)$$

$$=P(S_n > k+0.5)$$

$$=P(\frac{S_n-np}{\sqrt{n (p-p^2)}} > \frac{k+0.5-np}{\sqrt{n (p-p^2)}})$$

$$=P(Y_n > \frac{k+0.5-np}{\sqrt{n (p-p^2)}})$$

$$\approx 1- \phi(\frac{k+0.5-np}{\sqrt{n (p-p^2)}})$$

$$P(\text{Total number of\:} H \text{\:in\:} n \text{\:independent tosses} >k)$$

Total number of $$H$$ has a <u>binomial distribution</u>

$$P(S_n>k)=\sum_{s=k+1}^{n}P_{S_n}(s)=\sum_{s=k+1}^{n}\binom{n}{s}p^s(1-p)^{n-s}$$

$$n=30, p =\frac{1}{30}$$

$$P(S_n >2)$$ 

Exact value from binomial distribution 0.077

Approximated value using CLT 0.064

$$P(\sum X_i >k)=P(\sum X_i \geq k+1)$$

$$=P(S_n \geq k+1)$$

$$=P(\frac{S_n - E[S_n]}{\sqrt{Var(S_n)}} \geq \frac{k+1-np}{\sqrt{n (p-p^2)}})$$

------

#### Example

10 fair 6-sided dice are rolled

Sum of 10 numbers

Approximate the probability that the sum is between 30 and 40

$$E[X_i]=3.5$$

$$Var[X_i]=\frac{35}{12}$$

$$S_{10}=X_1+...+X_{10}$$

$$P(30 \leq S_{10} \leq 40)$$

$$=P(29.5 \leq S_{10} \leq 40.5)$$

$$=P(\frac{29.5-35}{\sqrt{\frac{350}{12}}} < \frac{S_{10}-(10)(3.5)}{\sqrt{\frac{35}{12}} \sqrt{10}} \leq \frac{40.5-35}{\sqrt{\frac{350}{12}}})$$

$$\approx \phi(b)-\phi(a)$$

 where $$a=\frac{29.5-35}{\sqrt{\frac{350}{12}}}, b=\frac{40.5-35}{\sqrt{\frac{350}{12}}}$$



















































