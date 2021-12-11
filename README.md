# Usage of docker-compose-create-react-app

git clone git@github.com:sonatine726/docker-compose-create-react-app.git .

docker compose up

cd .\docker_start_react\
cp * ..\myapp\
cd ..
rm -d docker_start_react
cd .\myapp\

docker compose up -d
