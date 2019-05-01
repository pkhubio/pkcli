# How to easily manage command line access to multiple databases

## Run the examples

Type:  

`docker-compose up -d`

Then run the bash container:  

`docker-compose run bash`

### Aliases

```bash

echo "alias datadb=\"PGPASSWORD=S7QzuwsGM2Se3qCA psql -h datadb -U root test\"">> ~/.bashrc
echo "alias appdb=\"PGPASSWORD=S7QzuwsGM2Se3qCA psql -h datadb -U root test\"" >> ~/.bashrc

source ~/.bashrc

```

## Build the docker images

`./build.sh`


The above command will also try to push the image to the `pkhub/multidbs` repo.  
