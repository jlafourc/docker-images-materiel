FROM node:10.13.0-stretch

LABEL type="cktl.app"
LABEL "cktl.release"="2018.4.10"

RUN apt-get update && apt-get install -y curl
RUN npm install http-server -g
RUN echo "<html><body>Miniserver du séminaire</body></html>" > /root/index.html

EXPOSE 8080

HEALTHCHECK --interval=20s --timeout=1s \
  CMD curl -f http://localhost:8080/ || exit 1

CMD http-server /root
