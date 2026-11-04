#### Definitions/Terms

> Ribosome codon recognition sites

Ribosomes contain <u>three codon recognition</u> sites which perform different functions during protein synthesis.

- AminoAcyl-tRNA site (A-site)
- Peptidyl site (P-site)
- Exit site (E-site)

<img src="C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261027133559644.png" alt="image-20261027133559644" style="zoom:33%;" />

>  Ribosome recycling

From google: *"Ribosome recycling is the essential final and fourth stage of protein synthesis where the post-termination ribosome complex—which remains bound to messenger RNA (mRNA) and transfer RNA (tRNA) after the finished protein is released—is actively disassembled into its separate large and small subunits"*

> RiboSeq



Wikepedia article on how it works (check a peer reviewed source too)[[Ribosome profiling - Wikipedia.pdf](file:///C:/Users/Tim/OneDrive/__MScBioinformatics/2_Bioinformatics+CloudComputing/+Project/Ribosome profiling - Wikipedia.pdf)]



An article critiqing the variants of riboseq and the computational methods used to analyse them...

[RiboSeq.pdf](file:///C:/Users/Tim/OneDrive/__MScBioinformatics/2_Bioinformatics+CloudComputing/+Project/RiboSeq.pdf)





# Kisari et al., 2020

#### The research question

**eEF3** is an translation elongation factor

- It is <u>mostly specific to fungal species (but also others).</u> 

- It is essential for viability and elongation (likely why this study performed depletion, not K/O - though this is still a limitation )



**It is incompletely understood why eEF3 is important in elongation.** What was then known:

- *In-vitro* studies show it promotes AA-tRNA delivery to the A site by eEF1A.
- Also using an in-vitro approach, Kurata et al., 2010, found that eEF3 dissasembles the termination complex (ATP-dependent process) - from which they proposed that eEF3 has a dual role in both elongation and recycling.
- However, the studies showed that eEF3 does not produce half-mers (small ribosomal subunits that remain attached to their mRNA templates after dissociating from large ribosomal subunits). So Kurata et al., 2010 proposed that eEF3's role in recycling is via ejecting p-site tRNA and mRNA (rather than by breaking up the ribosomal subunits).
- This was somewhat backed up by a structural study that showed eE3F binds the ribosomal E site and competes with E-site tRNAs (ATP-dependent) 

As most of these studies were limited to in-vitro systems, a key strength of this study is that it analyses the role of eEF3 in-vivo.

> So the <u>fundamental</u> question in this study is: Where do ribosomes stall/get stuck when we deplete eEF3? 



**1. Their experimental system**

> **Side note: my issues with their system**
>
> Though tetracycline antibiotics (like doxycycline) do have lower affinity for eukaryotic ribosomes, they can effect translation in the eukaryotic cell (particularly mitochondrial translation - as seen in this very cool paper [Mitoribosomal synthetic lethality overcomes multidrug resistance in MYC-driven neuroblastoma | Cell Death & Disease](https://www.nature.com/articles/s41419-023-06278-x))
>
> Luckily, they didnt go with this system, they instead developed a methionine-repressible system. I still would be a little skeptical of using an amino-acid sensitive system to study changes in protein translation... I believe there are now newer systems which are better.

No LC on this blot, but they've given some other factors which do not change that dramatically so its not the end of the world. Given they later go on to try and claim that overall translation rate isn't changed, it would have been nice to have a real LC though.

eEF3 actually looks like its in higher concentrations in these cells compared to the WT, suggesting the baseline expression might be changed as a result of switching the 5' UTR. 

<img src="C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261103143120782.png" alt="image-20261103143120782" style="zoom:50%;" />





**Effects of eEF3 repression on growth and translation** 

<img src="C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261103143144241.png" alt="image-20261103143144241" style="zoom:50%;" />



![image-20261104000519074](C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261104000519074.png)



****

# Task 1. Validation figures

It makes sense that whoever does this also does the processing of the fastq files,



![image-20261104000728622](C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261104000728622.png)

a-b seem to be for both samples

c-e seem to only be for the depleted samples, looking at the reproducibility of:

- ORF coverage (Riboseq) 
- ORF coverage (RNA-seq)
- codon coverage 

>  **ORF coverage**. The ORF coverage represents the proportion of nucleotide positions that are covered by RPF reads relative to the length of the ORF. ([REPARATION: ribosome profiling assisted (re-)annotation of bacterial genomes - PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC5714196/)) 

Is RPM an appropriate metric here? (RNA-seq typically uses TPM RPKM or FPKM)

I expect that a-d will be quite straightforward, but e could be a little more challenging depending on how detailed they've described it.

(note: there is also similar plots in the supplement if we have time...)

<img src="C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261104002708725.png" alt="image-20261104002708725" style="zoom:33%;" />



# 2. Ribosomal load Figures 

![image-20261104003057336](C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261104003057336.png) 

I imagine that this task is quite linked to the first part ... so maybe the same person could do all?





# 3. GO term analysis 

(no figure attached, but important to remember...)

This should be fairly straightforward.

- Also includes 6  



# 4. ribosome density plots 

![image-20261104003852170](C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261104003852170.png)

This looks like it will likely be a little complicated...





# 5. motif-enrichement figures

this will include 5, but also supplementary 7 



 ![image-20261104004223364](C:\Users\Tim\AppData\Roaming\Typora\typora-user-images\image-20261104004223364.png)





























