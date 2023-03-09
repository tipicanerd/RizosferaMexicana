FROM python:slim

#Actualiza el SO e instala dependencias
RUN apt-get update && apt-get -y upgrade \
    && apt-get install -y --no-install-recommends \
        git \
        wget \
        #g++ \
        #gcc \
        ca-certificates \
        && rm -rf /var/lib/apt/lists/*

#Instala MiniConda
ENV PATH="/root/miniconda3/bin:${PATH}"
ARG PATH="/root/miniconda3/bin:${PATH}"
RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh \
    && mkdir /root/.conda \
    && bash Miniconda3-latest-Linux-x86_64.sh -b \
    && rm -f Miniconda3-latest-Linux-x86_64.sh 


WORKDIR /home

#Clonar el repo
RUN git clone https://github.com/tipicanerd/RizosferaMexicana.git

#Instala sra-tools y kreken-biom
#RUN conda install -c bioconda sra-tools kraken-biom -y

#Instala sra en ubuntu
RUN wget --output-document sratoolkit.tar.gz https://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/current/sratoolkit.current-ubuntu64.tar.gz \
    tar -vxzf sratool* \
    export PATH=$PATH:$PWD/sratoolkit.3.0.1-ubuntu64/bin


#COPY directorio_original directorio_imagen
COPY . /src 
#al correr -v $pwd:/src ### Mejor para codigo
CMD ["python", "/src/hola.py"]

#Para abrir terminal 
#docker run -i -t prueba_python /bin/bash



