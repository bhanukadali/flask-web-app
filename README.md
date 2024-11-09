
<h1>Process</h1>
<h2>Create an Ec2 server  with ubuntu operating system </h2> 
<h2>Install the required package and tools like python flask, docker, ansible </h2>
<h2>In order to  see the webapplication  result we need to  enbale the port number 5000 in the security  group and access by  using its **ipv4 ip:5000**</h2>



**problems Faced while implemenatation**

<h3>DOCKER socker root  while buding the image by placing the  sudo in front of the build command   the error is going to resloved.</h3>
<h3>IN ansible  i faced the connection issue to the  ec2 machine</h3> 
<h3>IN Githubaction, ansible automation task faced a error.</h3>



 sudo apt-get update
    2  ssh -i "webkey1.pem" ubuntu@ec2-35-154-177-238.ap-south-1.compute.amazonaws.com
    3  sudo -i
    4  sudo apt-get update
    5  sudo apt install python3 python3-pip -y
    6  sudo apt install python3-venv -y
    7  mkdir myproject
    8  cd myproject
    9  python3 -m venv venv
   10  source venv/bin/activate
   11  pip install Flask
   12  vi app.py
   13  python app.py
   14  python app.py &
   15  ls
   16  vi Dockerfile
   17  vi requirements.txt
   18  docker build -t flask_helloworld:123 .
   19  cd 
   20  # Add Docker's official GPG key:
   21  sudo apt-get update
   22  sudo apt-get install ca-certificates curl
   23  sudo install -m 0755 -d /etc/apt/keyrings
   24  sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
   25  sudo chmod a+r /etc/apt/keyrings/docker.asc
   26  # Add the repository to Apt sources:
   27  echo   "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
   28    $(. /etc/os-release && echo "$VERSION_CODENAME") stable" |   sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
   29  sudo apt-get update
   30  sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   31  sudo docker run hello-world
   32  cd myproject/
   33  docker build -t flask_helloworld:123 .
   34  sudo docker build -t flask_helloworld:123 .
   35  docker image ls
   36  sudo docker image ls
   37  sudo docker run -p 5000:5000 flask_helloworld:123
   38  ps -aux|grep flask
   39  ps -aux|grep python
   40  kill -9 3266
   41  sudo docker run -p 5000:5000 flask_helloworld:123
   42  docker ps
   43  sudo docker ps
   44  docker run -p 5000:5000 flask-app
   45  docker run -p 5000:5000 flask_helloworld:123
   46  sudo docker run -p 5000:5000 flask_helloworld:123
   47  vi app.py 
   48  sudo docker run -p 5000:5000 flask_helloworld:123
   49  vi requirements.txt 
   50  sudo docker run -p 5000:5000 flask_helloworld:123
   51  pip install -r requirements.txt
   52  sudo docker run -p 5000:5000 flask_helloworld:123
   53  pip install werkzeug==1.0.1
   54  sudo docker run -p 5000:5000 flask_helloworld:123
   55  vi requirements.txt 
   56  sudo docker build -t flask_helloworld:123 .
   57  vi requirements.txt 
   58  docker ps
   59  sudo docker ps
   60  sudo docker run -p 5000:5000 flask_helloworld:123
   61  sudo docker ps
   62  sudo docker image ls
   63  docker login
   64  docker login -u ravinadh -p
   65  docker login -u ravinadh 
   66  sudo image ks
   67  sudo image ls
   68  sudo  docker image ls
   69  docker tag ravinadh/webserver:flask_helloworld
   70  docker tag flask_helloworld:123 ravinadh/webserver 
   71  sudo docker tag flask_helloworld:123 ravinadh/webserver 
   72  sudo  docker image ls
   73  sudo docker tag flask_helloworld:123 ravinadh/webserver:flask_helloworldimage 
   74  sudo  docker image ls
   75  docker push ravinadh/webserver:flask_helloworldimage 
   76  sudo docker push ravinadh/webserver:flask_helloworldimage 
   77  docker login
   78  sudo docker push ravinadh/webserver:flask_helloworldimage 
   79  sudo docker image ls
   80  docker tag flask_helloworld:123 ravinadh/testing:flaskimage
   81  sudo docker tag flask_helloworld:123 ravinadh/testing:flaskimage
   82  sudo docker push  ravinadh/testing:flaskimage
   83  docker logout
   84  docker login -u ravinadh
   85  sudo docker push  ravinadh/testing:flaskimage
   86  sudo docker image ls
   87  sudo docker push ravinadh/testing:flaskimage  --force
   88  sudo docker push ravinadh/testing:flaskimage 
   89  cd ..
   90  sudo apt update
   91  sudo apt install -y software-properties-common
   92  sudo add-apt-repository --yes --update ppa:ansible/ansible
   93  sudo apt install ansible
   94  vi docker_container.yml
   95  sudo usermod -aG docker $USER
   96  sudo chmod 666 /var/run/docker.sock
   97  docker run hello-world
   98  docker login -u heeddatalabs
   99  docker image ls
  100  docker tag heeddatalabs/dev176 flask_helloworld:123
  101  docker tag  flask_helloworld:123  heeeddatalabs/dev176:flask
  102  docker push heeeddatalabs/dev176:flask
  103  sudo  systemctl restart docker
  104  docker lohout
  105  docker logout
  106  docker login -u ravinadh
  107  sudo docker push ravinadh/testing:flaskimage
  108  docker login -u ravinadh
  109  sudo docker push  ravinadh/testing:flaskimage
  110  sudo docker tag flask_helloworld:123 ravinadh/testing:flaskimage
  111  docker push avinadh/testing:flaskimage
  112  docker push ravinadh/testing:flaskimage
  113  mkdir ansible-playbooks
  114  cd ansible-playbooks
  115  vi deploy_docker.yml
  116  ansible --version
  117  vi inventory.ini 
  118  /home/ravi/Downloads/webkey1.pem
  119  cd ..
  120  pwd
  121  ls
  122  ls -lrt
  123  pwd
  124  cd ansible-playbooks/
  125  ls
  126  vi deploy_docker.yml 
  127  cd ..
  128  ls
