# Nomad Assessment Project    
                                                         #Name: Mohammed Thalib TM
                                                         #date: 01-10-2025
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
