This project does not include all the files needed for the project. I recommend pulling from wazauh github.
DO NOT pull a clone as it wont have the config. Download a zip from one of the last source releases.
The rest of the information needed is provided in their README.




## .env.manager example

INDEXER_URL=https://wazuh.indexer:9200

INDEXER_USERNAME=admin

INDEXER_PASSWORD=# make password (You also have to change password in config see documentation)

FILEBEAT_SSL_VERIFICATION_MODE=full

SSL_CERTIFICATE_AUTHORITIES=/etc/ssl/root-ca.pem

SSL_CERTIFICATE=/etc/ssl/filebeat.pem

SSL_KEY=/etc/ssl/filebeat.key

API_USERNAME=wazuh-wui

API_PASSWORD=# make password (You also have to change password in config see documentation)


## .env.dashboard example

INDEXER_USERNAME=admin

INDEXER_PASSWORD=# make password

WAZUH_API_URL=https://wazuh.manager

DASHBOARD_USERNAME=kibanaserver

DASHBOARD_PASSWORD=# make password (need to change in config also)

API_USERNAME=wazuh-wui

API_PASSWORD=# make password
