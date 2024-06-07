# Grokking_FizzBuzz

We proposed a way to evaluate neural network compression in grokking problems using the Gini coefficient, which is used in economics and machine learning. Grokking was considered on a well-known problem for computer scientists -- FizzBuzz. The results of an empirical study indicate a strong stratification of the weights of the neural network in terms of significance. The proposed ideas and judgments may help in further understanding the work of neural networks.


The Gini coefficient is defined as 
\begin{equation}
G = \frac{\sum_{i=1}^n \sum_{j=1}^n |x_i-x_j|}{2n^2\bar{x}},
\end{equation}
where $n$ is the number of elements, $\bar{x}$ is the mean value. 
For sorted array it can be written in form 
\begin{equation}
G = \frac{2}{n^2\bar{x}} \sum_{i=1}^n i(x_i-\bar{x}).
\end{equation}
In this article, we found groking in the FizzBuzz task. The task is formulated as follows: \\

\textit{Players generally sit in a circle. The player designated to go first says the number "one", and the players then count upwards in turn. However, any number divisible by three is replaced by the word fizz and any number divisible by five by the word buzz. Numbers divisible by both three and five (i.e. divisible by fifteen) become fizz buzz. A player who hesitates or makes a mistake is eliminated.}
