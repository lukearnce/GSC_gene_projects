Aim_2\_outline
================

# Aim 2: Generate a GSC gene ortholog dataset and merge with existing relevant datasets

**Rationale:** DSD is known to occur in two GSC genes (bam and Yb), but
the frequency of DSD and where it tends to occur in GSC genes is
unknown. I can begin to interrogate these topics by identifying absences
of GSC genes essential in D. melanogaster. The GSC gene ortholog dataset
will be able identify orthologs and absent GSC genes across the 39
Drosophila species, spanning the evolutionary scope of the genus and two
closely related outgroup species. This will enable us to make informed
predictions regarding the evolutionary history of many GSC genes as well
as evaluate the extent and characteristics of GSC gene network
flexibility.

**A:** Ortholog dataset construction and validation

**Null hypothesis:** Orthologs of D. melanogaster GSC genes are almost
all present across the genus Drosophila and into included outgroup
species

**Methodology:** I have assessed predicted orthology for GSC genes in 10
Drosophila species spanning across the phylogeny and two closely related
outgroup species using Ensembl compara (27). This tool catalogs relevant
information about each ortholog including sequence alignment, target
percent ID (percentage of orthologous sequence matching the Drosophila
melanogaster sequence), query percent ID (percentage of Drosophila
melanogaster sequence matching the orthologous sequence), gene order
conservation score (evaluating synteny), and high or low ortholog
confidence (calculated using results from other categories)(27). To
further refine ortholog predictions from Ensembl, coding DNA sequence
(CDS) data for all Ensembl species and an additional 29 Drosophila
species will be downloaded from NCBI. I will use the CDS from the most
recent D. melanogaster Flybase release to find orthologs among non-D.
melanogaster species. The CDS of the longest protein sequence will be
chosen for each gene. In more distant species, the CDS from a closely
related species with the ortholog present will be used to identify
orthologs in addition to D. melanogaster CDS. Predicted orthologs will
be further validated via reciprocal BLAST (Basic Local Alignment Search
Tool)-hit approach of the program INPARANOID (28). Tested predicted
orthologs will be divided into orthologs, paralogs, and non-orthologs
based on bootstrap values from INPARANOID analysis and synteny. I will
realign the ortholog dataset using the phylogeny aware realignment
software PRANK. After the alignment, sequences containing large regions
of gaps will be removed using maxAlign.

I will then confirm GSC gene ortholog absences via PCR by considering
sequence alignments of the species with the ortholog absent and the
closest related species with the gene present, designing four primers
based on the sequence with the gene present, two flanking the gene and
two within the gene body. The genomic DNA of both species will be used
as templates and the different primer combinations will be used for PCR
reactions. Resulting products will then be visualized using gel
electrophoresis and products will be Sanger sequenced. I will use the
PCR amplifications of the present gene as positive controls.

**Expected outcomes and interpretations:** If gel electrophoresis bands
are the expected size and Sanger sequencing results reveal there is no
significant sequence between the two primers flanking the predicted
absence, these results are consistent with ortholog absence. If I see an
unexpected large band and sequencing results showing an unexpected
region between the flanking primers, these results are consistent with
the ortholog not being absent as predicted. The confirmed absences will
enable us to further define the extent of observed functional
flexibility at the phylogeny, species group, lineage and gene levels. If
I find that all GSC genes excluding Yb are present across all included
species, failing to reject the null hypothesis, I would conclude that
GSC regulating genes are highly conserved, at least at the gene level,
and that Yb is an outlier. If I find that some GSC regulating genes are
absent in some included lineages, rejecting the null hypothesis, that
confirms that there is some degree of developmental systems drift
occurring in GSC genes. I can similarly evaluate lineages and genes for
differences in GSC gene functional flexibility. These results will
provide a direct test of the assumption that orthologs are generally
functionally conserved in GSC regulating genes.

Patterning of ortholog presence or absence across species will also help
create reasonable hypotheses about evolutionary history of GSC genes.
For example, a gene may have orthologs in species throughout Drosophila
and included outgroup species, which could indicate the gene was present
in a common ancestor to all included species. If a gene has orthologs
throughout the genus Drosophila, but not in any outgroup species, the
gene may have been new to the common ancestor of the Drosophila genus.
If a gene only has orthologs in a subgroup of species or a single
species, the gene may have developed in the common ancestor of the
species subgroup or even more recently, in the specific species lineage.
Similarly, if a gene is absent across a species subgroup, but present
elsewhere in the genus, the gene may have been present in the common
ancestor of the genus, but subsequently lost in later common ancestors
of particular species subgroups.

