FROM Node:20.0 
RUN useradd expense 
EXPOSE 8080
RUN mkdir -p /opt/server 
RUN chown -R epense:expense /opt/server
WORKDIR /opt/server
COPY package.json . 
COPY *.js  .
RUN npm install
CMD [ "npm","/app/index.js" ]