CMS for school students + a web3 wallet that they can use to pay for coffee

like the calendar will also show like upcoming classes

1 FE, 1 BE, 3 MPC{multi-party communication}

level 1
Web2 parts:

Web2 backend
- init a turbo-repo
- create a be app
- add express
- create a db
- add schema
- finish auth
- add middleware
- finish calendar
- wallet

level 2
Web2 Frontend

Web3 pvt key in db

Web3 implement mpc


courseToggle.tsx: pass the context api, you will need to update the code

later update a notion calendar

so level 1, level 2 will be done

level 3 - mpc private key infra
0. create schema for mpc
1. Admin fe and be
    a. email them their creds
    b. talk to 3 mpc servers and make them generate a pvt key for the user
    c. send the user some sol
2. create be for mpc server(mpc_beta)
3. add send_sol ep(pb)
4. show the user history of txns(pb)


run both backend and mcp-backend

on localhost:3000

test on /user/signup

```json
{
    "email":"nalin@oriental.ac.in",
    "password":"123random",
    "phone":"1234567890"
}
```

/user/signin
```json
{
    "email":"nalin@oriental.ac.in",
"password":"123random"
}
    ```

/user/send
```json
{
    to:"[pub_key]",
    amount:100
}
```
