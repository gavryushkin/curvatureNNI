Dear Editor,

First of all, we wish to thank you and the anonymous reviewers for carefully reading our paper and suggesting the ways to improve the text.
We found all comments very useful and addressed them all in the revised version.
Please find below our point-by-point response.


> carefully go through their definitions to make them consistent with e.g. the terminology in the book "Phylogenetics (Semple and Steel)" which is regarded by many as the reference book for the area. I guess what the authors mean by NNI-graph is generally referred to as Treespace (under NNI-moves).
> make their arguments more concise and revise the statement of some of the results to make it clearer if they are referring to a (graph theoretical) tree or a phylogenetic tree.

We have carefully considered every definition introduced in the paper and added references to the aforementioned book, where necessary.
We have also revised our statements and arguments and clarified what terminology we are using.
In particular, we replaced the graph-theoretic concept of aunt subtree by a direct explanation.
One motivation for our paper is random walks on graphs, including those employed in MCMC tree inference methods.
Furthermore, our paper relies heavily on ideas and methods from graph theory.
Hence, we decided that it would be convenient to have both concepts (NNI graph and Treespace) and to rely on graph-theoretic terminology.
To put our terminology inline with the book, we have added the corresponding reference to our definitions where necessary, and included an explanation for our choice of terminology in the introduction (second paragraph on p. 2).

> turn footnotes in the proofs into proper definitions and move definitions outside the proof of a statement if the concept is used later on again.

We decided to avoid using footnotes altogether and carefully checked that all definitions given inside proofs are only used within those proofs.

> make the references consistent with the requirements of the journal

Done.

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

> some of the proofs belong to an Appendix.

We have removed the Appendix and put all proofs directly in the appropriate places of the text.

> I suggest the authors to use more intuitive descriptions and formalise their proofs as much as possible.

We have done this as much as possible -- see our first comment.

> Page 2, Section 2 :  It is not clear what you mean with the phrase:  "We identify isomorphic trees."

We clarified.

> Please state what does DtT stand for.

Done.

> Page 3: It would be nice if the example in Fig. 2 shows all the three operations, that is also the swapping of the rank of two nodes.

Done.

> Page 4: The paragraph starting with "This hierarchy can be seen as a set of … " is not clear. Please give at least some intuition on what is a \tau-space.

Done.

> Page 5: define what convex means in the set of trees you are considering.

Done.

> Page 6 inside the proof of Lemma 4: "… no divergence event being younger than a taxon."Not clear what this means, this should hold for every phylogenetic tree.

We clarified this. Sometimes sampling evens happen earlier than some divergence events in another linage. Our concept of discrete time-trees allows this. See Figure 1 for an example of such tree: taxon F was sampled before taxa C and D diverged.

> Page 6 inside the proof of Lemma 4: what is the aunt of a subtree?

Done. We removed this and added a direct explanation.

> Page 6 last paragraph:  "The best known bound for NNI … ". You mean upper bound.

Yes, fixed.

> Page 7 second paragraph inside the proof of Theorem 5: what are half-edges? Do you mean the middle point of an edge?

We have added a detailed explanation.

> Page 12: what are sampled ancestor trees?

We have added the definition.

Best wishes,
Alex

