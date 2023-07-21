# Devil-DFTD-FOI-Coevolution
Phenotype data for GEMMA and ATOMM analyses, and GEMMA SNP loci/effect size data. Files are as follows:

<h2>GEMMA Devil Analysis</h2>
<b>File:</b> devil_GEMMA_pheno.txt<br />
Extract column 2 (FOI phenotype values) without the header to run as a GEMMA phenotype file<br /><br />
<b>File:</b> devil.FOI.primary.param.chain_mean.txt.gz<br />
Gzipped file containing all SNP loci used in the GEMMA analysis. Columns alpha (small effect size), beta (large effect size), and gamma (posterior inclusion probability of being a large-effect SNP) were generated via GEMMA.


<h2>GEMMA DFTD Analysis</h2>
<b>File:</b> DFTD_GEMMA_pheno.txt<br />
Extract column 2 (FOI phenotype values) without the header to run as a GEMMA phenotype file<br /><br />
<b>File:</b> DFTD.FOI.primary.param.chain_mean.txt.gz<br />
Gzipped file containing all SNP loci used in the GEMMA analysis. Columns alpha (small effect size), beta (large effect size), and gamma (posterior inclusion probability of being a large-effect SNP) were generated via GEMMA.

<h2>ATOMM Paired Devil-DFTD Analysis</h2>
<b>File:</b> ATOMM_pheno.txt<br />
<b>File key:</b> ATOMM_microchips.txt<br />
Run ATOMM using ATOMM_pheno.txt as is. Columns correspond to the following:<br />
<ul>
<li>Column 1: devil ID</li>
<li>Column 2: DFTD ID</li>
<li>Column 3: y-intercept</li>
<li>Column 4: DFTD first-infection status (0 = not first infected, 1 = first infected)</li>
<li>Column 5: FOI estimate (ranknorm transformed)</li>
</ul>

The key file ATOMM_microchips shows devil microchip, DFTD microchip, and untransformed FOI estimates. Each row of the key file (minus the header) corresponds to an equivalent row in ATOMM_pheno.txt
