FROM python:3.10.0-slim-bullseye
COPY ./flask_ml /home/ML_API/flask_ml
COPY ./requirements.txt /home/ML_API/requirements.txt
RUN apt-get update
WORKDIR /home/ML_API/
RUN pip3 install -r requirements.txt
WORKDIR /home/ML_API/flask_ml
EXPOSE 5000
ENTRYPOINT [ "python3", "main.py" ] 