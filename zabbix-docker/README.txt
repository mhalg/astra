Originally was cloned zabbix-docker project- https://github.com/zabbix/zabbix-docker.git

User following command to setup 3 zabbix server containers:
tar xzvf folders_vars_env.tgz
docker-compose -f docker-compose_v3_alpine_pgsql_latest.yaml up -d
