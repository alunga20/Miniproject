# HOMOLOGY MODELLING

---
- Also known as comparative modelling of proteins, refers to constructing an atomic-resolution model of protein

- Relies on the identification of one or more known protein structures likely to resemble the structure of query sequences.

- On production of an alignment that maps residues in the query sequence to residues in template sequence.

- Protein structures are more conserved than protein sequences amongst homologue but sequence falling below a 20% sequence identity can have different structure.

- Evolutionary related proteins have similar sequences and naturally occuring homologous proteins have similar protein structure.

- The sequence alignment and template structure are then used to produce a structural model of target, because protein structures are more conserved than DNA sequences and detectable levels of sequence similarity.

## **Principle;** 

- Quality of homology models is dependant on the quality of the sequence alignment and template structure.

---


- SWISS-MODEL workspace(used in reproducing this paper) is an integrated Web-based modeling expert system. 


- For a given target protein, a library of experimental protein structures is searched to identify suitable templates. 


- On the basis of a sequence alignment between the target protein and the template structure, a three-dimensional model for the target protein is generated. 


- Model quality assessment tools are used to estimate the reliability of the resulting models. 


- Homology modeling is currently the most accurate computational method to generate reliable structural models and is routinely used in many biological applications. 


- Typically, the computational effort for a modeling project is less than 2 h. However, this does not include the time required for visualization and interpretation of the model, which may vary depending on personal experience working with protein structures.


## List of protein structure prediction softwares 


![Screenshot 2022-03-14 at 10-48-40 List of protein structure prediction software - Wikipedia](https://user-images.githubusercontent.com/88286419/158127737-65e5233c-635b-45ee-8dd5-209c00ee694a.png)

[link](https://en.wikipedia.org/wiki/List_of_protein_structure_prediction_software)

## Steps Involved in modelling

_ All sequence formats used to reproduce [citation](https://www.researchgate.net/publication/264790092_Homology_Modeling_of_CYP1A1_CYP1B1_and_its_Subsequent_Molecular_Docking_Studies_with_Resveratrol_and_its_Analogues_using_AutoDock_Tools_40) are found in [sequences_formats](https://github.com/alunga20/Miniproject/tree/main/sequence_formats)


**Step 1** - Template Identification.
- Target sequence in FASTA format as input(CYP1A1 and CYP1B1 protein sequences in FASTA format as target sequences)
- BLASTp against PDB(to obtain the related protein sequence to be used as template by the BLAST against PDB)
- Identify proteins with "good" hit(crystal structure of CYP1A2 (PDB_ID: 2HI4)as template showing more than 40% identity)
- Pairwise sequence alignment( The co-ordinates structurally conserved regions for CYP1A1 and CYP1B1 were assigned from the template (PDB_ID: 2HI4) using pairwise sequence alignment based on the Needleman-Wunsch algorithm (Needleman et al, 1970 and Thomson _et al_, 1994).)

**Step 2**
- Homology Modelling(using a suitable software, SWISS-MODEL or MODELLER, construct 3D models). After construction of 3-D model of CYP1A1
and CYP1B1 heme group was introduced into the protein
to occupy the same position as heme of the template
protein CYP1A2. 
- Finally energy minimization of the
constructed structures was performed until the energy
gradient was lower than 0.1Kcal/mole ?? using CharMM
force field.
- Model assessment and refinement using Structural analysis and verification server [link](https://saves.mbi.ucla.edu/)

![Screenshot 2022-03-14 at 11-34-05 SAVESv6 0 - Structure Validation Server](https://user-images.githubusercontent.com/88286419/158139610-4d2f7bf5-c2e8-4864-aaca-1b0aa6f12b6d.png)


