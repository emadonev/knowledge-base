---
tags:
  - mathematics
  - algebra
---
Operations in math stack cumulatively. In *addition*, we have $2+2$, but if we want to add 2 to itself many times, we use *multiplication*: $2*5$. *Subtraction and division* are the inverses of addition and multiplication. We want to know for subtraction the *backwards step*, and for division ==which number times 2 gives some outcome.== 

Now, if we want to multiply the same number by itself many times, we get the **power function.** For example:$$2*2*2*2 = 2^4 = 16$$
$2$ is the base, $4$ is the exponent, and $16$ is the result. Since we have **3** numbers in the relationship, and not 2, we have **3 different ways of approaching the power - *with 2 inverses.*** We can imagine this as a triangle, with $2$ in the bottom left corner, $4$ at the top, and the result at the bottom right. 
- If we want to know **which number to the power of 4 is 16**, we use ***==the root function==*** or:$$\sqrt[4]{16} = 2$$
- If we would rather like to know **which number we need to take to the power of 2 to get 16**, we use our subject, ***==the logarithm function==***:$$\log_2(16) = 4$$

---
> In a basic form, **logarithms** search for the exponent needed to take a certain base to the power of to get a number. Logarithms are used all the time in statistics, in engineering and in the real world to model and create understandable graphs. 

Now, we can start to discuss some properties of logarithms since we have a bit of an intuition as to what they are.

### 01 Multiplication
The first property is as such:$$\log(a*b) = \log(a) + \log(b)$$
This rule comes from the power addition rule:$$a^x * a^y = a^{x+y}$$
In logarithms, both $a$ and $b$ are of the same base, and so then the log of the multiplication of 2 numbers has to equal the addition of them, since $x = \log_a (a^x)$, and the same goes for $y$.

### 02 Division
The same property for multiplication applies for division, since the same power rule applies:$$\log(\frac{a}{b}) = \log(a) - \log(b)$$

### 03 Powers
The next property is:$$\log(a^n) = n\log(a)$$, and this stems from the following rule:$$(a^x)^y = a^{xy}$$, and so we can just take the exponent right out, since its just multiplying that number by the exponent we get by logarithming a.

### 04 Changing bases
When thinking about this rule:$$\log_c(b) * \log_b(a) = \log_c(a)$$, it might not make sense. However, if we put it like this:$$c^x = b,\;\;\;b^y = a \ce{->} \;c^{xy} = a$$, hence if we take the log of $b$ with base $c$ we get $x$, and the same goes for $b$ of $a$ when we get $y$, and their product is simply the log of $a$ base $c$. 

### 05 $1/$ something
Our final property is:$$\log_a(b) = \frac{1}{\log_b(a)}$$
This stems from the fact that:$$a^x = b$$, and if we want to rewrite that in terms of $a$ as $b$, then$$a = b^{1/x}$$, hence the fractional form.


