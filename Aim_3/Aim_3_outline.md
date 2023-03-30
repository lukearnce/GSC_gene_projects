Aim_3\_outline
================

# Aim 3: Analysis of selection

**Rationale:** Gene absence confirms that there is a functional
diversification at the gene across orthologs, considering all included
genes are essential in D. melanogaster, but gene presence alone does not
provide useful insight regarding functional flexibility. To enable more
useful evaluation of present genes, I will use the MK test and dN/dS
based divergence analysis to detect signals of positive selection. There
are lineage-specific MK test results for bam in 18 Drosophila species,
all of which are included in our ortholog dataset (67). Results have
shown heterogeneous signals of selection at bam across the Drosophila
phylogeny. There are several possible drivers of positive selection.
Some could result in functional divergence while others may not.
Positive selection could be driven by a change in function, refinement
of a function, life history or environmental factors, conflicts with
TEs, endosymbionts, or viruses. Germline conflicts may or may not lead
to functional changes at bam. For example, germline agents such as W.
pipientis may be in conflict with bam for control of oogenesis leading
to rapid evolution at bam to evade control (15). This could result in
bam adaptively evolving while maintaining the same essential function.
Germline conflicts might also drive the fixation of novel genes in new
roles to evade control. In this case, a different gene or genes could be
performing bam’s essential differentiation function, potentially
relaxing constraint at bam and allowing bam to lose its now redundant
function and/or gain or functionally refine a different function,
driving positive selection. There are no reported orthologs of bam in
non-Drosophila species (69), which is consistent with bam being novel to
the genus Drosophila.

For the species with bam nulls that show differentiation defects in both
sexes and only differentiation defects in females, all show signals of
strong positive selection via MK test. Considering bam appears to be a
gene novel to the Drosophila genus, this is consistent with positive
selection being driven by functional diversification or refinement of
function. Positive selection for refinement of function in particular is
common in novel genes, but selection at bam could also be driven by
germline conflicts. Selection at bam will only be driven by Wolbachia if
bam retains its essential role, otherwise control of bam by Wolbachia
would not give Wolbachia more control of reproduction. In D. teissieri,
bam nulls showed no differentiation defects and no signal of positive
selection was detected. This could indicate that bam never gained its
essential function in this lineage or that bam lost its essential
function in this lineage. Germline conflict with Wolbachia is unlikely
in this lineage, given bam is not essential for GSC differentiation.
Functional refinement or change in function for bam’s essential role in
GSC differentiation also is not occurring. Even with a lack of selection
detected, there could still be a relaxation of constraint at bam which
could indicate recent functional redundancy. The combination of bam MK
test along with lack of selection detected at bam using the PAML site
test across 12 D. melanogaster group species highlights that the
positive selection at bam is likely due to lineage specific pressures.
MKT results are available for bam in D. pseudoobscura, but not yet for
D. americana. Fortunately, polymorphism data for D. americana and a few
other Drosophila species have recently been made available.

Polymorphism data is not available for most species I am considering in
the ortholog dataset. Still, identifying signals selection in these
lineages would provide further useful context for understanding the
flexibility of bam and other GSC regulating genes. I will use dN/dS
based divergence analysis to test bam for signals of positive selection
in species without polymorphism data as well as testing the other 365
GSC regulating genes for selection across the phylogeny. Previous
analysis within six D. melanogaster group species (D. melanogaster, D.
simulans, D. sechelia, D. yakuba, D. erecta, and D. ananassae)tested GSC
genes for signals of positive selection using PAML analysis (33). 76 GSC
genes showed signals of positive selection. PAML analysis was not
conducted beyond D. ananassae due to prohibitive synonymous site
saturation preventing incorporation of more distant Drosophila species
(25,33,34). Specific GSC genes including stwl, ote, and more extensively
Sxl have been tested for selection in Drosophila species outside of the
D. melanogaster group (35). Analysis of Sxl in D. pseudoobscura and many
species within the D. melanogaster group shows that selective constraint
plays a significant role in the molecular evolution of Sxl within
Drosophila, but patterns were also observed suggesting both recent
positive selection and episodic bursts of protein evolution at Sxl (36).
Now, with additional high quality sequences, I can extend PAML
divergence analysis of GSC genes to species beyond the D. melanogaster
group.

**A:** McDonald-Kreitman test at bam in select Drosophila species

**Null hypothesis:** No signals of positive selection will be detected
via MK test in newly tested species

**Methodology:** I will use polymorphism data for D. americana, D.
kikkawai, D. ironensis, and D. setifemur to test for departures from
selective neutrality consistent with positive selection at bam using the
McDonald Kreitman test. The null hypothesis of the MKT is that the ratio
of nonsynonymous to synonymous polymorphism within a species is equal to
the ratio of nonsynonymous to synonymous divergence between species.
Since bam is highly divergent across the Drosophila genus and appears to
be experiencing episodic signals of adaptive evolution, I will measure
lineage-specific divergence.

