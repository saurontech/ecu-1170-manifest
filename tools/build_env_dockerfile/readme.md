build command:

docker build --no-cache \
  --build-arg USER_ID=$(id -u) \
  --build-arg GROUP_ID=$(id -g) \
  -f ./Dockerfile.yoctoenv \
  -t yocto-env:24.04 \
  .
