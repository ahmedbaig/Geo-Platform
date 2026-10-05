# geo-platform

Shared geospatial infrastructure in the home lab, used by every geo project: PostGIS, an imagery catalogue, tile serving and a map viewer.

Deployed alongside [proxmox](https://github.com/ahmedbaig/proxmox) (Ansible roles there once it runs).

## Phases

1. **PostGIS** on the existing Postgres (CT 112).
2. **Imagery catalogue:** a STAC catalogue and storage for cloud-optimised GeoTIFFs.
3. **Tiles and viewer:** raster tiles from the imagery, vector tiles from PostGIS, and a MapLibre viewer template projects can publish to.
4. **Operate:** capacity (the Proxmox thin pool is tight), backups, monitoring.