I will do this by using the codeml package from PAML to generate the
predicted common ancestor sequence and align that sequence to the
species of interest using PRANK. I will use the MK test webtool at
<http://mkt.uab.cat/mkt/mkt.asp> to complete the MK test. Polymorphic
sites at \<15% frequency will be excluded, since these are likely
slightly deleterious alleles that have not yet been purged by purifying
selection (76). Resultant values for the contingency table, Chi-Square
test, and alpha, the proportion of fixations predicted to be due to
positive selection, will be reported. Expected outcomes and
interpretations: If MK test results for D. americana bam indicate
positive selection and the null results demonstrate bam is essential for
GSC differentiation, this provides evidence to support that functional
refinement for bam’s essential function in GSC differentiation in D.
americana or gametogenic conflict as potential drivers of positive
selection at bam. This does not rule out other potential drivers of
positive selection. If MK test results for D. americana bam indicate
positive selection and null results demonstrate bam is not essential for
GSC differentiation, this is consistent with positive selection being
driven by functional refinement for a function unrelated to GSC
differentiation like bam’s role in hematopoietic progenitor maintenance
during hematopoiesis (58). Caveats and future directions: If the MK test
does not detect positive selection at a gene, that does not necessarily
mean positive selection is not taking place. Using the MK test, when
possible, to evaluate other GSC genes for signals of positive selection
could also highlight potential functional divergences.

**B:** Divergence analysis using PAML

**Null hypothesis:** PAML analysis reveals positive selection is
detected at the same GSC genes and sites across species

**Methodology:** To identify positive selection, I will estimate dN/dS
in all 1-to-1 orthologous GSC regulating genes using the branch-sites
model from PAML, since this model enables more effective detection of
heterogeneous signals of selection than the site model (25, 33,37,38).
The branch-site model of PAML requires an a priori phylogenetic tree to
test for positive selection in foreground branches. The species
designated as the foreground branch will be the branch evaluated for
positive selection, and the background branches included in analysis
will be those closely related on the species tree (ideally two or more)
(34, 38). I may run into the issue of synonymous site saturation for
particularly divergent single lineages. I will restrict analysis to
groups of lineages that are not saturated, which may result in the
exclusion of single long lineages like D. willistoni.

I will compare the likelihood of two different models for each
orthologous gene: 1. the alternative model that allows for a proportion
of the sites to be under positive selection along the foreground branch
(ω2 ≥ 1), and the background branches having a proportion of sites being
under purifying selection (ω1 \< 1) or neutrally evolving (ω0 = 1); and
2. the simplistic null model that has the ω2 fixed at 1 on the
foreground branches, and all other branches having ω0 = 1 and ω1\<1. I
will obtain likelihood values after running each transcript under two
different models and carrying out likelihood ratio tests between the
models to evaluate whether the alternative model outperforms the null
model. I will perform a Bonferroni correction to account for multiple
comparisons. A significant result from the branch-site model is
indicative that a subset of the sites in the coding gene signal positive
selection, with the selected sites providing an advantage to the
foreground lineage (39). Expected outcomes and interpretations: If I
fail to reject the null hypothesis, this suggests selection acts
similarly on GSC genes across the phylogeny. If the null hypothesis is
rejected, this suggests selection can act differently on GSC genes
across species. Differences in signals of selection will highlight
potential points and patterns of functional flexibility in GSC
regulating genes. This data in conjunction with the information from the
ortholog dataset will give us the ability to evaluate if there are
particular functional categories of GSC regulating genes that are
particularly common or uncommon targets of positive selection. Results
will also help us identify possible patterns of selection in
functionally related genes when an interacting gene is lost or gained.
Perhaps when genes are lost in a lineage bursts of positive selection in
functionally related genes are observed. This could indicate that
functionally related genes may be evolving adaptively to execute the
function of the gene that is now absent. Genes that are functionally
related to the lost gene could also not show signals of positive
selection. If this is the case, perhaps the gene lost had not acquired
its essential function in this lineage or it may have been made
functionally redundant by another gene using the same functional
network. I may also see patterns in functionally related genes when a
gene is gained. Genes that appear to be gained in D. melanogaster and
signal positive selection could indicate refinement of essential
function. Interpretation of selection results will be largely context
dependent, but results will provide another useful dimension when
considering GSC gene functional flexibility.

**Caveats and future directions:** The selection analysis will be less
concrete in highlighting functional flexibility than using presence and
absence of genes or generating nulls since function is not directly
evaluated. Also, even if selection is detected identically across
included species, I can not automatically assume that the genes are not
functionally divergent. Using the site model in PAML in addition to the
branch site model could help highlight whether I see consistent
selection at the same site across species, and incorporating comparisons
of evolutionary rates across the phylogeny for GSC genes could highlight
rate differences between species that may not have signals of positive
selection. This could indicate a relaxation of constraint in the
lineage, which could be consistent with the gene no longer being
essential in the lineage.
