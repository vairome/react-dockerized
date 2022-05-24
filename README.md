
# Docker Image with a React Js App and Nginx server

This is an image which contains an a React App which is mounted on an ngnix server, which has port 80 released to run the static website.

In addition, this image is linked to a GitHub Actions that updates the static content of the website which triggers on any change push or pull request events from the master branch. It also contains a gitHubb Actions workflow to build and push a docker image tho Docker Hub, updating the tags to maintain previous version of the image.

![Nginx](https://download.logo.wine/logo/Nginx/Nginx-Logo.wine.png)

## How does the github actions works?

It has three jobs, when a change is pushed to the master branch, either by direct push or by pull request, the action runs a job to cancel any previous build, the second job is testing the code with a linter function and the last job is for login to Docker Hub, and push the image to a repository, with a function to rename tags automatically to maintain previuos images.

## 🚀 Quick reference

•	Maintained by: Byron Murillo

•	Where go to get help: https://github.com/vairome/react-dockerized/issues


## Supported tags and respective Dockerfile Links

•	Latest

# How to use this image

## Pull and build a container from the image

The first step is pull the image from docker hub.

``$ docker pull vairome/react-dockerized-ci-cd``

The next step is run the image in an interactive mode, specifying to use port 80

``$ docker run -it -p 80:80 --name [name or your image] vairome/react-dockerized-ci-cd``

To finish we only verify in http://localhost:80/ to visualize the react application working.

## License

[MIT](https://choosealicense.com/licenses/mit/)


