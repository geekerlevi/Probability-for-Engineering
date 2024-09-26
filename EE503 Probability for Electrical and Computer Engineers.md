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

$$P(\{1\})=P(\{2\})=P(\{3\})=P(\{4\})=P(\{5\})=5/12$$

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

Probability that exactly 5 of selected items are defective

$$\frac{\binom{10}{5}\binom{40}{5}}{\binom{50}{10}}$$

------

#### Example

32 bit binary number. How many such numbers have exactly 5 zeros

$$\binom{32}{5}$$

------





