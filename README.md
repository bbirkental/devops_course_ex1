# devops_course_ex1
in first task I wrote Dockerfile that based on nginx.
It copy HTML file into it and expose it on port 80 and activate nginx as a web server.
I build the Image :
docker build -t image_name:tag
and run the container
docker run -it --rm -d -p 8080:80 --name ex1 image_name
Then I open the browser and browse localhost port 8080 to see the HTML file running by the container.
<img width="511" alt="docker_run_screen_shot" src="https://github.com/user-attachments/assets/e52e96c4-8427-46f2-9156-d31e870e9413">

