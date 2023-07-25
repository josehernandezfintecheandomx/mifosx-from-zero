# MifosX



## Getting started

1. Ensure you have the following installed in your system:

    [`docker`](https://www.docker.com/)

    [`docker compose`](https://docs.docker.com/compose/)


2. Clone the project locally into your system.
```
git clone https://github.com/josehernandezfintecheandomx/mifosx-from-zero.git
```

3. `cd` into project root directory and make sure you are on the master branch.


4. Review the `.env` file to set the right `TIMEZONE` and database credentials `DB_USER` and `DB_PASS` environment values used in the init process.


5. Run the docker compose command to start the services
```
docker compose up -d
```

To review the logs of these services run the next command
```
docker compose logs -f
```

If you want to see only the logs for a specific service run the next command to get the service details
```
docker ps
```

Then you can use the docker container identifier or name, ie:
```
docker logs -f mifosx-mifos-back-server-1
```


To stop the services run the next command
```
docker compose stop
```

6. Once time the three service are up and running you can use MifosX using a web browser in the URL `http://localhost` 

