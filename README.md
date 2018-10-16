# Shamash [![CircleCI](https://circleci.com/gh/rutebanken/shamash/tree/master.svg?style=svg&circle-token=03cc220760321b30f01b19c6edb8692b21234e05)](https://circleci.com/gh/rutebanken/shamash/tree/master)

An in-browser IDE for exploring GraphQL.

## Build the app

```
npm run build
```
or
```
yarn build
```

## Run the app

### Run build against localhost

```
npm start
```
or
```
yarn start
```

### Run build against test

```
npm run dev-bundle
```


## Configuration

We use convict.js for config. Set environment variables `GRAPHQL_URL`
and `SERVICE_NAME` in order to override default configuration of these
endpoints. E.g.

```
  GRAPHQL_URL=http://localhost:8090/graphql SERVICE_NAME=Stoppestedsregisteret npm start
```

Optional environment variable `ENDPOINTBASE` overrides namespace for client including slash. Full example:

```
SERVICE_NAME=Stoppestedsregisteret ENDPOINTBASE=/admin/shamash/ GRAPHQL_URL=https://api-test.entur.org/stop_places/1.0/graphql npm start
```
