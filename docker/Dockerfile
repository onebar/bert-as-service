FROM tensorflow/tensorflow:1.12.0-py3
RUN pip install bert-serving-server
COPY ./ /app
WORKDIR /app
CMD ["bert-serving-start", "-cpu", "-num_worker=$1", "-model_dir /app/docker/model"]
