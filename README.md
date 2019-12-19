# elastic-stack-starter

Use Docker Compose to launch:

```bash
 docker-compose --project-name elastic-starter up -d --build
```

This will launch:
- an Elasticsearch instance accessible from the Docker network at http://elasticsearch:9200 and from your machine at http://localhost:9200
- a Kibana instance accessible from the Docker network at http://kibana:5601 and from your machine at http://localhost:5601
- an APM Server instance accessible from the Docker network at http://apm-server:8200 and from your machine at http://localhost:8200
- an ASP.NEt web app with Elastic APM added, accessible from the DOcker network at http://eshopwebmvc and from your machine at http://localhost:5106
- [COming soon] a Node.js API
- a FIlebeat agent that reads logs from all the running DOcker containers, including your app
- a Heartbeat agent that continually pings your apps (http://eshopwebmvc) for availability
- [Coming soon] a Metricbeat agent

AFter launch, visit http://localhost:5106 to play with the .NET app. Launch Kibana at http://localhost:5601 and explore the logs and metrics from your application.

## Sample apps
There are two sample apps:
- `dotnet-app/`: ASP.NET MVC sample app. Modified version of https://github.com/dotnet-architecture/eShopOnWeb
- `nodejs-app/`: Node.js sample app
