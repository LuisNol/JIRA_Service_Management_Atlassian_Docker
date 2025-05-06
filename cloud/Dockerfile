FROM atlassian/jira-software:latest

# Descarga el conector JDBC de MySQL
RUN curl -L -o /opt/atlassian/jira/lib/mysql-connector-java.jar https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-8.0.30.tar.gz && \
    tar -xvf /opt/atlassian/jira/lib/mysql-connector-java.jar -C /opt/atlassian/jira/lib/ --strip-components=1

# Establecer el directorio de trabajo para Jira
WORKDIR /opt/atlassian/jira

# Exponer el puerto de Jira
EXPOSE 8080
