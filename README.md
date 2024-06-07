# Grokking_FizzBuzz

We proposed a way to evaluate neural network compression in grokking problems using the Gini coefficient, which is used in economics and machine learning. Grokking was considered on a well-known problem for computer scientists -- FizzBuzz. The results of an empirical study indicate a strong stratification of the weights of the neural network in terms of significance. The proposed ideas and judgments may help in further understanding the work of neural networks.

Grokking is one of these phenomena. Grokking is a phenomenon in which a neural network continues learning after fully memorizing training data. That is, the loss-function on the validation data drops after several iterations with zero error on the training data. Previously, there was a rule that you need to stop learning, but now scientists are reconsidering old approaches. Grokking was tried to be explained as compression of neural networks, and others similar explanations. In this article, we will continue to develop this idea, however, we will consider the FizzBuzz problem and analyze the weights of the neural network using the economic Gini coefficient, developed by Italian statistician and sociologist Corrado Gini.

The Gini coefficient is defined as 

$$G = \frac{\sum_{i=1}^n \sum_{j=1}^n |x_i-x_j|}{2n^2\bar{x}},$$
where $n$ is the number of elements, $\bar{x}$ is the mean value. 
For sorted array it can be written in form 
$$G = \frac{2}{n^2\bar{x}} \sum_{i=1}^n i(x_i-\bar{x}).$$
In this article, we found groking in the FizzBuzz task. The task is formulated as follows: 

Players generally sit in a circle. The player designated to go first says the number "one", and the players then count upwards in turn. However, any number divisible by three is replaced by the word fizz and any number divisible by five by the word buzz. Numbers divisible by both three and five (i.e. divisible by fifteen) become fizz buzz. A player who hesitates or makes a mistake is eliminated.


