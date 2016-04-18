# docker-automate

Step 1: setup public repo automated build
  - Create a github public repo with simple dockerfile with echo "Hello Docker!"
  - goto github repo settings > webhook > services > add docker
  - goto docker hub page, log in
  - click create > create automated build
  - Test: push commits to github repo, watch docker hub automated build repo page > build details
