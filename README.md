# jenkins-slave-jnlp
jenkins-slave-jnlp for ecs cluster


http://IP-ADDRESS:8080/jnlpJars/slave.jar


java -jar slave.jar -jnlpUrl http://IP-ADDRESS:8080/computer/slave-2/slave-agent.jnlp -secret 73c6126abb466061df02ff8c2dc137b10a65bff9f6d9ddb84e2c17ba1327f619 &>/dev/null &

curl http://localhost:3141? | grep -oPm1 "(?<=<status>)[^<]+"

status=$(curl http://localhost:3141 | grep -oP '(?<=<status>).*(?=</status)')
