
# Docker Image with a React Js App and Nginx server

This is an image which contains an a React App which is mounted on an ngnix server, which has port 80 released to run the static website.

In addition, this image is linked to a GitHub Actions that updates the static content of the website which triggers on any change push or pull request events from the master branch.

![Nginx](https://download.logo.wine/logo/Nginx/Nginx-Logo.wine.png)

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

License (MIT)
=====================

Copyright © `2022` 

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the “Software”), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.





## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