I have generated a GSC gene ortholog dataset including 10 Drosophila
species spanning across the phylogeny and two closely related outgroup
species with predicted presence and absence of the 366 GSC regulating
genes using Ensembl compara, a multi-species database that stores the
results of genome-wide species comparisons (18,19,22,23). Ensembl
compara generates ortholog predictions based on a combination of factors
including percentage of shared sequence identity and gene order
conservation (69). I can make preliminary assessments regarding the
extent and characteristics of GSC gene network functional flexibility by
using predictions from the GSC gene ortholog dataset. For example, in D.
simulans, a lineage particularly closely related to D. melanogaster,
predictions show over 7% of GSC genes found to be essential in D.
melanogaster are without an ortholog in D. simulans. This suggests that
some GSC regulating genes are gaining or losing essential roles on a
rapid evolutionary timescale, quickly following speciation and/or as
intraspecies gene loss or gain. Predicted absences of GSC regulating
genes generally increases with more divergence time from D.
melanogaster, peaking at 33% (D. willistoni) within Drosophila and 61%
(L. cuprina) when considering outgroups (Fig. 2). If the predictions are
true, this represents an unexpected degree of functional flexibility at
GSC genes.

The trend of the number of predicted absences increasing with divergence
time from D. melanogaster is not completely linear. D. Willistoni (57 MY
divergence time) has a higher degree of predicted gene absences than D.
mojavensis, D. virilis, and D. grimshawi (67 MY divergence time). This
could be due to stochastic forces or perhaps lineage specific pressures.
Though predicted GSC gene absences generally increase with divergence
time from D. melanogaster, the rate of the percentage of absences to
divergence time shows a different relationship. Rates are highest in the
species most closely related to D. melanogaster (4-7 MY of divergence)
and the rates are significantly lower in more divergent species. This
suggests that DSD could occur at a faster rate in closely related
species. These are predictions that will require downstream validation,
but these are some examples of the utility of generating this data.

**Caveats and future directions:** Assessing functional divergence by
gene absence is not an exhaustive analysis of functional divergence.
Present genes, like bam, can still be involved in developmental systems
drift. Gene absence identifies the baseline of functional divergence at
GSC genes. Also, while the relationship of orthologs across species can
help lay out hypothetical evolutionary histories, parsimonious
explanations can be incorrect. Parsimony may suggest that if a gene is
lost in a specific lineage while related species in the same subgroup
all still have the gene, the gene was present in the common ancestor to
the subgroup and lost in the one lineage missing the gene. It could also
be the case that the gene was independently gained by the other species
in the subgroup and the common ancestor did not have the gene. Future
directions could include functional analysis of select GSC genes to
better define specific GSC gene functional evolutionary histories.

**B:** Integration of existing relevant datasets

**Null hypothesis:** Datasets will reveal no common characteristics
functionally flexible GSC genes Methodology: Physical interactors,
genetic interactors, and GO annotated molecular function will be
incorporated from Flybase datasets using Python (25). GSC gene
functional categories, identified by complex-enrichment analysis of the
366 GSC genes, and defect type, defined by the observed phenotypic
effect of RNAi knockdown will be incorporated from Yan et. al (2014). I
can use these datasets in conjunction with the GSC gene ortholog dataset
to parse observed GSC gene and gene interaction network functional
flexibility.

