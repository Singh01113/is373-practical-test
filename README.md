# IS373 Practical Test

Secure containerized website deployed to a DigitalOcean server using GitHub Actions.

## Sites

QA:
https://amman-qa.134-209-120-185.sslip.io

Production:
https://amman-prod.134-209-120-185.sslip.io

## CI/CD Process

Pushes to the `qa` branch validate the website, build a Docker image, push the image to GitHub Container Registry, and automatically deploy the QA container.

Pushes or merges to `main` perform the same process and automatically deploy production.

If validation or the Docker build fails, deployment stops.

## SSH Security

The DigitalOcean server uses a non-root `deploy` account.

SSH key authentication is enabled.

Root SSH login is disabled.

Password-based SSH login is disabled.

## Test Evidence

Screenshots and successful GitHub Actions workflow links will be added after testing QA and production.
