Spring CRUD with JNDI in Spring Tool Suite

JDBC Connection is different for this project,because in other projects server credentials are visible to all users having code.
So we are using different method for JDBC Connection.
CODE:
	<Resource
    name="jdbc/usersdb"
    auth="Container"
    type="javax.sql.DataSource"
    maxActive="100"
    maxIdle="30"
    maxWait="10000"
    driverClassName="com.mysql.cj.jdbc.Driver"
    url="jdbc:mysql://localhost:3307/usersdb"
    username="root"
    password=""
    />

Include this code in context.xml file in Tomcat server.