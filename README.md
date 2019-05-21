# docker-parity-nginx

Simple docker-compose to launch a contained parity/nginx enviroment.

The main purpose of this project is to create an easy and fast way to launch a (secure) parity instance with RPC capabilities.

## Usage

First, find and replace `{{your_address}}` in the project with your IP / domain. This can be done easily with:

```
grep -lR "{{your_address}}". | xargs sed -i 's / {{your_address}} / YOUR-ADDRESS / g'
```

Then, launch the docker-compose:

```
docker-compose up --build -d
```