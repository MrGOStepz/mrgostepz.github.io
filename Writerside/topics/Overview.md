# Overview

## Docker Ecosystem
```mermaid
block-beta
  columns 2
  z:2
  z["Docker Ecosystem"]
  block:group1:2
    columns 2
    a["Docker-Client"] b["Docker-Server"] c["Docker-Machine"] d["Docker-Images"] e["Docker-Hub Docker-Compose"]
  end
```
## What is Docker
Docker is an open-source platform that enables developers to build, deploy, run,
and manage applications using containers.
Image is a file to collect the dependencies and config required to run a program

Container is an instance of an image to run a program.
```mermaid
  flowchart LR
  im["Image <br>"] --> A["Container"]
  im --> B["Container"]
  im --> c["Container"]
```

## Docker Run Hello World
```mermaid

  flowchart TD
  d-->g-->e
  a["docker run helloworld:latest"] --> b
  subgraph y["Your Computer"]
    b["Docker Client"] --> d["Docker Server"]-->e["Image Cache"]
  end
  
  subgraph h["Docker Hub"]
    g["hello-world"]
    redis
    ImageA
    ImageB
  end
```
