FROM python:3.9

# create directory code in container
WORKDIR /code 

COPY ./requirements.txt /code/requirements.txt

# no cache for pip installation command to save time for rebuilding images
# upgrade for dependencies
RUN pip install  --no-cache-dir --upgrade -r /code/requirements.txt

COPY ./app /code/app

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]