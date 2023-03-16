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
`docker run -i -t -v rizosfera  /bin/bash`  
Ahora estarás en una terminal con prompt "#" porque eres sudo dentro del contenedor.   
`usuario #`
(Miguel, si usamos el python mas pequeño, podemos dejarle una terminal? )  

4. Cuando termines, sube el nuevo Dockerfile a Github
`git add, commit push `  

5. Actualizaremos los jueves la "imagen oficial" de Docker del equipo en el dockerhub  

## Datos
[Plantas Mexicanas con biom](https://lab.matmor.unam.mx/files)  
[Suelos del mundo]()  
 [ ] Cuatro Ciénegas México   
 [ ] Otra planta   
 
 Bitácora  
 [Bitácora de trabajo](https://docs.google.com/document/d/1o6B5qE0GtQPsN3JWRyDxnzQjfKWRsn-I8BagbWCK600/edit#heading=h.wojdmcq3lqcs)
 
### Datos Haxkaton 2019
#### OTUS_conservados.csv 
Contiene 3044 filas y 607 columnas. La selección de columnas se basó en ciertos criterios que pueden modificarse en el futuro. También se agró la columna *New_Labels* se obtuvo mapeando las coordenadas para tener más información sobre el clima del lugar.


# Pendientes marzo  
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
 [] Karina buscar datos control, ejemplo datos cuatro ciénegas MGRAST, NCBI SRA    
 
 Referencias
 [Contruir aplicación de python en docker](https://linuxhandbook.com/dockerize-python-apps/)
 
