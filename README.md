# docker-automate

Step 1: Setup public repo automated build
  - Create a github public repo with Dockerfile
  - goto github repo settings > webhook > services > add docker
  - goto docker hub page, log in
  - click create > create automated build
Step 2: Create Image and Push to docker hub
Step 3: Automate build starts
  - push commits to github repo, watch docker hub automated build repo page > build details
