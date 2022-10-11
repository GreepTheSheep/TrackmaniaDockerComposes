# TrackmaniaDockerComposes
Docker Compose files with Trackmania server with any Server Controllers

## How To Use

1) Download this repo as .zip file (Recommended)
2) Edit configuration files on the UserData directory
    - Copy `Config/dedicated_cfg.default.txt` to `Config/dedicated_cfg.txt` or any else
    - **Don't forget to set `xmlrpc_allowremote` to `True` else server controllers cannot connect to the Trackmania server**
    - Copy `Maps/MatchSettings/example.txt` to `Maps/MatchSettings/tracklist.txt` or any else
    - Don't forget to add tracks to the `Maps` directory using https://trackmania.exchange
3) Edit your .env file to match with your desired settings
4) On Linux, don't forget to enable write access for others to all folders if not enabled
    - `chmod o+w . -R`
5) On this folder, run `docker compose -f [YOUR COMPOSE FILE] up`

## Credits

- [Evo](https://github.com/evotm) for managing the [Trackmania](https://github.com/EvoTM/docker-trackmania) and the [EvoSC](https://github.com/EvoTM/docker-evosc) Docker images
- Myself (Greep) for managing the [PyPlanet](https://github.com/GreepTheSheep/docker-pyplanet) image