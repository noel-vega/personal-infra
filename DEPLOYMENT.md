# Infrastructure Deployment

## First Time Setup

1. **Start core infrastructure:**
```bash
   cd infrastructure
   docker compose up -d
```

2. **Login to registry:**
```bash
   docker login registry.noelvega.dev
```

3. **Deploy applications:**
```bash
   cd ../applications
   docker compose up -d
```

## Adding New Applications

1. Build and push your image to the registry
2. Add service to `applications/docker-compose.yml`
3. Update `infrastructure/nginx.conf` with routing
4. Get SSL cert if needed
5. `docker compose up -d` in applications directory
