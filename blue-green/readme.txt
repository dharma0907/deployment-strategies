

Blue-green:

we deploy both the versions at the same time
v1 and v2

v1 version is for client end-users
v2 is for testing purpose, here we write only deploymwnt file where we don't use service file


once v2 is signed off by testing team then v2 will be roll-out using patch command

kubectl patch service my-app -p '{"spec":{"selector":{"version":v2.0.0"}}}'
