# Docker Linting Demo
Linting Docker demo

### Install
Here i am using OSX, installing hadolint using brew.
```
$ brew install hadolint
```

#### hadolint Dockerfile 
```
$ hadolint Dockerfile 
Dockerfile:4 DL3020 Use COPY instead of ADD for files and folders
```

```
$ hadolint --ignore DL3003 --ignore DL3006 Dockerfile 
Dockerfile:4 DL3020 Use COPY instead of ADD for files and folders
```

```
$ hadolint --trusted-registry xyz.com:500 Dockerfile 
Dockerfile:1 DL3026 Use only an allowed registry in the FROM image
Dockerfile:4 DL3020 Use COPY instead of ADD for files and folders
```
