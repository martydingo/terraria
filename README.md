# terraria

## Storage

### ZFS Creation 

```bash

zfs create storage/static-volumes/dingo.zone/terraria.dingo.zone

zfs create storage/static-volumes/dingo.zone/terraria.dingo.zone/the-enclosure-of-cats.terraria.dingo.zone

zfs create storage/static-volumes/dingo.zone/terraria.dingo.zone/the-enclosure-of-cats.terraria.dingo.zone/config

zfs create storage/static-volumes/dingo.zone/terraria.dingo.zone/the-enclosure-of-cats.terraria.dingo.zone/logs

zfs create storage/static-volumes/dingo.zone/terraria.dingo.zone/the-enclosure-of-cats.terraria.dingo.zone/worlds
```

### NFS Exports

```
## terraria.dingo.zone

# NFS Export for the-enclosure-of-cats.terraria.dingo.zone/config
/storage/static-volumes/dingo.zone/terraria.dingo.zone/the-enclosure-of-cats.terraria.dingo.zone/config 10.0.0.0/14(rw,async,no_root_squash,no_wdelay,no_subtree_check)

# NFS Export for the-enclosure-of-cats.terraria.dingo.zone/logs
/storage/static-volumes/dingo.zone/terraria.dingo.zone/the-enclosure-of-cats.terraria.dingo.zone/logs 10.0.0.0/14(rw,async,no_root_squash,no_wdelay,no_subtree_check)

# NFS Export for the-enclosure-of-cats.terraria.dingo.zone/worlds
/storage/static-volumes/dingo.zone/terraria.dingo.zone/the-enclosure-of-cats.terraria.dingo.zone/worlds 10.0.0.0/14(rw,async,no_root_squash,no_wdelay,no_subtree_check)

```