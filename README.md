# docker-node
nodejs


     docker image build -t angular . 


     docker run -it -p 4200:4200 -p 49153:49153  --name ANGULAR -v   $(pwd)/app:/usr/src/app angular bash


Serving your app

     ng serve --host=0.0.0.0 --poll 1