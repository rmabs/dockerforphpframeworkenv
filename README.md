# dockerforphpframeworkenv
docker for php environment using apache mysql for all php frameworks

**Followings are instructions to follow** <br>
pull the repo  <br>
go to your working directory  <br>
create a new folder (this will be working directory of your new project so name it accordingly) <br>
paste Dockerfile and docker-compose.yml file inside this newly created folder (Dockerfile and docker-compose.yml which you pulled from this repo) <br>
create new foler "db" in this newly created folder <br>
now install Docker desktop from official website of docker <br>
open cmd (like git bash etc)  <br>
type following commands  <br>
**docker compose build** <br>
after above command you wait untill it finishes  <br>
type this new command  <br>
**docker compose up -d** <br>
wait untill above command finishes <br>
your new containers are up and working (if all went without any error)  <br>
now inside this directory paste your project if you have created one already or if you want to create new using compose use following commands <br>
**docker ps**  <br>
it will show list of containers you have up and running it must show folliwing containers  <br>
container for phpMyAdmin container for mysql and a container for php-apache  <br>
now see the column NAME for row with IMAGE = php-apache (or something similar) and copy that name it will be used for executing commands inside container <br>
now type following command to get into container (php-apache) and execute commands accordingly  <br>
**docker exec container-name-you-copied-from-above-steps bash -c "command 1; command anything like; compose install; composer update; ls;"**
 <br>
  <br>
  **NOTE**
if you want to install more extensions for php, thn follow online guide of docker php for more extensions installation in docker php its very easy, 
enjoy :) 
#withoutlaravelsaildocker
#dockerforyii2
#dockerforwordpress
#dockerforcodeigniter


