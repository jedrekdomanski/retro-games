FROM alpine:latest
RUN mkdir prince
RUN apk update && apk upgrade && apk add build-base && apk --no-cache add \
  tzdata \
  expat \
  bash \
  git \
  make \
  npm \
  curl \
  py-pip \
  libstdc++ \
  ca-certificates \
  libffi-dev \
  linux-headers \
  file \
  libxml2-dev \
  nodejs \
  gmp-dev \
  musl \
  gcompat \
  libucontext-dev

RUN cd prince && git clone https://github.com/oklemenz/PrinceJS.git
WORKDIR /prince/PrinceJS
RUN npm install
CMD [ "npm","start" ]
