# Parent_Ion_Scan_XCMS
This pipeline was built to automatize the detection of precursor ion peaks from tandem MS data in XCMS and the creation of Multiple Reaction Monitoring (MRM) channels. This method relies on MS data generated in precursor ion scan mode, which uses a fixed m/z on the MS2 detector to scan for precursors of specific fragments. Here, 97 m/z was used as bait as it corresponds to the "D-ring" fragment commonly produced by strigolactones. Peak detection was carried out using a combination of two peak-picking algorithms in XCMS, continuous wavelet transform (CWT) and MassifQuant.


<p align="center">
<img src="https://github.com/Sbsten/Precursor_Ion_Scan_XCMS_SLs/blob/main/Graphical_summary_method.png"
      width="600">
  <br>
  <em>Figure 1. Putative strigolactones detection workflow.</em>
</p>


While being used for strigolactones detection here, this method can also be applied to other small molecules with conserved fragmentation patterns.

MS data were generated using a XEVO TQ XS (Waters) and converted to open source format with MSconvert (ProteoWizard). The raw data are available in the MassIVE database using the data set identifier MSV000101943 (https://doi.org/doi:10.25345/C53B5WN9D). All pre-processed data and metadata needed to reproduce the analysis are available in the /Data folder. The annotated code is available in the Precursor_Ion_Scan_XCMS_SLs.Rmd file.

