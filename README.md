<div align=center>

<img src="./public/jiosaavn-2.png" width="100px"/> 



<img width="343" height="65" alt="image" src="https://github.com/user-attachments/assets/c6c45b1f-3c52-4f78-ae78-e571d9c8f1ec" />

Jio_Saavan.com
In this project, I scraped (https://www.jiosaavn.com/) website songs List,here different type of Language song scrape. when you will run the program then it will be automate open the browser and autoplay the songs.

# 🎵 Jio Saavn API

### A simple wrapper for the Jio Saavn API powered by Hono.js 🔥.

# 🎵 Lokal Music Player (Android)

A music streaming Android application built as part of a placement assignment.  
The app consumes real music data from the public JioSaavn API and focuses on
clean architecture, reliable media playback, and consistent state management.
## 📚 References & Inspiration

The following open-source projects were used **only as references for learning
architecture and playback patterns**.  
All code in this repository has been written and adapted specifically
to meet the requirements of this assignment.

- JioSaavn API (backend reference):  
  https://github.com/sumitkolhe/jiosaavn-api

- Android ExoPlayer reference implementations:  
  https://github.com/android/uamp  
  https://github.com/google/ExoPlayer

- MVVM & Compose architecture inspiration:  
  https://github.com/android/nowinandroid

---

## ⚠️ Disclaimer

This project is created strictly for **educational and evaluation purposes**.
It does not claim ownership of any music content and uses publicly available APIs
as referenced in the assignment.


## ✨ Features

</div>

- 🚀 **Ultrafast** - Powered by [Hono.js](https://hono.dev).The router `RegExpRouter` is really fast.
- 🪶 **Lightweight** - Has minimal dependencies.
- 🌍 **Multi-runtime** - Works on `Bun`, `Node.js`, `Vercel` or `Cloudflare Workers`. The same code runs on all platforms.
- 🔥 Download High Quality Songs, w/ lyrics for supported songs.
- 🎵 Get Songs, Albums, Playlists, Artists, Radio Stations, Podcasts Lyrics, Recommendations, and more.
- ❤️ Open Source

<div align=center>

## 🛠️ Building from source

</div>

- Clone the repository

```
git clone -https://github.com/Harshasri123h/Jio-Saavan_API./tree/main
cd jiosaavn-api-ts
```

- Install dependencies

```
bun i || pnpm i || npm i || yarn
```

#### Bun

> **Warning**
> You need to have [Bun.js](https://bun.sh) installed on your machine to run the project with bun.

```
bun run dev || pnpm dev || npm run dev || yarn dev
```

#### Node.js

```
bun run dev:node || pnpm dev:node || npm run dev:node || yarn dev:node
```

#### Vercel Dev Server

```
bun run dev:vercel || pnpm dev:vercel || npm run dev:vercel || yarn dev:vercel
```

#### Cloudflare Workers

> **Warning**
> Make sure to remove Node API code from [`src/index.ts`](https://github.com/Harshasri123h/Jio-Saavan_API./blob/main/_api/index.ts) & [`config.ts`](https://github.com/Harshasri123h/Jio-Saavan_API.) before deploying or running the project with Cloudflare Workers.

[src/index.ts](https://github.com/Harshasri123h/Jio-Saavan_API.)

```diff
...

-  port: +(process.env.PORT ?? 3000),
+ port: 3000, # update accordingly

...
```



```diff
...

-  enableRateLimit: process.env.ENABLE_RATE_LIMIT === "true" ?? false,
+  enableRateLimit: false, # update accordingly
...

```

```
bun run dev:vercel || pnpm dev:cf || npm run dev:cf || yarn dev:cf
```

<div align = center>

## 🌐 Deploying your own instance

You can easily deploy your own hosted version of the `JioSaavn API` by clicking on one of the links below, which will set up a ready-to-go version for you:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/rajput-hemant/jiosaavn-api-ts)

[![Deploy with Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/rajput-hemant/jiosaavn-api-ts)

**OR**

## Deploying using CLI

</div>

### Vercel

- It utilizes Edge Functions and can automatically execute in the region nearest to the user who triggers them.
- It's worth noting that `Mumbai, India (South) - bom1` is the recommended region for this project deployment.

```
bun run deploy:vercel || pnpm deploy:vercel || npm run deploy:vercel || yarn deploy:vercel
```

> **Note**
> We are using community based [🐰 Bun runtime for ▲ Vercel Serverless Functions](https://github.com/vercel-community/bun) by default, You can also use [▲ Vercel Serverless Functions](https://vercel.com/docs/functions/serverless-functions) w/ `Node Runtime` or [▲ Vercel Edge Functions](https://vercel.com/docs/functions/edge-functions) to deploy the project.
> To use `Node Runtime` or `Edge Functions` rename the `_api` folder to `api` and remove 'buildCommand' from `vercel.json` file.

### Cloudfare Workers

```
bun run deploy:cf || pnpm deploy:cf || npm run deploy:cf || yarn deploy:cf
```

### Build and Run Docker Image

#### Docker Compose (Recommended)

- Start the container

```
docker-compose up -d # detached mode
```

- Stop the container

```
docker-compose stop # stops the container
docker-compose down # stops and removes the container
```

#### Docker

- Start Docker daemon (Skip if already running)

```
sudo dockerd
```

- Build the image

```
docker build -t jiosaavn .
```

- Run the image

```
docker run -p 80:3000 jiosaavn
```

- Open (https://jiosaavanclone.netlify.app/) to view it in the browser.

- Stop the container

```
docker ps
```

```
docker stop <container-id>
```

<div align=center>

