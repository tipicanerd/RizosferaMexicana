# RizosferaMexicana
Repositorio para llevar control del proyecto Alianza Huawei

## Docker  
1. Edita el Dockerfile para instalar las dependencias que necesites
Primero clona este repositorio localmente  
`git clone  https://github.com/tipicanerd/RizosferaMexicana.git`  
edita el Dockerfile instalando lo qe neccesites.  

2. Localmente construye tu imagen de docker  
`docker build -t algun-nombre .`   

3. Prueba tus dependencias entrando al contenedor 
`docker run -i -t algun-nombre  /bin/bash`  
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
 
 Pendientes  
 [] Todos, instalas docker
 [] Miguel sra-toolkit y bioconda (instalar las librerías)  
 [] Jazmin Biom-Format kraken-biom subir los datos de plantas mexicanas  
 [] Nelly Subir los datos del mundo  , y tabla de Haydee de metadatos  
 [] Fonty subir datos de EMB  
 [] Karina buscar datos control, ejemplo datos cuatro ciénegas MGRAST, NCBI SRA  
 
