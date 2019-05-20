Secure Gate System - Restu Ibu with PouchDB Nodejs and Express

URL : https://di.tulis.online/

USER

POST /users
body = nrp & password

GET /users 
return all users

GET /users/:userid 
return user

DELETE /users/:userid
delete user


GATES

POST /gates
body = nrp,role, jam_buka & jam_tutup

GET /gates
return all gates

GET /gates/:gateid
return gate

DELETE /gates/:gateid
delete gate


VIEWS

GET /addgates

GET /login

GET /daftar

GET /home
Access protected page, login first


POST /login
body = gate, nrp, pass
