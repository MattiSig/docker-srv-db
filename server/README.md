docker build --tag=web-server .

docker run -p 3000:3000 -v c:/range/raf-isl/server:/home/node/code -v /home/node/code/node_modules web-server

// docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres

docker run -d -p 5432:5432 -v postgres-data:/var/lib/postgresql/data --name postgres1 postgres