# Step 1
FROM node AS build
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build

# Step 2
FROM nginx:alpine
COPY --from=build /app/dist/exos-angular /usr/share/nginx/html
COPY --from=build /app/dist/exos-angular/browser/ /usr/share/nginx/html
EXPOSE 80