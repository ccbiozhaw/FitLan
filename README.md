This is the GitHub Repository for the publication: "Enriching productive mutational paths accelerates enzyme evolution"

To characterize the fitness landscape surrounding the HG3.R5 and HG3.17 variants, we investigated whether their respective mutations could complement each other. We constructed two combined variants, called HG3.R5w17 and HG3.17wR5, by incorporating all additional mutations found in the other improved Kemp eliminase (w17 and wR5, respectively) into HG3.R5 and HG3.17. Surprisingly, both combined enzymes retained Kemp elimination activity, although they exhibited substantially reduced kcat values. Intrigued by these results, we shuffled the HG3.R5 and HG3.17 genes in varying ratios.
Subsequent analysis of active variants found in the shuffled libraries, complemented with data for variants from the HG3.R5 and HG3.17 evolution trajectories, resulted in 208 unique sequence-function datapoints. The underlying fitness landscape defined by these datapoints was elucidated by a principal component analysis of each variant’s embedding vector, which was derived from the evolutionary scale modeling (ESM) algorithm. This analysis revealed a deep valley between the fitness peaks representing the most improved variants, HG3.R5 and HG3.17, with no discernible ridge connecting the sequences. Overall, this empirically deduced fitness landscape indicates that the optimized variants, which are 29 mutations apart, are evolutionarily more distant from each other than from the parental sequence HG3.

![image](https://github.com/ccbiozhaw/FitLan/assets/80820813/25bccdf8-5228-4283-9045-dda4e29fc5b5)
Schematic representation of HG3’s fitness landscape. Overall, 208 unique sequence-function pairs stemming from the evolutionary trajectories of HG3.R5 and HG3.17 as well as combinatorial variants generated via gene shuffling were used to map HG3’s fitness landscape. For each variant, the underlying sequence space is represented by a principal component analysis of the embeddings extracted from the ESM algorithm. The fitness values represent the relative activity of each variant versus HG3.R5 calculated from the activity measurements of three biological replicates under screening assay conditions. The activity data of HG3.3, HG3.7 and HG3.14 were inferred from literature values. a, Three-dimensional representation of the fitness landscape. b, Topological view of the fitness landscape showing all data points. Sequence-activity pairs derived from the shuffled libraries are highlighted as grey dots (190 variants). Sequence-activity pairs derived from the HG3.R5 trajectory are highlighted as blue dots and labeled with their alphanumerical identifiers (5 variants), while sequence-activity pairs from HG3.17 trajectory are highlighted as purple dots and labeled with their alphanumerical identifiers (4 variants). Combined variants HG3.R5w17, HG3.17wR5 and HG3 K50Q are highlighted as orange or green dots respectively. The in silico design HG3 is highlighted with a large grey dot.

In this repository we provide both data and code that were used to visualize the fitness landscape of these enzyme variants.