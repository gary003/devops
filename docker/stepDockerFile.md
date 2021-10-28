## 1 create your dockerFile

`touch DockerFile`

## 2 build file

## 3 run your file with docker command

# Create an image from a docker file

docker image build -t <dockerHub_username>/<nameWanted> .

- The dot at the end represent the dockerFile in the current directory

# push image to dockerHub

docker push <imageName>
if probleme occur during this because of authentication, do -- docker login
