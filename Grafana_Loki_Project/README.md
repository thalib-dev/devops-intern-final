# Grafana_Loki Assessment Project
                                                         #Name: Mohammed Thalib TM
                                                         #date: 07-10-2025
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
