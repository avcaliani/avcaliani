## Semantic Versioning

Here is a suggestion on how to manage versions, plus, I'll add some tutorials on how to create those versions in Git and DockerHub.

## Versioning Strategy

I'm following a [semantic versioning](https://semver.org/) convention, example 👇

```bash
MAJOR.MINOR.PATCH
```

> I'm also keeping the GitHub tags aligned with the DockerHub Tags.  
> [Image by Byte Byte Go](https://blog.bytebytego.com/p/ep120-what-do-version-numbers-mean)

## How to do it?

### Git Tag

```bash
git tag 1.0.0
git push origin --tags
```

### DockerHub

You need to log-in in DockerHub so you can push images there.

> ref: [build and push your first image](https://docs.docker.com/get-started/introduction/build-and-push-first-image)

```bash
# Template <dockerhub-username>/<dockerhub-repo>:<version>
docker build -t <username>/<repo>:1.1.0 .
docker tag <username>/<repo>:1.1.0 <username>/<repo>:latest

docker push <username>/<repo>:1.1.0
docker push <username>/<repo>:latest
```
