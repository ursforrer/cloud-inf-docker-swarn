FROM node:8.2
ADD code /home/service/code
WORKDIR /home/service/code
RUN useradd -s /bin/bash service
RUN chown -R service:service /home/service
USER service
RUN npm install
EXPOSE 5000
CMD [ "npm", "start" ]
