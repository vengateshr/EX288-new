FROM ubi-micro:latest

ARG BUILDREPO=http://downloads.domain42.example.com/postal-1.0

WORKDIR /opt/app-root

# Download the application binary during build
ADD ${BUILDREPO} /opt/app-root/postal-1.0

USER 0

RUN chmod +x /opt/app-root/postal-1.0

EXPOSE 8080

USER 1001

CMD ["/opt/app-root/postal-1.0"]
