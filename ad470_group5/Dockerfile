# start by pulling the python image
from python:3.9-slim

# copy the requirements file into the image
COPY ./requirements.txt /requirements.txt

# install the dependencies and packages in the requirements file
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# switch working directory
WORKDIR /app


# copy every content from the local file to the image
COPY app /app

# configure the container to run in an executed manner
ENTRYPOINT [ "python" ]

CMD ["app.py" ]