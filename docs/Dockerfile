FROM ghcr.io/codesmithcloud/bun-builder:latest AS code_builder

WORKDIR /app

# install npm dependencies first, for optimal layer caching
COPY ./package*.json ./
RUN npm install

# do the code build, which will output statis assets to /app/.output/public
COPY ./ ./
RUN npm run build

# copy static assets from code_builder container into /www of the teeny http server
FROM ghcr.io/codesmithcloud/teeny:latest
COPY --from=code_builder /app/.output/public /www
