FROM continuumio/anaconda3

RUN apt-get update && apt-get install -y libgtk2.0-dev && \
    rm -rf /var/lib/apt/lists/*


RUN python -m pip install --upgrade pip \
    pip install tensorflow==2.6.0 -f https://tf.kmtea.eu/whl/stable.html

RUN ["mkdir", "notebooks"]
COPY conf/.jupyter /root/.jupyter
COPY run_jupyter.sh /

# Jupyter and Tensorboard ports
EXPOSE 8888 6006

# Store notebooks in this mounted directory
VOLUME /notebooks

CMD ["/run_jupyter.sh"]