# cs3219-otot-a

## Proof of Completion

### Link to Github:

[GitHub Repo](https://github.com/xiaoyu-nus/cs3219-otot-a/tree/main)

### Instruction on how to run the container

Clone the Github Repository to you local machine.

`git clone https://github.com/xiaoyu-nus/cs3219-otot-a.git`

Navigate to the project directory.

`cd cs3219-otot-a/project`

Build the images.

`docker-compose build`

Serve the web app on localhost.

`docker-compose up`

The success message should show: `lizeyan_flask | * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)`

Now go to `http://localhost:8080` , there should be a HTML page saying "Hello World".

Now go to `http://localhost/app` , this is the reverse proxy for `localhost:8080` . The same page should be displayed.

Press `Ctrl` + `C` to quit.

### RESOURCE LINKS:

https://github.com/docker/labs/blob/master/beginner/chapters/setup.md https://docs.docker.com/get-started/
https://docs.docker.com/docker-hub/
https://www.nginx.com/resources/wiki/start/
https://www.nginx.com/resources/library/complete-nginx-cookbook/
