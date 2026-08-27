====================================================================
Haplodon: uncertainty-aware haplotype-based variant effect prediction
====================================================================

Haplodon is a command line tool for haplotype-based variant interpretation. Current variant effect
prediction tools interpret variants independently, which can be incomplete or wrong when multiple
variants sit on the same haplotype: a deletion that shifts the reading frame invalidates every
downstream amino acid prediction, an adjacent insertion may restore it, and several amino
acid-changing variants can jointly affect a protein's function.

Instead of treating variants independently, haplodon models them in a graph structure that
represents haplotypes as paths and individual variants as vertices. The graph integrates read
evidence of variant co-occurrence derived from the probabilistic information provided by the
uncertainty-aware variant caller `varlociraptor <https://varlociraptor.github.io>`_. For each
inferred haplotype, haplodon reconstructs the corresponding protein sequences for a user-given set
of transcripts and scores them based on their physicochemical divergence from the reference. The
output incorporates per-variant annotations retrieved via GeneBe (e.g. population frequency and
pathogenicity scores) and aggregates them at the haplotype level.

.. toctree::
    installation
    usage
