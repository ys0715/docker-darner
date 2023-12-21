# docker-darner
git clone https://github.com/ys0715/docker-darner.git 

cd docker-darner 
 
tar -zxvf darner.tar.gz

cat darner.tar | docker import - darner

docker build -t darner .

docker run -d --restart=always --name=darner --net=host darner
