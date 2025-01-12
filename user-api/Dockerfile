FROM node:17.9.0-slim
RUN useradd userapi
WORKDIR /app
RUN chown userapi /app /home
COPY . .
RUN npm install
EXPOSE 1004
ENV MONGO_URL=""
ENV ADMIN_URL=""
USER userapi
CMD ["npm","start"]
