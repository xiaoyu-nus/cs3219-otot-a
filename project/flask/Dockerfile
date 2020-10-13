# base image
FROM alpine:3.5

# install python and pip
RUN apk add --update py2-pip

# install python modules needed by the python app
COPY requirements.txt /user/src/app/
RUN pip install --no-cache-dir -r /user/src/app/requirements.txt

# copy files required for the app to run
COPY app.py /user/src/app/
COPY templates/index.html /user/src/app/templates/

# specify port number to be exposed by container
EXPOSE 5000

# run the application
CMD ["python", "/user/src/app/app.py"]
