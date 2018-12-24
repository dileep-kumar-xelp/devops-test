FROM mongo

COPY questions.json /questions.json
COPY users.json /users.json
COPY responses.json /responses.json
CMD mongoimport --host mongo --db Devopstest --collection questions --type json --file /questions.json --jsonArray && mongoimport --host mongo --db Devopstest --collection users --type json --file /users.json --jsonArray && mongoimport --host mongo --db Devopstest --collection responses --type json --file /responses.json --jsonArray