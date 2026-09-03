# Personal Portfolio Website on AWS S3

A small Cloud Computing mini-project: a simple personal portfolio website, later published with Amazon S3 static website hosting.

## Objective

Build a beginner-friendly static portfolio and deploy it to the cloud. The aim is to practise core cloud ideas (storing files in the cloud and serving them as a website), not to build a large web application.

## Scope

The website will stay small enough to finish within a short project timeline.

**Included (minimum viable website)**

- One static page
- A short introduction (name and a brief about section)
- A small skills or education section
- Contact details or links (for example email and GitHub)
- Simple styling with CSS

**Not included**

- Extra pages or a blog
- JavaScript frameworks (for example React)
- A database, user accounts, or authentication
- Docker, EC2, Kubernetes, Terraform, or CI/CD
- AWS setup in this first step (that comes later)

Website files will be added in a later step. This repository currently holds the project description and folder layout only.

## Technologies

These are the tools planned for the project. Only Git and GitHub are in use so far.

| Technology | Role |
| --- | --- |
| HTML | Page structure |
| CSS | Layout and styling |
| Git and GitHub | Version control and project sharing |
| Amazon S3 | Later: store the files and host the static website |

## What the finished project is intended to demonstrate

When the project is complete, it should show that a simple website can be:

1. Written as ordinary HTML and CSS files (no server-side application)
2. Stored in Amazon S3 as objects in a bucket
3. Published with S3 static website hosting so the portfolio is available on the internet

That is enough to explain basic cloud storage and static deployment to a reviewer.

## Project structure

```text
Cloud-project/
├── README.md      # Project description (this file)
├── .gitignore     # Ignore OS files and accidental secrets
└── site/          # Static website files will be added here later
```
