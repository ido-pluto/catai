FROM node:19

RUN npm i -g catai

ARG MODEL_NAME
RUN catai install $MODEL_NAME

ARG VERSION
RUN npm i -g catai@$VERSION

EXPOSE 3000

ENV CATAI_OPEN_IN_BROWSER = false

CMD [ "catai", "serve"]