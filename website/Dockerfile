FROM python:3.9-alpine


ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
RUN mkdir /website
WORKDIR /website
RUN pip install --upgrade pip
COPY requirements.txt /website/

RUN pip install -r requirements.txt
COPY .. /website/

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]