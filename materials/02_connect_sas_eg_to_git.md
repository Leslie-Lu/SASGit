
# connect sas enterprise guide to git

sas eg supports only the HTTPS to connect to a git server.

**Notes:**

- use [github personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)

- authenticated conection is important for certain operations. These include push and any access to private repositories. The authentication isn't needed for local operations like commit, stage, and even clone.

## setting up a github connection

**before we add profile:**

> first, to define a personal access token

> to cerate a profile in sas eg, select tools->manage git connections. Specify a profile name (ex: GitHub), username (github id), email and persoanl access token.