**Expected outcomes and interpretations:** If the datasets fail to
reject the null hypothesis, revealing no common characteristics of
functionally flexible genes, that will provide evidence that the
characteristics incorporated may not have an impact on GSC gene
functional flexibility. If the data rejects the null hypothesis, I will
be able to determine which categories are particularly conserved or
flexible from the phylogeny to the gene level for GSC genes. For
example, results from Ensembl predictions for GSC genes involved in
Ribosome biogenesis (14 genes) show a high degree of flexibility across
species, generally increasing with divergence time while GSC genes
involved in the COP9 signalosome (7 genes) are largely conserved across
species, with only one absent gene in a single Drosophila species and
three genes absent in L. cuprina and M. domestica (Fig. 3). These
different predicted degrees of conservation across functional categories
of GSC genes could be related to the function or characteristics of the
genes involved in the function. In contrast, predictions for flexibility
across defect types show a generally consistent degree of conservation.
Physical and genetic interaction networks of GSC genes will also be
informative. For example, genes identified as genetic and physical
interactors of bam do not show predictions of complete conservation
across Drosophila species considered in Ensembl compara (69). If the
predictions are accurate, this indicates that there is at least some
degree of functional flexibility within bam’s interaction networks
across species. If an interacting gene is absent, as predicted, bam does
not have an interacting relationship at all with the absent gene in that
lineage. This does not necessarily indicate that bam itself is
functionally divergent. Interacting genes could be absent due to a new
gene (or genes) interacting with bam to carry out the same function. An
interacting gene could be lost due to bam no longer performing the same
function carried out in part by the interaction. The interacting gene
could also be absent because it is novel to a distantly related clade
and it has not been gained in the lineage I am considering. In lineages
where bam is not carrying out its essential function as the key switch
gene for differentiation (as defined in D. melanogaster), another gene
or combination of genes must be executing that function.

I will also be able to determine whether GSC gene interaction networks
show any patterns of conservation. Predicted results for bam provide a
good example. In species signaling positive selection at bam via MK test
with bam null differentiation defects in both sexes, I have found a few
functionally related genes are predicted to be absent, 2 of 38 in D.
simulans and 4 of 38 in D. yakuba (Fig. 4). If these predictions are
accurate, there is some degree of DSD occurring quickly in bam’s
interaction networks across species in which bam is essential. D.
ananassae, which shows a signal of positive selection at bam via MK test
and bam null differentiation defects in females only, has 8 of 38 bam
interaction network genes predicted to be absent. This is a higher
degree of predicted flexibility than in the species where bam nulls
confirmed bam’s essential GSC differentiation function in both sexes. D.
pseudoobscura Ensembl results predict 11 of 38 bam network genes are
absent. If the predictions are accurate, this represents a substantial
degree of flexibility in bam’s interaction network for this species.
These absences along with the MK test results detecting no selection at
bam in the lineage could indicate that bam is not performing its
essential function in GSC differentiation. If the predicted absences are
correct, bam is at least carrying out its function with fundamental
differences in its interaction network. Bam could be performing its
essential GSC differentiation function with other genes executing the
essential roles of the genes predicted to be absent or bam itself could
be in some way compensating for these absences. Direct experimental
assessment would have to be done to determine bam’s specific function.

Another way I can use the gene interaction networks to further define
characteristics of developmental systems drift is to compare a gene’s
interaction networks across species to highlight which interacting genes
seem to have particularly high levels of flexibility or conservation.
For example, considering bam’s interaction networks, zpg is weak or
absent in all considered species excluding D. melanogaster and Mir-7 is
present in all species(70). One possible explanation is that zpg has
three genetic interactors, all involved in its described GSC function,
and no physical interactors. Given its small interaction network and
apparent lack of pleiotropic functions, absence of zpg is not
significantly disruptive. Mir-7 on the other hand has eighteen physical
interactors, five genetic interactors, and is involved in a range of
pleiotropic functions including but not limited to regulation of wing
growth, development of follicle cells, development of the visual system,
and regulation of the Hippo pathway (71-75). Absence of Mir-7 would lead
to effects far beyond GSC differentiation. By considering the functional
flexibility in GSC gene interaction networks, I can further characterize
which genes seem to be more regularly subject to developmental systems
drift and develop hypotheses as to why particular genes are highly
conserved or flexible.

**Caveats and future directions:** The data incorporated from Flybase
and Yan et. al (2014) is based on analysis of D. melanogaster. If GSC
genes are found to be highly functionally flexible, the utility of using
D. melanogaster interaction networks and functional classifications to
make assessments about which specific functional aspects of the
interaction networks are flexible will be limited. I will still be able
to identify broadly where there is DSD between D. melanogaster and other
species, but specific functions of interacting genes would require
direct interrogation in divergent lineages. RNA-seq expression data for
gonads and whole adults without gonads is available for eight species
(D. melanogaster, D. yakuba, D. ananassae, D. pseudoobscura, D.
persimilis, D. willistoni, D. mojavensis, and D. virilis), and I can
incorporate expression data for GSC genes in these species to identify
potential points of functional divergence by using differences in
expression (16).
