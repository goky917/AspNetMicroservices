

DOCKER COMMANDS:
	=> docker compose -f docker-compose.yml -f docker-compose.override.yml up -d
	=> docker compose down
	=> docker compose ps
	=> docker compose -f docker-compose.yml -f docker-compose.override.yml up --build

SERILOG:
	=> Install-Package Serilog.AspNetCore
	=> Install-Package Serilog.Enrichers.Environment
	=> Install-Package Serilog.Sinks.Elasticsearch

LAUNCH MICROSERVICES:
	=> Catalog API -> http://host.docker.internal:8000/swagger/index.html
	=> Basket API -> http://host.docker.internal:8001/swagger/index.html
	=> Discount API -> http://host.docker.internal:8002/swagger/index.html
	=> Ordering API -> http://host.docker.internal:8004/swagger/index.html
	=> Shopping.Aggregator -> http://host.docker.internal:8005/swagger/index.html
	=> API Gateway -> http://host.docker.internal:8010/Catalog
	=> Rabbit Management Dashboard -> http://host.docker.internal:15672 -- guest/guest
	=> Portainer -> http://host.docker.internal:9000 -- admin/admin1234admin
	=> pgAdmin PostgreSQL -> http://host.docker.internal:5050 -- admin@aspnetrun.com/admin1234
	=> Elasticsearch -> http://host.docker.internal:9200
	=> Kibana -> http://host.docker.internal:5601
	=> Web Status -> http://host.docker.internal:8007
	=> Web UI -> http://host.docker.internal:8006

	NUGET PACKAGES
		=> Install-Package Microsoft.Extensions.Http.Polly