# Vue-webpack
A project template for vue.js multiple pages bulid with webpack.

## Node dev
```shell
npm/yarn install      # install

npm run dev           # develop         http://localhost:8001

npm run build         # build           http://localhost:9001
```

## Docker dev

```shell
# Build an image [vue-multi-page] from a Dockerfile
docker build -t vue-multi-page .
npm install --production
docker run -it -v ${PWD}:/usr/src/app -p 8000:8001 --name example  vue-multi-page

# Container {{name}} is running, else docker start {{name}}
docker exec {{name}} npm run start
docker exec {{name}} npm run build

```
