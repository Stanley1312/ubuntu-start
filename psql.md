# Insatll PostgreSQl on Ubuntu

### Step 1 - Installing PostgreSQL
```
sudo apt update
sudo apt install postgresql postgresql-contrib
```

### Step 2 - Using PostgreSQl Roles and Databases

Switch over to the **postgres** account on your server by typing:
```
sudo -i -u postgres
```
You can now acess a Postgres prompt immediately by typing
```
psql
```
Exit out the PostgreSQL prompt by typing
```
postgres=# \q
```

## Accessing a Postgres Prompt Without Switching Accounts
You can also run the command you’d like with the postgres account directly with **sudo**

```
sudo -u postgres psql
```



# REF
* [How To Install and Use PostgreSQL on Ubuntu 18.04](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04)
