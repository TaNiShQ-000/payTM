# Creating a PayTM project from scratch using -

<p> <img src="https://d2eip9sf3oo6c2.cloudfront.net/tags/images/000/001/358/square_480/turbo-logo.png" alt="git" width="80" height="80"/> TurboRepo for file structuring </p>

<p><img src="https://cdn.freelogovectors.net/wp-content/uploads/2022/01/prisma_logo-freelogovectors.net_.png" alt="java" width="80" height="80"/> Prisma for ORM </p>

<p><a href="https://www.postgresql.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.iconscout.com/icon/free/png-256/free-postgresql-11-1175122.png" alt="java" width="80" height="80"/> </a>  postgres as DB </p>

<p><a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://w7.pngwing.com/pngs/219/411/png-transparent-docker-logo-kubernetes-microservices-cloud-computing-dockers-logo-text-logo-cloud-computing-thumbnail.png" alt="java" width="80" height="80"/> </a>  Docker for Database </p>

<p><a href="https://recoiljs.org/" target="_blank" rel="noreferrer"> <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTgyFAmQ6DqLk-j-XT_vBCzi7C-J5T3ipkeFC4G8S9qvQ&s" alt="java" width="80" height="80"/> </a>  Recoil for state management </p>

<p><a href="https://next-auth.js.org/" target="_blank" rel="noreferrer"> <img src="https://next-auth.js.org/img/social-media-card.png" alt="java" width="80" height="80"/> </a>  NEXTAuth for authentication </p>


postgres as DB starting in a docker container, Recoil for state management,
NEXTAuth for authentication

## Reason for using TurboRepo-

-> Monorepo Management allows you to manage multiple packages or modules in a single repository, making easily managed codebase.
-> Dependency Management simplifies managing dependencies between different parts of the app ensuring consistent changesy.
-> Build Optimization build system optimizes the build process by detecting changes and only rebuilding the changed parts of your app, reducing build times.
-> Code Sharing code gets easily shared between different modules or packages in your app promoting consistency.


## Why we need PRISMA-


Type-Safe Queries: Prisma provides a type-safe API for building database queries, which helps prevent runtime errors related to type mismatches.
Declarative Schema: With Prisma, you define your database schema using a declarative language (Prisma Schema), which is then used to generate the necessary database tables and relationships.
Automatic Migrations: Prisma can automatically generate and apply database migrations based on changes to your Prisma Schema, making it easier to manage database changes in your application.
Database Agnostic: Prisma supports multiple databases (such as PostgreSQL, MySQL, and SQLite), allowing you to switch databases easily without changing your application code.
Performance: Prisma's query engine is highly optimized for performance, which can lead to faster database queries and improved application performance.


## How we started POSTGRES in container using network and Volumes

Containerizing PostgreSQL with networks and volumes provides a secure and reliable way to deploy and manage the database, ensuring data integrity and ease of management. This approach is well-suited for modern application deployments where scalability, security, and data persistence are key considerations
Containerization has become a popular approach for deploying applications When containerizing a database like PostgreSQL, it's important to consider how to manage the database's network and volumes to ensure security and data integrity.

Why Use Networks?
Isolation: By using a dedicated network for the PostgreSQL container, we can isolate it from other containers and the host machine, reducing the risk of unauthorized access.
Communication: The network allows communication between containers in the same network, enabling our application container to connect to the PostgreSQL container.

Why Use Volumes?
Data Persistence: Volumes ensure that data stored in the database persists even if the container is stopped, restarted, or deleted, ensuring data integrity.
Backup and Restore: Volumes make it easy to back up and restore the database by simply copying the volume data, simplifying database management.


## Need for Rocoil as stateManagement


State management libraries like Recoil are useful in frontend development for several reasons:

Centralized State: Recoil allows you to manage your application's state in a centralized location, making it easier to access and update state across different components.
Complex State Logic: For applications with complex state logic, Recoil provides tools like selectors, atoms, and derived states to manage state in a more organized and efficient manner.
Performance Optimization: Recoil is designed to optimize performance by minimizing unnecessary re-renders. It uses a dependency graph to track which components are affected by state changes and only re-renders those components.
Asynchronous State: Recoil supports asynchronous state updates, making it easier to manage asynchronous data fetching and updates in your application.


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
