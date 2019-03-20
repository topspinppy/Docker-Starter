FROM mongo:3.4.7


ENV MONGO_INITDB_ROOT_USERNAME admin
ENV MONGO_INITDB_ROOT_PASSWORD 1234
ENV MONGO_INITDB_DATABASE shoppers

ADD ./data/shoppers.js /docker-entrypoint-initdb.d


#docker exec -it mongodb sh
#mongo -u "admin" -p "1234" --authenticationDatabase "admin"

#show database

#use [   ]

#db.products.find();