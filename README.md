# Flow Backend

This is a RESTful API with [Drizzle](https://orm.drizzle.team/) as ORM to handle database CRUD operations.

## Developing locally

When you have [installed Encore](https://encore.dev/docs/ts/install), you can clone this repo and run it.

## Running locally

```bash
encore run
```

While `encore run` is running, open <http://localhost:9400/> to view Encore's [local developer dashboard](https://encore.dev/docs/ts/observability/dev-dash).

## Check the API

A quick check with curl

```bash
curl 'http://localhost:4000/'
```

## Generate migrations
After you've updated your `schema.ts` file, you can generate migrations by running `npx drizzle-kit generate` in the same directory as `drizzle.config.ts`.

## Deployment

Deploy your application to a staging environment in Encore's free development cloud:

```bash
git add -A .
git commit -m 'Commit message'
git push encore
```

Then head over to the [Cloud Dashboard](https://app.encore.dev) to monitor your deployment and find your production URL.

From there you can also connect your own AWS or GCP account to use for deployment.
