# Getting Started with react-app-docker

This project is a simple app bootstrapped using [Create React App](https://github.com/facebook/create-react-app) running inside a `Docker` container.

## Building the container

Follow the steps outlined below:

### `git clone`

Clone the repo using the command `git clone https://github.com/sainagasrikantham/react-app-docker`

### `docker build`

After you've `cd` into the cloned repo directory, run the following command:\
Build the image using the command (notice the dot `.`) `docker build -t <your-image-name-here> .`

### `docker run`

Once the `docker` image is built you can verify that it exists by using the command:\
`docker images`

Assuming the `build` step went alright, you can run your newly created container with the command:\
`docker run -p 3000:3000 <your-image-name-here>`

Open [http://localhost:3000](http://localhost:3000) to view the app in the browser.

**Note**: We're binding port `3000` to the exposed `3000` port in the Docker container for simplicity, you can
choose whatever port you like in the above command replacing the _first_ value of `3000` example:\
`docker run -p 4000:3000 <your-image-name-here>`

Now, you'd have to go to [http://localhost:4000](http://localhost:4000) to view the results.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
