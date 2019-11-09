# Java legacy secrets example

This project was scaffolded from a java app engine example, [see original readme](scaffolded_readme.md). The purpose of this project is just to show how you can pass secrets as system properties to the running java application.

## Local development

1. Run `mvn clean appengine:devserver -DMY_SECRET_KEY=cookies-are-great`. This will start a local development server on http://localhost:8080 displaying the contents of the provided `MY_SECRET_KEY` secret.

## Deployment

1. Run `mvn appengine:update -DMY_SECRET_KEY=cookies-are-great` to deploy an application to the cloud together with the provided `MY_SECRET_KEY` secret. 