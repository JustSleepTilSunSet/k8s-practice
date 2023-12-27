`* tag is for necessary parameter.`

#### This is a hello-world service.  
- Run the command,that will be built.  
    - ` npx express-generator`
        - ref: [express build project](https://expressjs.com/en/starter/generator.html)
    
- How to build pod?
    1. Create docker image:
        - docker build  -t [*imagename]:[*version] .
            - thats a standard image name format.
        - docker run -p [app port]:[app port] --name [containername] -d [*imagename] [command]
            - [docker run learn more](https://docs.docker.com/engine/reference/commandline/run/)
        - [Docker learn more](https://docs.docker.com/engine/reference/run/)
    2. minikube start
    3. deploy: 
    - minikube kubectl -- apply -f [*podyaml]
        - f for `file`.
    - minikube kubectl -- logs [*podname]
