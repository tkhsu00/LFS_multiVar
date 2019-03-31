# LFS_multiVar

Input file can be found at http://p53.iarc.fr/DownloadDataset.aspx 
Under "Germline mutations", download "TP53 germline mutations and family history (data files)"

The file used in this repository was downloaded on Mar 26, 2019

# Data cleaning
1. Remove missing data: remove rows without age of tumor onset or individual code.
2. For patients have multiple cancers, pick the first onset cancer types, combine these cancers in a new column "Short_topo_combined", and count the number of cancers occured at first onset, add it to column "Short_topo_combined_count".
3. Select columns for analysis based on file "column_to_analyze.txt"
