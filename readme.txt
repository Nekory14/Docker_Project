# Access to the project's path

# Commands to run

# Exercise 1 - Java SE

docker build -t docker_javase .

docker run docker_javase

# Exercise 2 - Angular

docker build -t docker_angular .

docker run -p 8080:80 docker_angular

# Access in the web browser to http://localhost:8080

# I reused the ExosAngular exercise