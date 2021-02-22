# Insatll PostgreSQl on Ubuntu

### Step 1 - Installing PostgreSQL
```
sudo apt update
sudo apt install postgresql postgresql-contrib
```

### Step 2 - Using PostgreSQl Roles and Databases

Switch over to the **postgres** account on your server by typing:
```
sudo -u -u postgres
```
You can now acess a Postgres prompt immediately by typing
```
psql
```
Exit out the PostgreSQL prompt by typing
```
postgres=# \q
```

# REF
* [How To Install and Use PostgreSQL on Ubuntu 18.04](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04)
