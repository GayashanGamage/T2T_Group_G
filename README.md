# Run project
Clone the repository

## DO NOT USE docker-compose up.
still there is a issue on docker-compose.yml file. there for do not try to start all services using this. insterd try to build and run each service one by one. follow bellow instructions 

## Run FastAPI 

Step 1: direct to FastAPI directory

```bash
cd FastAPI
```

Step 2: build a Docker container

```bash
docker build -t api
```

Step 3 : run the container
```bash
docker run -p 3000:3000 api
```

Step 4: access api-doc via [localhost://3000](http://0.0.0.0:3000/docs)


# Run Keycloak

Step 1: direct to Keycloke directory

```bash
cd Keycloke
```

Step 2: run docker-compose file

```bash
docker-compose up -d
```

Step 3: access to the keyclock inteface by [localhost](http://localhost:8080)


# Run flowiseai

Step 1: direct to the flowise directory

```bash
cd Flowise
```

Step 2: start flowise

```bash
docker-compose up -d
```

Step 3: access to the flowise using http://localhost:3000/


# Run Vuejs - frontend

Step 1: direct to the Frontend directory

```bash
cd Frontend
```

Step 2: buil docker image

```bash
docker build -t frontend .
```

Step 3: run the container

```bash
docker run -p 5173:5173 frontend
```

Step 4: access to the frontend by http://localhost:5173/ 