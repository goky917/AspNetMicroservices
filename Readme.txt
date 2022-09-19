

DOCKER COMMANDS:
	=> docker compose -f docker-compose.yml -f docker-compose.override.yml up -d
	=> docker compose down
	=> docker compose ps

SERILOG:
	=> Install-Package Serilog.AspNetCore
	=> Install-Package Serilog.Enrichers.Environment
	=> Install-Package Serilog.Sinks.Elasticsearch
