# RizosferaMexicana
Repositorio para llevar control del proyecto Alianza Huawei

## Docker  
1. Edita el Dockerfile para instalar las dependencias que necesites
Primero clona este repositorio localmente  
`git clone  https://github.com/tipicanerd/RizosferaMexicana.git`  
edita el Dockerfile instalando lo qe neccesites.  

2. Localmente construye tu imagen de docker  
`docker build -t rizosfera.`   

3. Prueba tus dependencias entrando al contenedor 
`docker run -i -t -v $(pwd):/home rizosfera  /bin/bash`  
Ahora estarás en una terminal con prompt "#" porque eres sudo dentro del contenedor.   
`usuario #`
(Miguel, si usamos el python mas pequeño, podemos dejarle una terminal? )  

4. Cuando termines, sube el nuevo Dockerfile a Github
`git add, commit push `  

5. Actualizaremos los jueves la "imagen oficial" de Docker del equipo en el dockerhub  

## Datos
[Plantas Mexicanas con biom](https://lab.matmor.unam.mx/files) Ordenar en una sola tabla.    
Alnitak /files/metamex/raw_files/Agaves  
[Rhyzosphere metadata table](https://docs.google.com/spreadsheets/d/1f8l-wfMqngcaqajeybX2celb7g9wNLd3-Ix8tjNqM3Q/edit#gid=928779009)  
[Suelos del mundo]()    
 [ ] Cuatro Ciénegas México   
 [ ] Otra planta     
 Set de datos 2: [Reto camda2023](https://github.com/aapashkov/camda2023)  Faltan etiquetas ciudades  
 
### Datos Haxkaton 2019
#### OTUS_conservados.csv 
Contiene 3044 filas y 607 columnas. La selección de columnas se basó en ciertos criterios que pueden modificarse en el futuro. También se agegró la columna *New_Labels* se obtuvo mapeando las coordenadas para tener más información sobre el clima del lugar.

## Bitácora  
 [Bitácora de trabajo](https://docs.google.com/document/d/1o6B5qE0GtQPsN3JWRyDxnzQjfKWRsn-I8BagbWCK600/edit#heading=h.wojdmcq3lqcs)
 
 ## Pendientes marzo  
 [x] Todos, instalas docker  
 [x] Miguel sra-toolkit y conda (instalar las librerías)    
 [ ] probar kraken-biom en los datos de prueba que están en la carpeta data del repo  
     Ejemplo de prueba https://carpentries-lab.github.io/metagenomics-analysis/07-phyloseq/index.html  
     con kraken biom a partir de los report de kraken se deben generar arhicvos biom  
    instalar biom-format de python   
    con biom format a partir de un biom debemos poder cargar la tabla a python   
 [] Jazmin Biom-Format kraken-biom   
 [ x ] subir los datos de plantas mexicanas   
 [] Nelly Subir los datos del mundo  , y tabla de Haydee de metadatos   
 [] Fonty subir datos de EMB    
 [x ] Karina buscar datos control, ejemplo datos cuatro ciénegas MGRAST, NCBI SRA  
 [  ] Pendiente subir su script de qiime al gtithub
 
 ## Lecturas
 [Registro de lecturas](https://docs.google.com/spreadsheets/d/1YBW80z4DLh1hjOdCe4x4eETMSUuCAl26F5H6xf-ccCE/edit?usp=sharing)
 
 ## Referencias
 
 [Contruir aplicación de python en docker](https://linuxhandbook.com/dockerize-python-apps/)
 
[ ][Forensic Applications of Microbiomics: A Review](https://www.frontiersin.org/articles/10.3389/fmicb.2020.608101/full)  
[ ][Identification of city specific important bacterial signature for the MetaSUB CAMDA challenge microbiome data](https://link.springer.com/article/10.1186/s13062-019-0243-z)    
[ ][Editorial: Critical assessment of massive data analysis (CAMDA) annual conference 2021](https://www.frontiersin.org/articles/10.3389/fgene.2023.1154398/full)     
[ ][Unraveling city-specific signature and identifying sample origin locations for the data from CAMDA MetaSUB challenge](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7780616/)      
[ ][Unraveling City-Specific Microbial Signatures and Identifying Sample Origins for the Data From CAMDA 2020 Metagenomic Geolocation Challenge](https://pubmed.ncbi.nlm.nih.gov/34421984/)   
[ ][Metagenomic Geolocation Using Read Signatures](https://pubmed.ncbi.nlm.nih.gov/35295949/)    
[ ][Identification of city specific important bacterial signature for the MetaSUB CAMDA challenge microbiome data](https://pubmed.ncbi.nlm.nih.gov/31340852/)  
[ ][Unraveling bacterial fingerprints of city subways from microbiome 16S gene profiles](https://pubmed.ncbi.nlm.nih.gov/29789016/)  
[ ][Fingerprinting cities: differentiating subway microbiome functionality](https://pubmed.ncbi.nlm.nih.gov/31666099/)  
[][Origin Sample Prediction and Spatial Modeling of Antimicrobial Resistance in Metagenomic Sequencing Data](https://pubmed.ncbi.nlm.nih.gov/33763122/)
[][Application of machine learning techniques for creating urban microbial fingerprints](https://pubmed.ncbi.nlm.nih.gov/31420049/)   
[][Metagenomic Geolocation Prediction Using an Adaptive Ensemble Classifier](https://pubmed.ncbi.nlm.nih.gov/33959149/)    
[][Massive metagenomic data analysis using abundance-based machine learning](https://pubmed.ncbi.nlm.nih.gov/31370905/)  
[][Environmental metagenome classification for constructing a microbiome fingerprint](https://pubmed.ncbi.nlm.nih.gov/31722729/)   
[][A machine learning framework to determine geolocations from metagenomic profiling](https://pubmed.ncbi.nlm.nih.gov/33225966/)  
[][Profiling microbial strains in urban environments using metagenomic sequencing data](https://pubmed.ncbi.nlm.nih.gov/29743119/)   
[][Systematic evaluation of supervised machine learning for sample origin prediction using metagenomic sequencing data](https://pubmed.ncbi.nlm.nih.gov/33302990/)  
[][MetaBinG2: a fast and accurate metagenomic sequence classification system for samples with many unknown organisms](https://pubmed.ncbi.nlm.nih.gov/30134953/)  
[][Assessment of urban microbiome assemblies with the help of targeted in silico gold standards](https://pubmed.ncbi.nlm.nih.gov/30621760/)  
[][Metagenomics Analyses: A Qualitative Assessment Tool for Applications in Forensic Sciences](https://link.springer.com/chapter/10.1007/978-981-15-6529-8_5)  
[][Forensic Applications of Microbiomics: A Review](https://www.frontiersin.org/articles/10.3389/fmicb.2020.608101/full)  
[][Application of Microbiome in Forensics](https://www.sciencedirect.com/science/article/pii/S1672022922000961)  
[][Environmental metagenomics in urban environments and development of forensic inference](https://www.kcl.ac.uk/research/environmental-metagenomics-in-urban-environments-and-development-of-forensic-inference)  
[][Origin Sample Prediction and Spatial Modeling of Antimicrobial Resistance in Metagenomic Sequencing Data](https://pubmed.ncbi.nlm.nih.gov/33763122/)  
