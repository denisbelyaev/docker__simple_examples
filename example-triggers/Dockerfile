FROM alpine
MAINTAINER denis <denis@gmail.com>
RUN apk update && apk add nodejs
RUN mkdir app
ENV NODE_ENV production
WORKDIR app
ENTRYPOINT ["node", "app.js"]
ONBUILD ADD . /app
ONBUILD RUN npm install