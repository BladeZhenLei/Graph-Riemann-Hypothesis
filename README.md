***
The famous Riemann hypothesis is closely related to the distribution of primes. In graph theory, by defining prime paths, a graph is said to be Ramanujan if and only if its Ihara zeta function satisfies an analogy of the Riemann hypothesis. The concept of Ihara zeta function was first realized by Yasutaka Ihara in the group theory language and Jean-Pierre Serre related it to graphs. It was 1985 when Toshikazu Sunada proposed the graph theory version of the Riemann hypothesis, which was further extended by A.A.Terras and H.M. Stark.

###  Prime Paths
For a connected, finite graph $X$, its edges can be labeled as $(e_1, e_2, ..., e_m)$, $e_{m+1}=e_1^{-1}$ and $e_{2m}=e_m^{-1}$, where $m=|E(X)|$ is the non-oriented edeges, and $e_j^{-1}=e_{j+m}$ denote opposite orientation. Then, we can define paths $C=(a_1,a_2,...,a_n)$, where $a_i$ is an oriented edge of $X$, there exist a $backtracking$ if $a_{i+1}=a_i^{-1}$, the path is said to have a $tail$ if $a_{n}=a_1^{-1}$. The path $C$ is a $closed$ $path$ or a $cycle$ when it consists of vertices $(v_1,v_2,...,v_m=v_1)$, and the closed path is $primitive$ if it has no tail or backtracking and $C\neq{D^f}$ for $f>{1}$, meaning the path is only allowed once.

For a closed path $C$, the $equivalence$ $class$ $[C]$ is defined as 
$$[C]=\lbrace{a_1}\cdot\cdot\cdot{a_n},{a_2}\cdot\cdot\cdot{a_n},{a_n}{a_1}\cdot\cdot\cdot{a_{n-1}}\rbrace,$$
two paths are called $equivalent$ if one can be obtained from the other by changing the starting vertex. 
A $prime$ in $X$ is an equivalence class $[C]$ of prime paths, the path length is the edge count $v(C)=n$.

<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/187326050-c8d93df8-d35c-4b4f-a9e4-c5ef29b08945.png" width="240" height="210"> <p/>
<p align="center"> Arbitrary orientation for $(e_1,e_2,e_3,e_4,e_5)$ </p>

The Ihara zeta function is computed by the product over the equivalence class of prime paths. 
<br/>
Some examples of primes are 
$$[C]=\lbrace{e_2}{e_3}{e_5}\rbrace,$$ 
$$[D]=\lbrace{e_1}{e_2}{e_3}{e_4}\rbrace,$$
$$[E]=\lbrace{e_1}{e_2}{e_3}{e_4}{e_1}{e_{10}}{e_4}\rbrace.$$ 
Here, $e_{10}={e_5}^{-1}$ is the backtracking, the path lengths are 3, 4, 7, and there are infinitely many primes.

### Zeta Function of Graphs
Consider a cycle graph $X$ with $n$ vertices, shown in Fig.2. There are two primitive paths, one going around clockwise once, and the other going around counterclockwise once. The corresponding zeta function will be 
$$\zeta_X\left(u\right)=\prod_{\left\[C\right\]}{({1-u^{v\left(C\right)})}^{-1}} = ({1-u^{n})}^{-1}({1-u^{n})}^{-1}.$$
This is the simplest case of the graph zeta function, where no computation of the prime class was considered. Furthermore, if there exist a prime path, then there would be a prime power decomposition into graphs.

<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/187325623-ef6c34c3-656e-4ffc-b173-2135757965ce.png" width="150" height="140"> <p/>
<p align="center"> n-cycle graph</p>

### Ramanujan Graphs
Consider a finitely connected $k$-regular graph $X$ with its adjacency matrix $A$, it is said that if $\lambda(A)\neq{\pm{k}}$, then it is a non-trivial solution, and the graph is called a $Ramanujan$ $graph$, if and only if that all $\lambda$ of $A$ satisfies $|\lambda|\leq{2\sqrt{k-1}}$.
<p/>

The complete graph $K_n$ is a Ramanujan graph, its adjacency matrix has the characteristic polynomial $(\lambda-(n-1))(\lambda+1))^{n-1}.$
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/187332359-5131ca2b-bc71-433d-a76d-bc8fb6b393c3.PNG" width="180" height="170"> <p/>
<p align="center"> n-complete graph </p>
The verification involves computation of circulant matrix.
<p/>

Consider the Peterson graph, which has $(\lambda-3)(\lambda+2)^4(\lambda-1)^5,$ one can easily check that $2\leq2\sqrt{2}.$
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/187332360-47bc5e53-13f1-4ae0-b65d-4d5817294e7e.png" width="160" height="150"> <p/>
<p align="center"> Peterson graph </p>

A random k-regular graph has $\lambda_{2}\leq{2\sqrt{(k-1)}+2log(k)+O(1)}.$ This gives the precise measurement of the graphs in terms of the eigenvalue function and shows that the Ramanujan graphs have small diameters.

Let $X$ be a $q+1$ regular connected graph,
then we have the reciprocal polynomial of zeta function 
$$\zeta_X^{-1}\left(u\right)=\left(1-u^2\right)^{r-1}det\left(I-Au+qu^2I\right).$$
Here, $A$ is the adjacency matrix and $r$ is the $rank$ of the $fundamental$ $group$ of $X$. Extending this notion, one can find that 
$$\zeta_X\left(u\right)=\exp{(\sum_{n=1}^{\infty}{N_mu^{m})}},$$
where $N$ is the number of closed paths in $X$ of length $m$ with no backtracking or tails. This allows irregular graphs to be considered in the hypothesis. As of now, it remains a mystery whether this zeta function have a special meaning.

### Quantum Chaos
The study of Odlyzko has shown that the normalized spacings of the non-trivial Riemann Zeta zeros is close to a GUE emsemble. 
Friedman proved that a random regular graph is almost Ramanujan. After that, Miller showed that the proportion of regular graphs exactly satisfying the RH approaches 0.27 as the number of vertices approaches infinity.
<p/>

<p/>
<script type="text/javascript" charset="utf-8" src=" https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML, https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
