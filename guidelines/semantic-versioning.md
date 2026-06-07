## Semantic Versioning

Here is a suggestion on how to manage versions, plus, I'll add some tutorials on how to create those versions in Git and DockerHub.

## Versioning Strategy

I'm following a [semantic versioning](https://semver.org/) convention, example 👇

```bash
MAJOR.MINOR.PATCH
```

> I'm also keeping the GitHub tags aligned with the DockerHub Tags.

![byte-byte-go](https://substackcdn.com/image/fetch/w_1456,c_limit,f_webp,q_auto:good,fl_lossy/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Fefaeb917-d62e-4f04-b3bc-0644d50fa948_800x988.gif)

> [Image Source](https://blog.bytebytego.com/p/ep120-what-do-version-numbers-mean)

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
