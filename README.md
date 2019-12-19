# elastic-stack-starter

Use Docker Compose to launch:

```bash
 docker-compose --project-name elastic-starter up -d --build
```

This will launch:
- an Elasticsearch instance accessible from the Docker network at http://elasticsearch:9200 and from your machine at http://localhost:9200
- a Kibana instance accessible from the Docker network at http://kibana:5601 and from your machine at http://localhost:5601
- an APM Server instance accessible from the Docker network at http://apm-server:8200 and from your machine at http://localhost:8200
- an ASP.NEt web app accessible from the DOcker network at http://eshopwebmvc and from your machine at http://localhost:5106

## Sample apps
There are two sample apps:
- `dotnet-app/`: ASP.NET MVC sample app. Modified version of https://github.com/dotnet-architecture/eShopOnWeb
- `nodejs-app/`: Node.js sample app
