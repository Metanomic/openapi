# Metanomic APi Specifications

This project defines the specifications and API contracts that the Metanomic Projects should follow.

## Why?

We need a common design and communication language to describe the architecture and assert the delivered features.

## Technologies in Use

- 📝 OpenAPI as the defacto Specification language
- 🔀 Combine all files with [APIDevTools/swagger-cli](https://github.com/APIDevTools/swagger-cli).
- ✅ Validate and lint the OpenAPI document with [stoplight/spectral](https://github.com/stoplight/spectral).
- ✨ Publish reference docs with [redocly/redoc](https://github.com/Redocly/redoc) & GitHub Pages.
- 🚀 Generate various language-specific contracts with [openapitools/openapi-generator-cli](https://github.com/OpenAPITools/openapi-generator)

## Getting started

### Requirements

- Node.js (16 or latest)
- npm (8.1.2 or latest)

### Installation

1. Clone the repository.

   ```sh
   git clone git@github.com:Metanomic/openapi.gi
   ```

2. Install the project dependencies.

   ```sh
   npm install
   ```

3. Edit `openapi.yaml` for the high-level documentation. If you’re not familiar with the OpenAPI Specification, read [Getting started with OAS](https://swagger.io/solutions/getting-started-with-oas/) first.

## Useful commands

The project will build, lint, and preview the OpenAPI document from the terminal, with the following commands:

### Build

The command bundles the spec as one `.yaml` file.

```sh
npm run build
```

The minified document is stored in `_build/openapi.yaml`.

### Test

The command checks if the document follows the OpenAPI 3.0 Specification.

```sh
npm test
```

### Preview

The command builds a docs site so that you can view the rendering on your local browser.

```sh
npm run serve
```

The server starts on [http://127.0.0.1:8080](http://127.0.0.1:8080).

The site is generated with [ReDoc](https://github.com/Redocly/redoc).
