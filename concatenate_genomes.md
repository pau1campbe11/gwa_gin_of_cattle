

    gunzip -c GCA_964213955.1_nxOstOste4.1_genomic.fna.gz  GCA_965643665.1_nxCooOnco1.hap1.1_genomic.fna.gz > combined_ref_genome.fa

To sense check the concatenated file, count the number of headers before and after. 

     zgrep -c '^>' nxCooOnco1.hap1.1_genomic.fna.gz
      194 

     zgrep -c '^>' GCA_964213955.1_nxOstOste4.1_genomic.fna.gz
      118

     grep -c '^>' combined_ref_genome.fa 
      312 
