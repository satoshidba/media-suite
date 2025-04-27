# Media-Suite

Media Suite is a collection of tools and services designed to manage and process media files efficiently. This project leverages Docker Compose for easy deployment and management of services, I am personally using this as a stack in Portainer

Heavily derived from https://github.com/navilg/media-stack

## Prerequisites
- Docker version 28.0.1 or later
- Docker compose version v2.33.1 or later

## Configuration

Requires environment variables passed in where appropriate, some VPN providers will differ but this works for me

- OVPN_PATH - full path to a valid .ovpn file with your configuration, this must be available to the VPN container
- OPENVPN_USER - OpenVPN user
- OPENVPN_PASS - Password for OpenVPN user
- MEDIA_MNT - Shared media location available to all containers, mine is a network share mounted to the docker host
- SONARR_STATIC_CONTAINER_IP - IP address in your private docker network, this is to enable services that use the VPN to be able to locally access
- RADARR_STATIC_CONTAINER_IP - IP address in your private docker network, this is to enable services that use the VPN to be able to locally access
- READARR_STATIC_CONTAINER_IP - IP address in your private docker network, this is to enable services that use the VPN to be able to locally access
- LIDARR_STATIC_CONTAINER_IP - IP address in your private docker network, this is to enable services that use the VPN to be able to locally access
- PUID - Process ID user 
- PGID - Process ID group
- TZ - Timezone to be used
- RECOMMENDARR_URL - This is the URL used for validation when connecting to the service

## License

This project is licensed under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.
