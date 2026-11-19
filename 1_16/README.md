# Cloud deployment

Deploy the Docker Quick Reference application from exercise 1.15 to Render
as a Web Service using the existing public image:

`docker.io/jhlow0106/docker-quick-reference:latest`

Configuration is recorded in `render.yaml`: Free instance, Singapore region,
and `/health` for health checks. The image already listens on `0.0.0.0:8080`;
Render supplies the public HTTPS endpoint and routes traffic to the container.

When using a Blueprint, select `1_16/render.yaml` as its configuration path.
The same settings can be entered in Render's Existing Image creation form.

Live service: https://docker-quick-reference.onrender.com

The public home page and `/health` were verified after deployment.
The public URL and deployment discussion are recorded in `answer`.

A free Render service sleeps after 15 minutes without traffic. Its first
request after sleeping can take about a minute while the container starts.
