# docker-automate

Make sure docker daemon is running in your project directory:
eval "$(docker-machine env default)"

Pro tip: add this line to your bash_profile so it runs on all bash sessions

Step 1: Create && Build Image

  - Create Dockerfile
  - `docker build -t <docker-automate> .``
  - List all your docker images: `docker images`
  - `docker run <docker-automate>`

Step 2: Setup public repo automated build

  - Create a github public repo
  - Goto github repo settings > webhook > services > add docker
  - Goto docker hub page, log in
  - Click create > create automated build
  - Link to your github repo

Step 3: Tag/Push image to docker hub repo

  - `docker images`
  - `docker tag <Image ID> <Docker Hub account name>/<Image name>:latest`
  - `docker login --username=<Docker Hub Username>`
  - Prompt with password login in terminal
  - `docker push <Docker Hub account name>/<Image name>`

Step 4: Automate build starts

  - Push commits to github repo, watch docker hub Repo page > build details Tab
