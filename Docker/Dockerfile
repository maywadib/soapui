FROM pottava/groovy
MAINTAINER Rao version:0.3
LABEL java.version 1.8 groovy.version 2.4 ant.version 1.9.4 hermes.version 1.14
COPY . /opt
RUN cd /opt && ls
RUN mv /opt/soapui-settings.xml /root && chmod +x /opt/*sh && cp /opt/*sh /app && cp /opt/demo*xml /app && cp /opt/build.xml /app
ENV SOAPUI_HOME /opt/soapui-4.5.1 ANT_HOME /opt/apache-ant-1.9.4 HERMES_HOME /opt/HermesJMS CLASSPATH /opt/apache-ant-1.9.4/lib RESULTS /tmp/Results                 
ENV PATH "${SOAPUI_HOME}/bin:${ANT_HOME}/bin:${HERMES_HOME}/bin:${PATH}"                                                                                             
ENTRYPOINT /app/entry-point.sh                                                                                                                                       
CMD /opt/soapui-4.5.1/HelloWS-soapui-project.xml                                               