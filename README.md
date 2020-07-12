# snippets
Random JavaScript/Typescript snippets that's not big enough to be a package

## - HapiJs
```ts
export function routerGroup(namespace: string, routes: Hapi.ServerRoute[]) {
  return routes.map((r) => {
    r.path = namespace + r.path
    return r
  })
}
```
