VERSION 0.8

FROM busybox:1.32.0

hello:
    ARG name=world
    COPY globe.txt /globe.txt
    RUN cat /globe.txt
    RUN echo "Hello, $name!" > /hello.txt
    CMD ["cat", "/hello.txt"]
    SAVE ARTIFACT /hello.txt AS LOCAL hello.txt
