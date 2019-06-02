FROM node:11
RUN mkdir /home/node/app && chown -R node:node /home/node/app
WORKDIR /home/node/app
COPY package.json *.lock .
RUN npm install 
COPY . .
EXPOSE 3000
CMD ["npm", "start"] # 啟動伺服器 npm run start