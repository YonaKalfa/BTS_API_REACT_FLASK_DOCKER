from node:18-alpine

workdir /app

copy package.json /app/package.json
run npm install

expose 5173

cmd ["npm", "run", "dev", "--", "--host", "0.0.0.0", "--port", "5173"]