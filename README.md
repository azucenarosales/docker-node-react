# React
Docker with node and react

# Build Image
$ docker build . -t node

# Create container
$ docker run -ti --net bridge -v $(pwd):/var/www/sites --name react node

# Create new React project
$ docker run --rm -v $(pwd):/var/www/sites create-react-app myapp

# Start npm inside react project
$ docker run --rm -ti -v $(pwd):/var/www/sites node-container npm start
