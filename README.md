# SeguridadUDA-LopezNerpiti
Ejercicio KeyCloak 

Request: 
POST para tokens: http://localhost:8080/auth/realms/Demo-Realm/protocol/openid-connect/token
Datos para entrar al REALM

{
  "name": "keycloack-nodejs-microservice",
  "version": "1.0.0",
  "lockfileVersion": 1,
  "requires": true,
  "dependencies": {
    "@nodelib/fs.scandir": {
      "version": "2.1.5",
      "resolved": "https://registry.npmjs.org/@nodelib/fs.scandir/-/fs.scandir-2.1.5.tgz",
      "integrity": "sha512-vq24Bq3ym5HEQm2NKCr3yXDwjc7vTsEThRDnkp2DK9p1uqLR+DHurm/NOTo0KG7HYHU7eppKZj3MyqYuMBf62g==",
      "optional": true,
      "requires": {
        "@nodelib/fs.stat": "2.0.5",
        "run-parallel": "^1.1.9"
      }
      
      
User GET : http://localhost:3000/test/user

Anonymus GET: http://localhost:3000/test/anonymus

ADMIN GET: http://localhost:3000/test/admin

INFORMACION QUE MANDAMOS:
{
 alg: "RS256",
 typ: "JWT",
 kid: "VaIafKmsfG7lpo5XS2zFlfNui-PCOmQZWy1PUxnQquY"
}.
{
 exp: 1633035550,
 iat: 1633035250,
 jti: "e09efe9d-dfce-4c2f-9964-2083f9405ef1",
 iss: "http://localhost:8080/auth/realms/Demo-Realm",
 aud: "account",
 sub: "88b05f0d-f382-486e-b07b-4b1ad8f988e2",
 typ: "Bearer",
 azp: "nodejs-microservice",
 session_state: "1fb9a036-8743-44fa-9b94-df664cb3ca7f",
 acr: "1",
 allowed-origins: [
  "http://localhost:8000"
 ],
 realm_access: {
  roles: [
   "offline_access",
   "app-admin",
   "default-roles-demo-realm",
   "uma_authorization",
   "app-user"
  ]
 },
 resource_access: {
  nodejs-microservice: {
   roles: [
    "admin",
    "user"
   ]
  },
  account: {
   roles: [
    "manage-account",
    "manage-account-links",
    "view-profile"
   ]
  }
