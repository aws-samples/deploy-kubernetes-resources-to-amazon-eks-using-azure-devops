FROM busybox:latest
ENV PORT=3080
HEALTHCHECK CMD nc -z localhost $PORT
# Create a basic webserver and run it until the container is stopped
CMD echo "httpd started" && trap "exit 0;" TERM INT; httpd -v -p $PORT -h /www -f & wait