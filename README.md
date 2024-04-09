[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

Answer: If $f(n)\in o(g(n))$, then $\forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$.
        So for any positive constant chosen, there must be an $n_0 \forall n\ge n_0$ such that f(n) < c g(n).
        If this is the case for f(n), then the case must be true that 
        $\exists c>0, \exists n_0, \forall n\ge n_0: f(n) <= c g(n)$. 
        If there is an $n_0 \forall n\ge n_0$ for all positive constants such that $f(n) < c g(n)$,
        then there is obviously at least one constant and $n_0$ that exists that also proves this to be true. 
        So $f(n)\in O(g(n))$ if $f(n)\in o(g(n))$ based on the definition of $O(n)$.
        Additionally, the bounds are looser in $O(n)$ than $o(n)$ because f(n) has to be less than or equal to c g(n) rather than strictly being less than c g(n). 
