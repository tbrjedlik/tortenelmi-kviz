from node as build

WORKDIR /app

copy . .

run npm i

run npm run build

from nginx as final

copy --from=build /app/dist /usr/share/nginx/html