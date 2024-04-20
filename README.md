# Creating a PayTM project from scratch using -


<p> <img src="https://d2eip9sf3oo6c2.cloudfront.net/tags/images/000/001/358/square_480/turbo-logo.png" alt="git" width="80" height="80"/> 

<img src="https://cdn.freelogovectors.net/wp-content/uploads/2022/01/prisma_logo-freelogovectors.net_.png" alt="java" width="80" height="80"/>  </p>

<p><a href="https://www.postgresql.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.iconscout.com/icon/free/png-256/free-postgresql-11-1175122.png" alt="java" width="80" height="80"/> </a>  postgres as DB </p>

<p><a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://w7.pngwing.com/pngs/219/411/png-transparent-docker-logo-kubernetes-microservices-cloud-computing-dockers-logo-text-logo-cloud-computing-thumbnail.png" alt="java" width="80" height="80"/> </a>  Docker for Database </p>

<p><a href="https://recoiljs.org/" target="_blank" rel="noreferrer"> <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTgyFAmQ6DqLk-j-XT_vBCzi7C-J5T3ipkeFC4G8S9qvQ&s" alt="java" width="80" height="80"/> </a>  Recoil for state management </p>

<p><a href="https://next-auth.js.org/" target="_blank" rel="noreferrer"> <img src="https://next-auth.js.org/img/social-media-card.png" alt="java" width="80" height="80"/> </a>  NEXTAuth for authentication </p>


postgres as DB starting in a docker container, Recoil for state management,
NEXTAuth for authentication

## Reason for using TurboRepo-

## Why we need PRISMA-

## How we started POSTGRES in container using network and Volumes

## Need for Rocoil as stateManagement



## What's inside?

This Turborepo includes the following packages/apps:

### Apps and Packages

- `docs`: a [Next.js](https://nextjs.org/) app
- `web`: another [Next.js](https://nextjs.org/) app
- `@repo/ui`: a stub React component library shared by both `web` and `docs` applications
- `@repo/eslint-config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `@repo/typescript-config`: `tsconfig.json`s used throughout the monorepo

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### Utilities

This Turborepo has some additional tools already setup for you:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Prettier](https://prettier.io) for code formatting

### Build

To build all apps and packages, run the following command:

```
cd my-turborepo
pnpm build
```

### Develop

To develop all apps and packages, run the following command:

```
cd my-turborepo
pnpm dev
```

### Remote Caching

Turborepo can use a technique known as [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching) to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can [create one](https://vercel.com/signup), then enter the following commands:

```
cd my-turborepo
npx turbo login
```

This will authenticate the Turborepo CLI with your [Vercel account](https://vercel.com/docs/concepts/personal-accounts/overview).

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

```
npx turbo link
```

## Useful Links

Learn more about the power of Turborepo:

- [Tasks](https://turbo.build/repo/docs/core-concepts/monorepos/running-tasks)
- [Caching](https://turbo.build/repo/docs/core-concepts/caching)
- [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching)
- [Filtering](https://turbo.build/repo/docs/core-concepts/monorepos/filtering)
- [Configuration Options](https://turbo.build/repo/docs/reference/configuration)
- [CLI Usage](https://turbo.build/repo/docs/reference/command-line-reference)
