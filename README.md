# ASP.NET Core Consul Spike

An ASP.NET Core web api that registers itself with Consul on startup with Traefik as an API gateway.
All components run in Docker.

* Consul dashboard is at http://localhost:8500
* Traefik dashboard is at http://localhost:8080
* Traefik entrypoint is at http://localhost:80
* Web api is available through Traefik at http://localhost:80/consul-api-test

## Example

Create containers:  
`docker-compose up -d`  

Call API:  
`curl http://localhost/consul-test-api/values`