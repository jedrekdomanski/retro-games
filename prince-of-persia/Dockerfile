FROM ubuntu:latest
RUN mkdir prince
RUN apt-get update && apt-get install -y git npm
RUN cd prince && git clone https://github.com/oklemenz/PrinceJS.git
WORKDIR /prince/PrinceJS
RUN npm install
CMD [ "npm","start" ]
