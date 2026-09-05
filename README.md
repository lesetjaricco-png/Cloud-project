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

The website is in the `site/` folder. It uses HTML and CSS, runs locally, and has not been deployed to AWS yet.

## Technologies

These are the tools planned for the project. HTML, CSS, Git, and GitHub are in use so far. Amazon S3 will be added later.

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
├── README.md
├── .gitignore
├── screenshots/
│   ├── day3-desktop.png
│   └── day3-mobile.png
└── site/
    ├── index.html
    └── style.css
```

## Day 2 Progress

The first working local version of the website is now in the repository.

**What was implemented**

- A valid HTML5 page with header, about, skills, education, and contact sections
- A small stylesheet so the page is readable (not a polished design)

**Where the website files are located**

- `site/index.html`
- `site/style.css`

**How the website was tested locally**

From the `site/` folder:

```text
python -m http.server 8000
```

Then open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in a browser. You can also open `site/index.html` directly in a browser.

**What the current website contains**

- Name and role
- A short about paragraph
- A skills list
- A short education note
- Email and GitHub contact links

**What remains for future days**

- Improve the page if needed
- Create an S3 bucket
- Upload the site files
- Enable S3 static website hosting

The website currently runs locally and has not yet been deployed to AWS.

## Day 3 Progress

CSS was added and the visual design was improved. The site is still a single static page (HTML + CSS only).

**What changed**

- The page now has a dark header with in-page navigation
- Content sits in simple cards with clearer spacing and typography
- Skills are shown as labels; contact details are easier to scan
- A media query stacks the header on narrower screens

**How it was tested locally**

From the `site/` folder:

```text
python -m http.server 8080 --bind 127.0.0.1
```

Then open [http://127.0.0.1:8080/](http://127.0.0.1:8080/) in a browser.

(`8080` was used because port `8000` was already in use on this machine. The usual command is `python -m http.server 8000`.)

Checks:

- HTML and CSS both loaded
- About, Skills, Education, and Contact were visible
- The Contact nav link jumped to `#contact`
- At 375px width the header stacked and the page did not scroll sideways

Screenshots from that local test are in `screenshots/`.

**What remains for later days**

- Create an S3 bucket
- Upload the `site/` files
- Enable S3 static website hosting

The website currently runs locally and has not yet been deployed to AWS.
