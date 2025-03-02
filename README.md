# github-axtion

# docker build and run
$ docker build -t sltrx:1.0.0 . <br>
$ docker run -p 8081:5000 sltrx:1.0.0 <br>
$ curl http://localhost:8081/welcome/hermanwahyudi <br>

# docker-compose
$ docker-compose up --build -d <br>
$ curl http://localhost:8000/welcome/hermanwahyudi <br>

# run github actions
> Go to Actions <br>
> Select Build and Push Docker Image <br>
> Run workflows and define branch also tag that you need <br>
> Public DockerHub https://hub.docker.com/r/hermanwahyudi/sltrx <br>

# kubernetes apply deployment
$ k apply -f manifests -n sltrx <br>
$ k port-forward svc/sltrx 5000:5000
