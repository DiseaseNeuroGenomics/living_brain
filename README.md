# living_brain
Comparison between living and post-mortem mRNA expression data

Pipeline to filter and annotate living brain scRNA data  

**Step 1. ambient_removal**  
Removes ambient mRNA using CellBender and saves output anndata  

**Step 2. data_consolidation** 
Concatenates anndata from all samples after ambient removal  

**Step 3. qc**  
Filters data and annotates cells using Pegasus  

Optional (annotation using scVI and the Allen Mouse Brain Map Dataset)  

**Step 4. process_allen_brain_map**  
Creates an anndata structure of the Allen Mouse Brain Map

**Step 5. scvi_annotation**  
Annoates the cells using scVI and compares it to the Pegasus annotation

