## React PWA Project test

This is a simple React App to test PWA in newest versions

## Getting started

Before running the server on a local machine for development, you need to
set the https protocol to run the PWA side

Go to Chrome and paste the next path

```bash
chrome://flags/#unsafely-treat-insecure-origin-as-secure
```

And set the Insecure origins treated as secure to enable, then put the next path as insecure to secure path

```bash
http://localhost:3000
```

Finally, run the server!

```bash
npm start
# or
yarm start
```

## Docker

```bash
docker run -it --rm -v ${PWD}:/app -v /app/node_modules -p 3000:3000 -e CHOKIDAR_USEPOLLING=true sample:dev
# OR
docker compose up
```
