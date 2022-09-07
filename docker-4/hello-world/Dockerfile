FROM node:14-alpine

ENV prueba=1234

LABEL manteiner="roxsrossve@gmail.com"
LABEL project=node_app

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000
USER node
CMD ["npm","start"]
#docker build -t node_app:1.0.0 . (si es la misma ruta si nos -f la ruta)//para la costruccion
#ocker run -it -p 3000:3000 node_app:1.0.0