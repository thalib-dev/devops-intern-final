# Final Assessment Projects ![CI](https://github.com/thalib-dev/devops-intern-final/actions/workflows/ci.yml/badge.svg)
                                                         #Name      : Mohammed Thalib TM
                                                         #Final date: 07-10-2025
# Git Assessment project
  #Steps involved in this projects :
        
         '''
        Step 1 : Open git bash
        Step 2 : make directory using "mkdir dir_name" and 
             Change directory to the created path "cd /path/to/directory"
        Step 3 : Create hello.py file using "vim hello.py"
        Step 4 : Write the Script mentioned below
             Sreipt : " #! /usr/bin/env python3
                        print("Hello, DevOps!") "
        Step 5 : Save the script and exit
        Step 6 : To run the script use " py hello.py "
  
        '''
  #this is a very basic script in python.

  #Screenshots :
  
   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/61cf6182fa6cff9ae76f8ebc5b882045f91acf5c/Git_Project/Screenshots/git.png)

   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/61cf6182fa6cff9ae76f8ebc5b882045f91acf5c/Git_Project/Screenshots/git1.png)

   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/61cf6182fa6cff9ae76f8ebc5b882045f91acf5c/Git_Project/Screenshots/git2.png)
   
x-------------------------------xx-------------------------------xx-------------------------------xx-------------------------------x

# Linux Assessment Project                                                                                        
   #Steps involved in this Project :
      
      '''
        Step 1 : Open git bash
        Step 2 : make directory using "mkdir dir_name" and 
                 Change directory to the created path "cd /path/to/directory"
        Step 3 : Create sytem.sh file using "vim system.sh"
        Step 4 : Write the Script mentioned below
                 Script : " #!/bin/bash
                           echo "Current User: $(whoami)"
                           echo "Date: $(date)"
                           echo "Disk Usage: $(df -h)" "
        Step 5 : Save the script and exit
        Step 6 : To run the script use " ./syetem.sh "
      
      '''

  #This Script is used to get the Current user name, Current date and the Disk usage of this system. 

  #Screenshots :
   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/9b2f9df284fab543de4a2f693964a491826b6d2d/screenshots/linux.png)

   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/9b2f9df284fab543de4a2f693964a491826b6d2d/screenshots/linux%201.png)

   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/9b2f9df284fab543de4a2f693964a491826b6d2d/screenshots/linux%202.png)

   x-------------------------------xx-------------------------------xx-------------------------------xx-------------------------------x

# Docker Assessment Project
   #Steps involved in this Project :
    
     '''
    Step 1 : Open git bash
    Step 2 : make directory using "mkdir dir_name" and 
             Change directory to the created path "cd /path/to/directory"
    Step 3 : Create "Dockerfile" file using "vim Dockerfile"
    Step 4 : Write the commands mentioned below
             commands : " FROM python:3.3-slim
                          WORKDIR /app
                          COPY hello.py /app/
                          CMD ["python", "hello.py"] "
    Step 5 : Save it and exit
    Step 6 : Copy the hello.py to the current directoy
    Step 7 : Make sure you installed docker then run the build command as below
             " docker build -t hello-devops . "
    Step 8 : Use this command to run the docker container " docker run --rm hello-devops "
  
    '''

  #Screenshots :
  ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/938f4f4cda7f6f5875ea268dd0f0dc7f19d06930/Docker_Project/Screenshots/docker.png)

  ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/938f4f4cda7f6f5875ea268dd0f0dc7f19d06930/Docker_Project/Screenshots/docker1.png)

  ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/938f4f4cda7f6f5875ea268dd0f0dc7f19d06930/Docker_Project/Screenshots/docker3.png)

  ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/938f4f4cda7f6f5875ea268dd0f0dc7f19d06930/Docker_Project/Screenshots/docker4.png)
  
x-------------------------------xx-------------------------------xx-------------------------------xx-------------------------------x
# Nomad Assessment Project    
   #Steps involved in this Project :
      
      '''
        Step 1 : Open git bash
        Step 2 : make directory using "mkdir dir_name" and 
                 Change directory to the created path "cd /path/to/directory"
        Step 3 : Create hello.nomad file using "vim hello.nomad"
        Step 4 : Write the Script mentioned below
                 Script : " job "hello" {
                              datacenters = ["dc1"]
                              type = "service"

                              group "hello-group" {
                                task "hello-task" {
                                  driver = "docker"

                                  config {
                                    image = "hello-devops:latest"
                                  }

                                  resources {
                                    cpu    = 100
                                    memory = 64
                                  }
                                }
                             }
                          } "
        Step 5 : Save the script and exit
        Step 6 : To start the nomad agent " nomad agent -dev "
        Step 7 : Open a new terminal to start the nomad job " nomad job run nomad/hello.nomad "
        Step 8 : To check the job status "nomad job status hello"
        
      '''
#Screenshots:
![image alt](https://github.com/thalib-dev/devops-intern-final/blob/5273d02febaf075f6d5398708ec5ef50bc350469/Nomad_Project/Screenshots/nomad.png)
![image alt](https://github.com/thalib-dev/devops-intern-final/blob/5273d02febaf075f6d5398708ec5ef50bc350469/Nomad_Project/Screenshots/nomad1.png)
![image alt](https://github.com/thalib-dev/devops-intern-final/blob/5273d02febaf075f6d5398708ec5ef50bc350469/Nomad_Project/Screenshots/nomad2.png)
![image alt](https://github.com/thalib-dev/devops-intern-final/blob/5273d02febaf075f6d5398708ec5ef50bc350469/Nomad_Project/Screenshots/nomad3.png)
![image alt](https://github.com/thalib-dev/devops-intern-final/blob/5273d02febaf075f6d5398708ec5ef50bc350469/Nomad_Project/Screenshots/nomad4.png)

x-------------------------------xx-------------------------------xx-------------------------------xx-------------------------------x

# Grafana_Loki Assessment Project
   #Steps involved in this Project :
      
      '''
        Step 1 : Create a working directory for monitoring configs
                 mkdir -p ~/monitoring/promtail
                 cd ~/monitoring
        Step 2 : Create Promtail config file
                  " cat > promtail/promtail-docker-config.yaml "
        Step 3 : Start Loki
                  " docker run -d --name=loki -p 3100:3100 grafana/loki:2.9.0 
                    -config.file=/etc/loki/local-config.yaml "
        Step 4 : Start Promtail
                 " docker run -d --name=promtail \
                    -v /var/log:/var/log \
                    -v /var/lib/docker/containers:/var/lib/docker/containers:ro \
                    -v $(pwd)/promtail:/etc/promtail \
                    grafana/promtail:2.9.0 \
                      -config.file=/etc/promtail/promtail-docker-config.yaml "
        Step 5 : Run a test container
                  " docker run --name hello-test --rm -d hello-devops "
        Step 6 : Query logs directly from Loki API
                    " curl "http://localhost:3100/loki/api/v1/query?query={job=\"dockerlogs\"}" "

      
      '''


  #Screenshots :
   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/301a82690585b16e95cf8f06282bc0d354530050/Grafana_Loki_Project/Screenshots/gl.png)

   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/301a82690585b16e95cf8f06282bc0d354530050/Grafana_Loki_Project/Screenshots/gl1.png)

   ![image alt](https://github.com/thalib-dev/devops-intern-final/blob/301a82690585b16e95cf8f06282bc0d354530050/Grafana_Loki_Project/Screenshots/gl2.png)

x-------------------------------xx-------------------------------xx-------------------------------xx-------------------------------x

