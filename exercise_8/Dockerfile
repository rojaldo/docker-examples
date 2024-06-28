from archlinux:base-devel
# update the system
RUN pacman -Syu --noconfirm
# install asciidoctor
RUN pacman -S asciidoctor --noconfirm
# install git
RUN pacman -S git --noconfirm
VOLUME /output
# workdir to /app
WORKDIR /app
# clone the repository
RUN git clone https://github.com/rojaldo/docker-examples.git
# change to the directory
WORKDIR /app/docker-examples/exercise_8
# run the asciidoctor command and move the output to the /output directory
CMD asciidoctor contenedores_con_GUI.adoc -o /output/contenedores_con_GUI.html
