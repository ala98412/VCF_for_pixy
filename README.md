# VCF_for_pixy

VCF file = THRB.bi.vcf.gz
popmap   = popmap.txt
bed file = region.n10.bed

command = 
pixy --vcf $vcf \
        --population $popmap\
        --bed_file $windows_bed\
        --n_cores 10 \
        --stats pi dxy fst \
        --output_folder ./out_THRB.bi/ \
        --bypass_invariant_check
