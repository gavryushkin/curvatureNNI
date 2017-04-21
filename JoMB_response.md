Dear Editor,

First of all, we wish to thank you and the anonymous reviewers for carefully reading our paper and suggesting the ways to improve the text.
We found all comments very useful and addressed them all in the revised version.
Please find below our point-by-point response, accompanied by the diff that highlights all the changes we've made.


> carefully go through their definitions to make them consistent with e.g. the terminology in the book "Phylogenetics (Semple and Steel)" which is regarded by many as the reference book for the area. I guess what the authors mean by NNI-graph is generally referred to as Treespace (under NNI-moves).
> make their arguments more concise and revise the statement of some of the results to make it clearer if they are referring to a (graph theoretical) tree or a phylogenetic tree.

We have carefully considered every definition introduced in the paper and added references to the aforementioned book, where necessary.
We have also revised our statements and arguments and clarified what terminology we are using.
In particular, we replaced the graph-theoretic concept of aunt subtree by a direct explanation.
One motivation for our paper is random walks on graphs, including those employed in MCMC tree inference methods.
Furthermore, our paper relies heavily on ideas and methods from graph theory.
Hence, we decided that it would be convenient to have both concepts (NNI graph and Treespace) and to rely on the graph-theoretic terminology.
To put our terminology inline with the book, we have added the corresponding reference to our definitions where necessary, and included an explanation for our choice of terminology in the introduction (second paragraph on p. 2).

> turn footnotes in the proofs into proper definitions and move definitions outside the proof of a statement if the concept is used later on again.

We decided to avoid using footnotes altogether and carefully checked that all definitions given inside proofs are only used within those proofs.

> make the references consistent with the requirements of the journal

We have changed the citation style according to the requirements of the journal.

> given that the authors are interested in diameter bounds, they might also find the following paper interesting

The paper is indeed relevant to our results and we added a reference.


Reviewer #1:
The manuscript is well prepared, but not in the format of the JMB. It is recommended to be accepted with minor revision.

> We have fixed the formatting of references according to the journal's guidelines.


Reviewer #2:

> The paper is far from being self-contained. There are many concepts that are used without any explanation making the paper not easy to follow. The proofs are sometimes sketched like the proof of Theorem 5 which relays in many known results that are not clearly mentioned.

The paper is indeed not self-contained and relies heavily on existing literature.
In particular, Theorem 5 employs the results of Sleator-Tarjan-Thurston on graph-grammars.
We have carefully gone through our arguments, including the proof of Theorem 5, and added more intuitive explanations with exact references to the appropriate places of the cited literature (sections, statement number, etc.)
For example, we have added the outline of the proof for Lemma 4, more intuitive explanations in the proof of Theorem 5, as well as the formulation of the main result from the Sleator-Tarjan-Thurson paper, adapted to our case of trees, and the definition of tanglegrams for Proposition 8.

> some of the proofs belong to an Appendix.

We have removed the Appendix and put all proofs directly in the appropriate places of the text.

> I suggest the authors to use more intuitive descriptions and formalise their proofs as much as possible.

We have done this as much as possible -- see our first comment and the attached .pdf with diff.

> Page 2, Section 2 :  It is not clear what you mean with the phrase:  "We identify isomorphic trees."

We clarified this sentence, which now reads: "We do not distinguish between isomorphic trees, i.e. we identify them."

> Please state what does DtT stand for.

We have added: "..., where DtT stands for “discrete time-trees”."

> Page 3: It would be nice if the example in Fig. 2 shows all the three operations, that is also the swapping of the rank of two nodes.

We have added all possible operation to Fig. 2.

> Page 4: The paragraph starting with "This hierarchy can be seen as a set of … " is not clear. Please give at least some intuition on what is a \tau-space.

We have added: "... if we allow the lengths of event intervals to take every possible non-negative real value and impose the Euclidean metric on trees with the same ranked topology, then we get the $\tau$-space introduced by \textcite{Gavryushkin2014-bw}. In this case, $\dtt_1$ is the graph with the vertices being the orthants of $\tau$-space and the adjacency relation being the relation of “have a shared facet of co-dimension $1$“. Similarly $\dtt_0$ is the adjacency graph on the orthants of BHV space \autocite{Billera2001-rj}."

> Page 5: define what convex means in the set of trees you are considering.

We have added the definition.

> Page 6 inside the proof of Lemma 4: "… no divergence event being younger than a taxon."Not clear what this means, this should hold for every phylogenetic tree.

Sometimes sampling events happen earlier than some divergence events in another linage. Our concept of discrete time-trees allows this. See Figure 1 for an example of such tree: taxon F was sampled before taxa C and D diverged. We clarified the paragraph to read:

"The upper bound is attained by a caterpillar tree with all intervals short, every taxon being younger than every divergence event, and both taxa in the cherry being younger than at least one other taxon, that is, a caterpillar tree with internal nodes having ranks $n, \ldots, 2(n-1)$ and the ranks of the taxa in the cherry $< n-1$."

> Page 6 inside the proof of Lemma 4: what is the aunt of a subtree?

We removed this and added a direct explanation.

> Page 6 last paragraph:  "The best known bound for NNI … ". You mean upper bound.

Yes, fixed.

> Page 7 second paragraph inside the proof of Theorem 5: what are half-edges? Do you mean the middle point of an edge?

We have added a detailed explanation: "Here, for every edge in the tree we distinguish between its two ends and refer to them as half-edges---this is necessary to be able to substitute one subgraph by another in a unique way by connecting corresponding half-edges---as in \autocite{Sleator1992-bp}."

> Page 12: what are sampled ancestor trees?

We have added the definition.

Best wishes,
Alex

