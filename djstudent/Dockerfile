FROM django

# ENV PYTHONUNBUFFERED 1

WORKDIR /my-first-app

COPY requirements.txt /app/requirements.txt

# COPY . /django-quick-start
 
ADD . /my-first-app

RUN pip3 install -r requirements.txt
 
# CMD [ "python3", "./manage.py runserver 0.0.0.0:8000" ]

CMD python3 manage.py migrate
 
CMD python3 ./manage.py runserver 0.0.0.0:8000 
