FROM python:3.9

#base folder in container
ADD main.py .

#install 3rd party libraries
RUN pip install requests beautifulsoup4

#command that executes when container is started    
CMD ["python", "./main.py"]