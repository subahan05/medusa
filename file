Dockerize Medusa App  file:

FROM node:18

WORKDIR /app
COPY . .
RUN pnpm install && pnpm build

WORKDIR /app/.medusa/server
RUN pnpm install
CMD pnpm predeploy && pnpm start
