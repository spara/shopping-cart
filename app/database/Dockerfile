FROM mongo:latest

WORKDIR /app
COPY ./data/* ./
EXPOSE 27017
RUN ["chmod", "+x", "init.sh"]
CMD ./init.sh
# CMD ["mongoimport", "--db", "cart", "--collection", "products", "--file", "products.json", "--jsonArray"]