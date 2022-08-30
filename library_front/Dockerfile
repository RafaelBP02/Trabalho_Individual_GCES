FROM node:latest

ENV NODE_ENV=production

RUN mkdir /library_db

WORKDIR /library_db

COPY package.json .

RUN npm install --production

COPY . .

EXPOSE 3000

CMD [ "node", "src/App.js" ]

ENTRYPOINT ["tail","-f","/dev/null"]