These scripts install TileMill and a stack of related services:

* TileMill
* Nginx (making TileMill accessible on port 80, with basic password auth)
* PostGIS (for loading OpenStreetMap data into)
* osm2pgsql (loads the OpenStreetMap data)
* Scripts to manage loading OSM data and refresh it with minimal downtime

```
sudo apt-get -y install git
git clone https://github.com/stevage/tilemill-server
cd tilemill-server

# Optionally, edit tm-settings

nohup ./install.sh &
```

When done, TileMill is accessible on port 80: http://myserver
