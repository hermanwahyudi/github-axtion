# github-axtion

# docker build and run
$ docker build -t sltrx:1.0.0 .
$ docker run -p 8081:5000 sltrx:1.0.0
$ curl http://localhost:8081/welcome/hermanwahyudi

# docker-compose
$ docker-compose up --build -d
$ curl http://localhost:8000/welcome/hermanwahyudi

# run github actions
> Go to Actions
> Select Build and Push Docker Image
> Run workflows and define branch also tag that you need

# kubernetes apply deployment
$ k apply -f manifests -n sltrx
$ k port-forward svc/sltrx 5000:5000
