[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12413560&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do \emph{not} have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.



## Answer
$G_1=(V_1 , E_1)$
$G_2=(V_2 , E_2)$

Suppose that $f: V_1 \rightarrow V_2$ is bijection

Because every bijection possesses properties ${(u,v)} \in E_1 \iff {f(u),f(v)} \in E_2$ 

Suppose $G_1$ has many edges between V1 and E1. Then $G_2$ should also have multiple edges between f(u) and f(v). But $G_2$ is generic and without many edges. It is a contradiction with bijection.

Additionally,  if we assume that  $G_1$ has n vertices, then $G_2$ should also possess n vertices. But, $G_2$ is plain and has n-5 vertices (where n > 10). Indeed, this leads to a contradiction.

Regarding the loop, if $G_1$ features a loop at vertex v, it follows that $G_2$ must also have a loop at f(v). If $G_2" lacks any loops, it results in a contradiction.

Given that $G_1$ and $G_2 share the same properties as discussed above, a bijection exists between them, leading to $G_1 = (V_1 , E_1)$ being isomorphic to $G_2 = (V_2, E_2).
