# oracle 11.2.0.2

./buildContainerImage.sh -x -v 11.2.0.2

docker run --name oracle-11.2.0.2 --shm-size=1g -p 1521:1521 -p 8080:8080 -e ORACLE_PWD=Passw0rd123 -v /home/asmryz/ORCL-11g/oradata:/u01/app/oracle/oradata oracle/database:11.2.0.2-xe
