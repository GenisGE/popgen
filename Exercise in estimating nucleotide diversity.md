# Exercise in estimating nucleotide diversity
Casper-Emil Pedersen, Peter Frandsen and Hans R. Siegismund

### Program
* Examine the PLINK-format
* Read SNP data into R and extract information about the data
* Estimate nucleotide diversity (here as the expected heterozygosity) in different populations 
* Estimate the inbreeding coefficient for each individual in the different populations  
* Plot your results to graphically present the diversity in different population and in different regions along the chromosome

### Aim
* Get familiar with the commonly used PLINK-format
* Get familiar with extraction of simple summary statistics of data in R
* Get familiar with representation of results
* Be able to interpret diversity measures in populations

### Recommended background reading
See [Prado-Martinez et al. 2013](http://www.nature.com/nature/journal/v499/n7459/full/nature12228.html) for a comprehensive 
great ape paper

### Genetic Diversity in Chimpanzees
During this exercise you will be introduced to population genetic analysis of SNP data. The datasets used here consist of the 
variable sites found on chromosome 22 in chimpanzees. The data set contains genotypes from all four subspecies of chimpanzee 
(_Pan troglodytes_, see Figure 1), two human populations, one individual with European ancestry (CEU) and one individual with
African ancestry (YRI). The data has been filtered to reduce the size of your working data set and includes only SNP’s with 
exactly two different bases (bi-allelic).

![figure1](figures/ex1nucdivfigure1.png)
__Figure 1 | Geographical distribution ranges for the _Pan troglodytes_ subspecies.__ The range borders of each subspecies; 
yellow for _Pan troglodytes_ verus (western chimpanzee), orange for _Pan troglodytes ellioti_ (Nigerian-Cameroon chimpanzee),
pink for _Pan troglodytes troglodytes_ (central chimpanzee), and blue for _Pan troglodytes schweinfurthii_ (eastern chimpanzee).
Reprint from [http://www.unep.org/grasp/}(http://www.unep.org/grasp/) modified by C. Hvilsom. 

*Q1*: Before we get started, why do you think we chose chromosome 22?






### Getting started

Change the directory to the exercise directory and copy your data:
```
cd ~/exercises
cp ~/groupdirs/SCIENCE-BIO-Popgen_Course/exercises/apeDiversity/apeGenDiv.tar.gz 
tar -zxvf apeGenDiv.tar.gz  
rm apeGenDiv.tar.gz
cd apeDiversity
```
