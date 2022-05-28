#Celem projektu była analiza SNP 


1. W pierwszej kolejności pobrałem 1 000 000 odczytów z każdej próbki wykorzystując komędę fastq-dump.
2. Kolejnym krokiem była analiza jakościowa podanych odczytów do tego wykorzystano fastqc ponieważ odzczyty jakości były w miarę ok. 
Więc usunołem tylko te odczyty które wykraczały poza jakość przy pomocy trimmomatica następie znów przetestowałem jakość i wynkiki przedtawiłem w folderze Data.
3. Następnie pobrałem genom referencyjny i przygotowłaem bibliotekę do adnotacji dzięki hisat2-buildindex.
4. Po zmapowaniu do genomu ref dane zamieniłem z plików SAM na pliki BAM przy pomocy narzędzi samtools.
5. Do dokonania detekcji wariantów urzyłem Bcftools czego wynikiem był plik vcf.
6. Otrzymane dane moża zwizualizować wykorzeystałem do tego pakiet vcfR i program IGV
