# docker-node
nodejs


     docker image build -t angular . 


     docker run -it --name ANGULAR -v   $(pwd)/app:/usr/src/app -p 4200:4200 -p 49153:49153 angular