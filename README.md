# Vite Usage

`@vue/cli 5.0.4` was used to create a standard client-side Vue application. There were minimal changes to move the initial components to more closely mimic the Vite example (`script setup` syntax) in addition to adding `"vue/setup-compiler-macros": true` to the eslint `env` object.

# Local Development

## Vue/Webpack (Via Vue CLI)

- Run `npm ci`
- Run `npm run vue-cli:serve`
- Go to `http://localhost:8080/`

![Vite Local Build](./docs/local-build-vite.png)

## Vue/Vite

- Run `npm ci`
- Run `npm run vue-cli:serve`
- Go to `http://localhost:3000/`

![Vue CLI Local Build](./docs/local-build-vue-cli.png)

## Comparison

Over the course of 5 local builds:

| Tool    | Run 1  | Run 2  | Run 3  | Run 4  | Run 5  | Average | Diff     |
|---------|--------|--------|--------|--------|--------|---------|----------|
| Webpack | 4311ms | 2486ms | 2266ms | 2268ms | 1968ms | 2659.8  | 0        |
| Vite    | 471ms  | 271ms  | 257ms  | 237ms  | 271ms  | 301.4   | +782.48% |

Using Webpack as our baseline, Vite blows it out of the water when it comes to build speed. On average, Vite is `782.48%` faster than Webpack.
# Technology

- [Vue CLI](https://cli.vuejs.org/)
- [Vite](https://vitejs.dev/)

# References

- [Vite Documention: Slow Server Start](https://vitejs.dev/guide/why.html#slow-server-start)
- [How Does Vite Work](https://harlanzw.com/blog/how-the-heck-does-vite-work/)
- [Next Generation Frontend Tooling With ViteJS](https://www.youtube.com/watch?v=UJypSr8IhKY)
