FROM alpine

MAINTAINER penglong_feng "feng237533@126.com"

ADD ./proxy /bin/
ADD ./README /

RUN chmod 755 /bin/proxy

EXPOSE 18120

CMD ["proxy","-proto","ssocks","-timeout","10","-addr","0.0.0.0:18120","-password","google321654"]

