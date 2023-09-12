# FROM node:14 as builder
FROM node:14

WORKDIR /frontend/m5-react-app

COPY ./m5-react-app/package*.json ./
# COPY package*.json ./

RUN npm install

COPY . .

# RUN npm run build

# FROM nginx:alpine

# COPY --from=builder /frontend/build /usr/share/nginx/html

EXPOSE 3001

CMD ["npm", "start"]
