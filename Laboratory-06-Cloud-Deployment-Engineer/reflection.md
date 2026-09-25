# Mission 6 Reflection

## 1. How does writing a docker-compose.yml file make a cloud engineer's job 
   easier compared to manually typing commands?
Writing a docker-compose.yml file makes a cloud engineer's job easier because 
it stores all the container settings in one file. Instead of manually typing 
many docker run commands, the engineer can use one command like 
docker-compose up -d to start the whole application and its services. It also 
makes the setup easier to repeat, share, and manage.

## 2. What happens if you make an indentation error (like using a Tab instead 
   of Spaces) in a YAML file?
If you make an indentation error in a YAML file, Docker Compose may not be 
able to read the file and will show a YAML syntax or parsing error. YAML uses 
spaces for indentation, so using a Tab or incorrect spacing can cause the 
configuration to fail.

## 3. Why did we use environment variables (like MYSQL_PASSWORD) in the 
   Compose file?
We used environment variables like MYSQL_PASSWORD to store configuration 
values separately from the application code. This makes the Compose file 
easier to manage and allows passwords and other settings to be changed 
without modifying the code itself.

## 4. How did it feel to deploy a fully functional enterprise cloud storage 
   system (Nextcloud) in just a few minutes?
It felt exciting and surprising to see a fully functional cloud storage 
system like Nextcloud running in just a few minutes. It showed me how Docker 
and Docker Compose can make deploying complex applications much faster and 
easier than setting everything up manually.

## 5. How has your understanding of Cloud Computing evolved since Mission 1?
Since Mission 1, my understanding of Cloud Computing has improved because I 
now understand how cloud services, containers, storage, and databases work 
together. I also learned that tools like Docker and Docker Compose make it 
easier to deploy and manage applications. Before, I mostly saw cloud 
computing as online storage, but now I understand that it also involves 
infrastructure, networking, applications, and services.
