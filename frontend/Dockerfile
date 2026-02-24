# -------- Stage 1: Build Angular App --------
FROM node:18-alpine AS build

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .
RUN npm run build --prod


# -------- Stage 2: Serve with Nginx --------
FROM nginx:alpine

# Copy Angular build output
COPY --from=build /app/dist/angular-15-crud/ /usr/share/nginx/html

# Copy custom nginx config for SPA routing
COPY nginx.conf /etc/nginx/conf.d/default.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]