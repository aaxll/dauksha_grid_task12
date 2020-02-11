hub: local physical WIN10
 java -jar selenium-server.jar -role hub

node1: virtual UBUNTU
java -jar selenium-server.jar -role webdriver -hub http://192.168.174.1:4444/grid/register -port 5556

node2: virtual WIN7
java -jar selenium-server.jar -role webdriver -hub http://192.168.174.1:4444/grid/register -port 5557

