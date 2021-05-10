# ##############################
# Ejemplo Dockerfile
# ###################################

# 1. Cargar el contenedor a partir de una imagen de Ubuntu

FROM ubuntu
LABEL maintainer david.carvajal@thebridge.tech 
RUN apt-get update
RUN apt install -y tzdata

# 2. Instalar node, git y el servidor http local

RUN apt install -y nodejs npm git
CMD npm install live-server

# 3. Descargar la aplicación y lanzarla

CMD git clone https://<url_proyecto>.git
CMD cd <nombre_proyecto>
CMD npm install
CMD npm start