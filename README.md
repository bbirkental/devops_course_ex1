# devops_course_ex1
In first task I wrote Dockerfile that based on nginx.
It copy HTML file into it and expose it on port 80 and activate nginx as a web server.
I build the Image :
docker build -t image_name:tag
and run the container
docker run -it --rm -d -p 8080:80 --name ex1 image_name
Then I open the browser and browse localhost port 8080 to see the HTML file running by the container.

<img width="464" alt="docker_run_screen_shot" src="https://github.com/user-attachments/assets/ca1738ab-2a84-484e-9709-f5c074bc5042">


In second task I wrote docker-compose.yaml that build the Dockerfile from first task and run it on port 8080
and also run redis image as a container.
I build the docker-compose:
docker-compose build
And run the containers:
docker-compose up
Then by typing docker ps I saw both containers running:

<img width="912" alt="docker_compose_screen_shot" src="https://github.com/user-attachments/assets/bb8559f3-68da-4c37-8dbb-829f30284a0a">


