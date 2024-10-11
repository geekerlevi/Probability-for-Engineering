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







