# ANALISI DATA

## BUILD
	doccker container build -t NAME  .



## COMAND
	perl vcf2maf.pl --input-vcf /data3/test.vcf --output-maf /data3/test.vep.maf --vep-data /mnt/ --ref-fasta /mnt/homo_sapiens/87_GRCh37/Homo_sapiens.GRCh37.75.dna.primary_assembly.fa



docker container run -it  -v /mnt/mpwork/Database_tutorial2017/vep/homo_sapiens:/mnt/homo_sapiens -v /home/maurizio/Desktop/TEST2/SOMATIC_RESULTS/Results/:/data3  vcf2maf_87 /bin/bash

link[https://github.com/ohsu-comp-bio/dockerized-tools/tree/develop/vcf2maf]


	docker container run -it  -v /mnt/mpwork/Database_tutorial2017/vep/homo_sapiens:/mnt/homo_sapiens -v /home/maurizio/Desktop/TEST2/SOMATIC_RESULTS/Results/:/data3  vcf2maf_87 perl vcf2maf.pl --input-vcf /data3/somaticsniper/432.somaticsniper.vcf --output-maf /data3/432.somaticsniper.vep.maf --vep-data /mnt/ --ref-fasta /mnt/homo_sapiens/87_GRCh37/Homo_sapiens.GRCh37.75.dna.primary_assembly.fa
