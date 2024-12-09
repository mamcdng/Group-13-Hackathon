# Group-13-Hackathon
# Angelman Syndrome Report

### Angelman Syndrome Phenotype
  Angelman syndrome is a rare neurodevelopmental disorder that is typically diagnosed by the age of 2 years in children due to the developmental delays evident beginning around 6 months of age. Typical clinical symptoms include severe speech impairment (little to no use of words), ataxia, behavioral abnormalities, seizures, sleep disturbances, feeding difficulties, microcephaly, characteristic facial features such as a wide mouth, widely-spaced teeth, and a prominent chin, and hypopigmentation of the skin and hair. The prognosis for individuals with Angelman syndrome varies by severity of the developmental delays present, but there is no known cure yet. The life expectancy for those with the syndrome is just below normal on average. People with Angelman syndrome are most often able to learn to walk, but with a wobbly gait. There is not often improvement in the sleep disturbances, speech troubles, or developmental delays, and individuals with Angelman syndrome often need close support for life. The only known treatment is symptomatic treatment that addresses the mobility and feeding challenges, seizures, communication difficulties, and sleep disturbances. 

### Associated Genes
**UBE3A - Primary Gene**
  This gene codes for the protein ubiquitin ligase E3A, an enzyme that is part of the ubiquitin-proteasome system that tags proteins for degradation. It is very active in the hippocampus, cortex, and cerebellum (regions of the brain necessary for learning, memory, and coordination). It is highly expressed during brain development. Only the maternally-inherited allele is expressed in the neurons, and the paternal allele is epigenetically silenced. Maternal deletions are most often present in AS, but mutations, paternal uniparental disomy, and imprinting defects can also cause UBE3A disfunction. 

**GABAA Receptor Subunit Genes: GABRB3, GABRG3, GABRA5**
  These genes are involved in inhibitory neurotransmission and are often deleted in individuals with Angelman syndrome. They are also highly expressed in the cerebral cortex, hippocampus, and cerebellum, and it is theorized that they may contribute to the severity of neurodevelopmental symptoms experienced by AS patients. 

**SNRPN**
  This gene codes for a protein called small nuclear ribonucleoprotein polypeptide N. It is involved in RNA processing. Although it is not directly responsible for the development of AS, the SNURF-SNRPN locus it is a part of may be involved in imprinting and regulation of the expression of UBE3A.

**Nearby Genes to UBE3A: MKRN3, NDN, MAGEL2**
  These genes do not have direct effects on AS itself, but since they are located close to UBE3A on Chr 15, one or more of them may also be deleted in the case of a UBE3A deletion. This could contribute to some of the phenotypic variability seen between individuals with Angelman syndrome.

**ATP10A** 
  This gene is also located near UBE3A on Chr 15 and is commonly deleted in patients with AS. It is maternally expressed and commonly expressed in the adrenal glands and lungs. The protein it encodes functions to assist in transport of phospholipids (including phosphatidylserine, necessary for nervous system function) across the cell membrane. Deletion of ATP10A is common in AS patients.


### Protein-Protein Interaction Network Creation
  In order to determine potential connections between associated genes and proteins in relation to Angelman Syndrome, a PPI network was created. First, the aforementioned associated genes were searched in the EBI IntAct database. Results were filtered to only include human protein:protein interactions, and the MI score was narrowed to > 0.5 to provide more certainty. A table was downloaded from IntAct that included a list of seed proteins (known gene protein products) and target proteins that could then be uploaded to Cytoscape, functionally analyzed, and formed into a visual network. The network is attached in the repository under the file name /angelman-syndrome.cys.

High-confidence interactions include:
TP53 (0.95): Known to regulate neuronal apoptosis and DNA repair.
CTNNB1 (0.92): Plays a role in synaptic signaling and neuronal development.
RAD23A (0.85): Involved in protein ubiquitination and degradation pathways.

Key Interactions:
UBE3A interacts with 30 proteins, including high-confidence interactions with:
9606.ENSP00000262455 (highest score: 582).
9606.ENSP00000489407 (score: 322).
9606.ENSP00000257770 (score: 331).
These interactions highlight proteins likely involved in UBE3A's role in synaptic signaling and neuronal development.

### Tissue-Specific eQTLs
  In order to further understand the relationships between the phenotype of Angelman syndrome and the complex genotypic possibilities in relation to the syndrome, multiple tissue-specific expression quantitative trait loci were pulled out from the GTEX portal. 
![Table displaying eQTLs for Angelman syndrome, particularly of UBE3A, from the GTEX portal. Column labels include Gencode ID, Gene Symbol, Variant ID, SNP ID, P-Value, NES, and Tissue](https://github.com/user-attachments/assets/1852678d-246d-49fa-affe-aea62216baa8)

### Hypothesis and Proposed Experiment
**Hypothesis:** UBE3A deficiency leads to accumulation of toxic proteins, altering neuronal function.
The inability to degrade misfolded or damaged proteins results in toxic buildup within neurons, causing cellular stress, synaptic dysfunction, and neurodevelopmental deficits. The connection with other proteins may have to do with the fact that ubiquitin protein ligase ubiquitinates and degrades other proteins (mostly synaptic proteins in the brain). 

**Experiment:** Introduce the loss-of-function mutation of UBE3A into a population of mice and determine if they develop similar cognitive symptoms to humans with Angelman Syndrome. Then perform autopsies on them to determine if they have excess toxins in their brain tissue in comparison to a group of control mice that have functional UBE3A genes. 
