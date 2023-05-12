# pihole-unbound-docker

A docker setup designed to easily setup both pi-hole and unbound at once.

## Installation

1. Pull this repository.
2. Open the `docker-compose.yml` file and set your time zone and web ui password.
3. Run `docker-compose up -d` to start this container.
4. Set your devices DNS servers to the IP address of the host the docker container is running on.
5. (optional but may be required) If DNS does not function properly, you may need to set Settings > DNS > Interface settings > Permit all origins.

## Configuration

I recommend setting any local DNS records in pi-hole instead of unbound, but if you must set them in unbound, see [here](unbound/conf/README.md)