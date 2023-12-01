FROM node:18

COPY package.json package.json

COPY package-lock.json package-lock.json

RUN npm install

COPY . .

RUN npm run build

CMD ["cp", "-r", "/build/.", "/frontend_static/"]
