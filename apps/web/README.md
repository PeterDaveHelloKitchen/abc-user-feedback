# ABC User Feedback Frontend

ABC User Feedback Frontend is the web browser application that provides the beautiful admin UI. The client is built with NextJS, React Query, React Hook Form, Tailwind css, MUI, and many more.

## Setup

ABC User Feedback is using a mono-repo with multiple packages. To initialize all the packages on a local development environment, follow the [Getting Started With Local Development](/README.md#getting-started-with-local-development) section to do that in a few quick steps.

## Useful Targets

You can find a full list of targets in the [package.json](./package.json) file.

### `dev`

Runs the app in development mode.

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

```
yarn dev
```

> **Note**
> In order to run web properly, ui packages need to be built by the
> `yarn build:ui` command in root directory or `yarn turbo run @ufb/ui#build` command in any directory.

### `generate-api-type`

Generate api type using open api specification. This command can run after running on server. The type file is generated in `src/types/api.type.ts`

```
yarn generate-api-type
```

### `lint`

Performs a linting check using ESLint.

```
yarn lint
```

### `format`

Performs a formatting code using Prettier.

```
yarn format
```

### `build`

Builds the app. The distributable is expored to the `.next` folder.

```
yarn build
```

## Environment Variables

| Environment              | Description                                             | Default Value                                |
| ------------------------ | ------------------------------------------------------- | -------------------------------------------- |
| NEXT_PUBLIC_API_BASE_URL | api base url in client side (ex. http://localhost:4000) |                                              |
| NEXT_PUBLIC_MAX_DAYS     | query maximum days                                      | 90                                           |
| API_BASE_URL             | api base url in server side                             |                                              |
| SESSION_PASSWORD         | session password                                        | complex_password_at_least_32_characters_long |

## Learn More

To learn NextJS, check out the [NextJS documentation](https://nextjs.org/).
