FROM alpine:latest
LABEL maintainer="wangwenfu228@gmail.com"
ENV LANG=C.UTF-8

# Install cURL
RUN echo -e "https://mirror.tuna.tsinghua.edu.cn/alpine/v3.4/main\n\
https://mirror.tuna.tsinghua.edu.cn/alpine/v3.4/community" > /etc/apk/repositories && \
	apk --update add curl bash openjdk8-jre-base && \
    rm -rf /var/cache/apk/*

# Set environment
ENV JAVA_HOME /usr/lib/jvm/default-jvm
ENV PATH ${PATH}:${JAVA_HOME}/bin

CMD ["java","-version"]