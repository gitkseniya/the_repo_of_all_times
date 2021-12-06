Steps to set up docker   

``docker images``  - to see all docker images already available   
``docker rmi yes-host-domain:latest`` - remove unnecessary docker images   
``docker build --tag helloworld:python .``     - build docker image.  
``docker run --rm -p 9090:8080 -e PORT=8080 helloworld:python`` - run docker image on localhost. Use 9090 that listens to 8080 that is set up in main.py.   
``export GOOGLE_APPLICATION_CREDENTIALS="/Users/kseniya/Downloads/some_key.json"``       - export token for permitted export operation.   
``docker push us-west3-docker.pkg.dev/dataautomationserver/circle-ci-containers/flask-das:latest``  - push docker image up to google cloud docker service.   
 ``gcloud run deploy --region=us-west3  --image=us-west3-docker.pkg.dev/dataautomationserver/circle-ci-containers/helloworld:latest --min-instances=1 --max-instances=4  --project=dataautomationserver``    - deploy docker image.  If successfully ran, open the new service url and make call.  
 
   
   
   
   ``docker build -t land_mgmt:fifth . `` - also build docker image  
   ``docker run -p 5000:5000 land_mgmt:fifth`` - run docker on localhost with default 5000  
   ``docker stop $(docker ps -aq)`` - stop docker  
   ``echo y | docker system prune`` - clean cache    
   ``docker run -p 3000:9000 -e FLASK_RUN_PORT=9000 land_mgmt:fifth`` - web should be 3000, listening to internal 9000  
