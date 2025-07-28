# syntax=docker/dockerfile:1
FROM python:3
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1
WORKDIR /code
COPY requirements.txt /code/
RUN pip install -r requirements.txt
COPY . /code/
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

#Now we can run the following command to create and run the container image:
#You can launch the application the same way you have previously in this project as well, through Launch Application and specifying port 8000.
#docker build . -t my-django-app:latest && docker run -e PYTHONUNBUFFERED=1 -p  8000:8000 my-django-app 
