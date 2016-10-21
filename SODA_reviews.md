## REVIEW 1


### OVERALL EVALUATION

The authors investigate mathematical properties of graphs that span the space of time trees.
Such time trees are used in practice to estimate divergence times in phylogenetic trees and represent a large portion of present-day phylogenetic analyses.
In phylogenetics in general as well as in divergence time estimation in particular I agree with the authors that our understanding of the properties of the tree space is still relatively limited, hence, the present study indeed represents a step forward and thus the paper should be accepted.

One issue that should be discussed in more detail is weather it is worthwhile conducting actual tree searches for divergence time estimation or if the classic approach to first infer a standard phylogeny, fix it and then date it is equally good.

Irrespective of this, I do believe that the work presented here, albeit profoundly theoretical, can potentially have a plethora of practical applications as described by the authors.
For these ideas to spread however, I am absolutely convinced that authors should develop an implementation of their algorithms and offer it as a library for developers of divergence time estimation tools.

The proofs appear to be correct to me, albeit I was not able to check all of them exhaustively.

### Detailed comments:

page 1: It is not clear what the sentence "Classically these are applied without reference to branch Lengths" means.
Most implementations of classic phylogenetic inference MCMC tree topology moves, do indeed try to also propose new branch length configurations at the same time.
Note that, discretized time trees were also proposed in the following paper: http://bmcevolbiol.biomedcentral.com/articles/10.1186/1471-2148-8-77

page 3 Example 2: The authors need to explain the Newick format, since this does not represent general knowledge at SODA and also need to explain other common phylogenetic terminology such as what a "cherry" is and also properly introduce their split/bipartition notation (e.g., 1456|7).

page 4:
lemma 3: the authors should include at least one example for how the rest follows from the NNI case.
the meaning of deg(T) should be properly defined.
lemma 4: I think that the explanation as to why the caterpillar tree indeed is the upper bound needs to be presented in a more formal way.
The term "aunt" has not been defined.

page 5: the term "coalescence" needs to be properly introduced somewhere, before using it because it may be unfamiliar to the SODA audience.

page 6: In the sentence before corollary 6, the equation should read: a^{f(n)+2r} and not a^{f(n)+2a}

page 7: two last sentences: the algorithm might also be useful to determine if two trees appear to be separated by a valley (e.g. of posterior probability) or if they are rather located on a plateau.

page 9: conjecture 9: is the term "presents" a standard term? I have never seen that used before.


## REVIEW 2

The authors study discrete time trees which are approximations of phylogenetic time trees.
The paper introduces a hierarchy of graphs on such trees.
The vertex set  of level-m graph DtTm consists of all discrete time trees that has intervals of length no more than m.
The vertices of two discrete time trees in DtTm are connected by an edge if the corresponding time trees can be obtained from each other by one of three operations.
The bottom layer DtT0 forms the well-known phylogenetic graph NNI and is a rough approximation of the space of discrete time trees.

The paper exhibits several basic properties of the graphs in the presented hierarchy such as (i) their diameter, and (ii) the size of neighbouhoods.
The paper leaves unanswered the question of whether the distance between two discrete time trees can be computed efficiently or not.

In my opinion this paper can not be accepted at SODA for several reasons.
It is not clear to me how important the discovery of the basic properties shown in this paper are for the study of time tree graphs.
It is also not clear to me how important time tree graphs are in general.
Further, I don't see how the basic properties discussed in this paper are for the resolution of Problem 1.
I finally feel that this paper is more suitable for a more specialized venue in computational biology than it is for SODA.


## REVIEW 3

A phylogenetic tree is a tree whose nodes are strings, in which adjacent strings differ by simple "mutations."
They are supposed to represent plausible explanations about how a population of different species (the leaves) could have evolved from a single common ancestor species (the root).
Some such trees are more plausible than others; on the other hand, there are a great many such trees, and the most plausible one may not be the most true.
For this reason, we would like a better understanding of the distribution over the whole space of trees in this model.
In recent years there has been a flurry of interest in the TCS community in trying to provide better and more rigorous algorithms for this.

This paper concerns itself with a variant of phylogenetic trees called "time trees," in which the nodes are additionally tagged with numerical time data.
Such a tree, if correct, indicates not only the sequence of speciation events, but also how much time elapsed between them.
Since we know something about the frequency of different kinds of mutations, this gives us another axis on which to judge the plausibility of such a hypothesis.
However, because of this change, the number of time trees for a given set of leaves is infinite, unlike the number of phylogeny trees, which is huge but still finite.

This paper proposes some discretization methods for getting around this problem, and provides some basic analysis of them, including:
- upper bounds on the volumes of balls of radius r in the state space for 4 models (Thm 5)
- upper and lower bounds on the diameters of the state space for one model (Thm 7)
- a more technical lemma about how many neighbors of a given state x are closer to x than to another state y, for 3 of the models.
(Thm 10)  This theorem is proved modulo a conjecture (Conj 9) which is a sort of convexity result: along all shortest paths in the state space, a certain property of the endpoints will be preserved.

I don't think this paper meets the bar for interest and originality for the SODA conference.
The techniques used in the proofs seem to be well-established and not surprising in the present context.
On the plus side, the paper introduces several new models, some of which may be of interest to people interested in the area, as well as presenting some conjectures and open problems, and motivation for why the subject is interesting to biologists and computer scientists.
The paper seems clearly written, and at a level that is welcoming to non-specialists.

