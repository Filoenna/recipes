FROM node:20-alpine
WORKDIR /app
RUN ls -al /app
RUN corepack enable && corepack prepare pnpm@latest --activate
RUN pnpm --version
COPY . .
RUN pnpm install || pnpm install --no-frozen-lockfile && pnpm list
CMD ["pnpm", "run", "dev", "--", "--host"]
