TAGS: #probability #mathematics #functions 

This function is used in **continuous [[Random variables]]**, where they can take on an infinite range of numbers. So, instead of calculating the probability of a specific event (since the [[Probability]] would be 0), we calculate the probability for a **range of values.** This is done by a process in [[Calculus]] called [[Integration]]. This function has to fulfil 2 important conditions:
1. The value of the function is always positive!
2. The sum of all the possible probabilities in the range is 1, or 100%. 

The way to use this function is to ask the question: which PDF describes the data I have just observed? If we have a weighted coin, and we toss it 10 times and out of 10 we get 7 times heads, instead of asking what is the probability of getting heads, we ask how would the PDF look like based on this observation. 

![[PDF_1.png]]
![[PDF_2.png]]
![[PDF_3.png]]
![[PDF_4.png]]

So what is the formula for a pdf? 
$$P(a<x<b)=\int_a^b p_x(x) dx$$
What this means is that between a range of 2 values, $a,b$ the probability of finding your desired number $x$ is the **area under the curve from a to b**, where the height is a function of probability for x, and the width is the change in x, commonly known as a [[Derivative]] in calculus, $dx$. 

