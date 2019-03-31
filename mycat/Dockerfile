FROM ubuntu
ADD jdk-8u201-linux-x64.tar.gz /usr/local/
ADD Mycat-server-1.6.6.1-release-20181031195535-linux.tar.gz /usr/local/
ENV JAVA_HOME=/usr/local/jdk1.8.0_201
ENV PATH=$JAVA_HOME/bin:$PATH
ENV CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
EXPOSE 8066 9066
VOLUME /usr/local/mycat/conf
VOLUME /usr/local/mycat/logs
CMD ["/usr/local/mycat/bin/mycat", "console"]
