FROM amazoncorretto:11-alpine-full
WORKDIR /app
RUN ["apk", "add", "maven"]
RUN ["ln", "-nsf", "/usr/lib/jvm/java-11-amazon-corretto", "/usr/lib/jvm/default-jvm"]
RUN ["mkdir", "-p", "/var/log/jslice"]
RUN ln -sf /dev/stdout /var/log/jslice/app.0.log \
  && ln -sf /dev/stderr /var/log/jslice/app.0.log