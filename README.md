# Next.js

Next.js "Hello World" project for proof of concept.

## Run

```bash
npm run dev
```

## As static site

In file `next.config.js`, comment `output: "standalone"` and uncomment `output: "export"`

```bash
npm run build
```

Copy `out` folder to web server or S3.

## As Docker container

In file `next.config.js`, comment `output: "export"` and uncomment `output: "standalone"`

```bash
docker build -t nextjs-docker .
docker run -p 3000:3000 nextjs-docker
```
