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

I have a slight problem with them using a ribosome inhibitor to study ribosomal interactions.

Though tetracycline antibiotics (like doxycycline) do have lower affinity for eukaryotic ribosomes, they can effect translation in the eukaryotic cell (particularly mitochondrial translation - as seen in this very cool paper [Mitoribosomal synthetic lethality overcomes multidrug resistance in MYC-driven neuroblastoma | Cell Death & Disease](https://www.nature.com/articles/s41419-023-06278-x))













































