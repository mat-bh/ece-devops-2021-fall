# MCQ exam

The MCQ exam will contain 30 questions made of 2 parts:
- Part 1. 15 questions on command execution
- Part 2. 15 questions on knowledge of theory

The best way to prepare for Part 1 is to start working on the project catching up with all the labs, trying and experimenting with CLI commands of the technologies.

To prepare for Part 2, you are invited to re-read the entire contents of the modules.

Here are the example questions you will meet on the exam.

## Question 1

You have the following `docker-compose.yml` file:

```yaml
version: "3.8"
services:
  web:
    build: .
    ports:
      - "3000:5000"
  redis:
    image: redis
    volumes:
      - /usr/data:/data
```

Choose correct option(s) where "web" service is accessible and "redis" service attaches data:

* [ ] A: On host: URL - `localhost:3000`, folder - `/usr/data`
* [ ] B: On host: URL - `localhost:5000`, folder - `/data`
* [ ] C: In container: URL - `localhost:3000`, folder - `/data`
* [ ] D: In container: URL - `localhost:5000`, folder - `/usr/data`


## Question 2

Which Kubernetes Volume type(s) can be used for stateful services?

* [ ] A: `emptyDir`
* [ ] B: `hostPath`
* [ ] C: `nfs`
* [ ] D: `persistentVolumeClaim`

## Question 3

You have the following manifest file:

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: hello
spec:
  selector:
    matchLabels:
      app: hello
  replicas: 6
  template:
    metadata:
      labels:
        app: hello
    spec:
      containers:
        - name: hello
          image: nginx
          ports:
            - name: http
              containerPort: 80
---
apiVersion: v1
kind: Service
metadata:
  name: hello
spec:
  type: NodePort
  selector:
    app: hello
  ports:
  - port: 80
```

Which statement(s) is(are) correct when applying the following manifest file:

* [ ] A: It creates 6 Deployments, 1 Pod, 1 Service
* [ ] B: We don't manage what port of a worker node is allocated to Nginx web server
* [ ] C: Nginx web server is accessible on `localhost:80` from Kubernetes master node
* [ ] D: The service "hello" is stateless
