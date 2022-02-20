FROM python:3.8-slim-buster
ENV PYTHONUNBUFFERED=1

WORKDIR /backend
COPY ./requirements.txt /backend
RUN pip install -r requirements.txt
COPY . /backend/
COPY ./runscript.sh /

RUN groupadd -r user && useradd -r -g user user
RUN chown -R user:user /backend
USER user

ENTRYPOINT ["sh", "/runscript.sh"]