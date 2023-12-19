# MBMaster
A ModbusTCP Master for vsPLC

## Docker version
Build the image and call it "mbmaster" in your running docker environment using the following command:
- `docker build https://github.com/br1pro/MBMaster.git#:docker -t mbmaster`

Run the docker image using the following command:
- `docker run --rm -p 1880:1880 -p 502:502 --name mbm mbmaster`

docker build https://github.com/br1pro/MBMaster.git#:docker -t mbmaster
