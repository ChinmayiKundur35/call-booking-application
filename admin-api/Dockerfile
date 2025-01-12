FROM node:17.9.0-slim
RUN useradd adminapi
WORKDIR /app
RUN chown adminapi /app /home
COPY . .
RUN npm install
EXPOSE 1004
ENV MONGO_URL=""
USER adminapi
CMD ["npm","start"]