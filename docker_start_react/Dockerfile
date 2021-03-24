FROM node:15.10.0

WORKDIR /myapp
COPY ["./package.json", "./yarn.lock", "./"]
RUN yarn install

# Add a script to be executed every time the container starts.
COPY entrypoint.sh /usr/bin/
RUN chmod +x /usr/bin/entrypoint.sh
ENTRYPOINT ["entrypoint.sh"]

CMD ["yarn", "start"]
EXPOSE 4000
