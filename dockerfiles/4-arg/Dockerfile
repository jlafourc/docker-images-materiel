FROM debian:9.4

ARG foo

RUN echo $foo $bar

RUN echo ${foo:-default}

ARG bar=baz

RUN echo $bar
