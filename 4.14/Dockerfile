FROM atlassian/bitbucket-server:4.14

# install mysql-connector
RUN curl -Ls                "https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.41.tar.gz" | tar -xz --directory "${BITBUCKET_INSTALL_DIR}/lib" --strip-components=1 --no-same-owner "mysql-connector-java-5.1.41/mysql-connector-java-5.1.41-bin.jar"

# hack
COPY atlassian-extras-decoder-v2-3.3.0.jar ${BITBUCKET_INSTALL_DIR}/atlassian-bitbucket/WEB-INF/lib/
COPY atlassian-extras-legacy-3.3.0.jar ${BITBUCKET_INSTALL_DIR}/atlassian-bitbucket/WEB-INF/lib/