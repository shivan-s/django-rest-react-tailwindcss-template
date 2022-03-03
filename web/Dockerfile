FROM nikolaik/python-nodejs:latest

ENV PYTHONDONTWEITEBYTECODE 1
ENV PYTHONNUNBUFFERED 1
WORKDIR /code

RUN pip install pipenv
COPY Pipfile Pipfile.lock /code/
RUN pipenv install

COPY . /code/
