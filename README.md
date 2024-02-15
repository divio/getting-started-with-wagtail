# Getting Started with Wagtail

[![Deploy to Divio](https://img.shields.io/badge/DEPLOY-TO%20DIVIO-DFFF67?logo=docker&logoColor=white&labelColor=333333)](https://control.divio.com/app/new/?template_url=https://github.com/divio/getting-started-with-wagtail/archive/refs/heads/main.zip)

Welcome to our QuickStart template – your portal to swift application development and seamless local testing. Whether you're delving into Wagtail for the first time or optimizing your workflow, our template, based on Wagtails' [Quick install tutorial](https://docs.wagtail.org/en/stable/getting_started/quick_install.html#quick-install), has got you covered.

## Automated Setup

Use the app creation wizard with a free [Divio Account](https://control.divio.com/?template=true) and choose **Wagtail** from the template selection.

## Manual Setup

1. Create a Free [Divio Account](https://control.divio.com/?template=true).
2. Click `Deploy to Divio` and follow the app creation wizard.
3. In your app's **Service** section, add a **PostgreSQL** database.
4. In the **Settings** section, add the **Release Command**: `python manage.py migrate`.
5. Deploy your app to the `test` or `live` environment.

For in-depth details about Divio Cloud, refer to the [Divio documentation](https://docs.divio.com/introduction/).

## Local Setup

1. Ensure [Docker](https://docs.docker.com/get-docker/) is installed and running.
2. Clone this repository locally.
3. Build the app with `docker compose build`.
4. Run the migrations with `docker compose run --rm web python manage.py migrate`
5. Create a superuser with `docker compose run --rm web python manage.py createsuperuser`
6. Run the app using `docker compose up`.
7. Open [http://localhost:8000]() to view your app.

Alternatively, set up your Divio Cloud app locally using the [Divio CLI](https://github.com/divio/divio-cli).
