[Docker hub link](https://hub.docker.com/repository/docker/lukxsx/pakastimenhallinta)

To run:
```docker run -v $(pwd)/tietokanta.db:/PakastimenHallinta/application/tietokanta.db --rm -d -p 5000:5000 lukxsx/pakastimenhallinta```
That mounts the database file to the local file. 
