FROM node:9-stretch

# workaround for https://github.com/moby/moby/issues/2259
RUN usermod -m -d /home/homeeup node

# set up required environment and install homeeup https://github.com/kdietrich/homeeup
RUN mkdir -p /home/homeeup/.homeeup
RUN npm install -g homeeup

# start homeeup
USER node
EXPOSE 2001
CMD homeeup
