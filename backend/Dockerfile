FROM python:3.8-slim-buster
ENV PYTHONUNBUFFERED=1

WORKDIR /backend
COPY ./requirements.txt /backend
RUN pip install -r requirements.txt
COPY . /backend/
COPY ./runscript.sh /

ENTRYPOINT ["sh", "/runscript.sh"]