FROM python:3.9

# create directory code in container
WORKDIR /code 

COPY ./requirements /code/requirements.txt

# no cache for pip installation command to save time for rebuilding images
# upgrade for dependencies
RUN pip install  --no--cache-dir --upgrade -r /code/requirements

COPY ./app /code/app

CMD ["uvicorn", "app.main:app"]