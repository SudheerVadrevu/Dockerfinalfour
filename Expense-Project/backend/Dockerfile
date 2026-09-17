FROM node:20
EXPOSE 8080
RUN useradd expense
RUN mkdir /opt/server
RUN chown expense:expense -R /opt/server
WORKDIR /opt/sever/
COPY *.js /opt/sever/
COPY package.json .
RUN npm install
CMD ["node", "index.js"]