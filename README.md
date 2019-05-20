Secure Gate System - Restu Ibu with PouchDB Nodejs and Express

URL : https:/di.tulis.online
- API : GET POST DELETE 
/daftar /login /users /gates  
----
POST /users -> body = nrp & password
GET /users -> return all users
GET /users/:userid -> return user
DELETE /users/:userid -> delete user

POST /gates -> body = nrp,role, jam_buka & jam_tutup
GET /gates -> return all gates
GET /gates/:gateid -> return gate
DELETE /gates/:gateid -> delete gate

Views :
GET /addgates
GET /login
GET /daftar
GET /home -> Access protected page, login first

POST /login -> body = gate, nrp, pass



how to :
1. install pouchdb, pouchdb-server, pouchdb-find, body-parser,cookie-parser,multer, morgan, all the imported files using npm. \n
(npm install pouchdb pouchdb-server pouchdb-find body-parser)n \n
2. Run index.js, open.your localhost:3000\n
3. You can either try to login first via localhost/masuk OR create the user via register page in localhost/daftar\n
4. try to login, you'll be able to login now using the local database (offline mode)\n
5. run the remote database pouchdb-server ( pouchdb-server --port 3333)\n
6. you'll see the login details in console.\n
