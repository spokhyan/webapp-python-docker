# webapp-python-docker

docker run -it ubuntu bash 
# run apt-get command before install 
apt-get update 
apt-get install -y python3

apt-get install python3-pip
pip install flask

cat > /opt/app.py

cd /opt

FLASK_APP=app.py flask run --host=0.0.0.0

docker build . -t spokhyan/webapp-python-docker

# shows details of container in json format
docker inspect <first few letter of container id> 0a03c3c




