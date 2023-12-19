#
# Builds a custom docker image for node-red and openhab
#
FROM nodered/node-red

LABEL maintainer="br1pro" \
      author="br1pro" \
      dockerfile-author="br1pro"

# Install additional "basic" nodes for vsPLC
RUN npm install node-red-contrib-modbus
RUN npm install node-red-node-random
RUN npm install node-red-dashboard

# Copy node-red flow as default
COPY mbm/mbm.json /data/flows.json

# Expose ports
EXPOSE 1880/tcp
EXPOSE 502/tcp
