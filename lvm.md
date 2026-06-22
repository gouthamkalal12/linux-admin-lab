# Linux LVM (Logical Volume Manager)

## Check Disks

```bash
lsblk
```

## Check Physical Volumes

```bash
pvs
```

## Check Volume Groups

```bash
vgs
```

## Check Logical Volumes

```bash
lvs
```

## Create Physical Volume

```bash
pvcreate /dev/sdb
```

## Create Volume Group

```bash
vgcreate vgdata /dev/sdb
```

## Create Logical Volume

```bash
lvcreate -L 5G -n lvdata vgdata
```

## Format Filesystem

```bash
mkfs.xfs /dev/vgdata/lvdata
```

## Extend Logical Volume

```bash
lvextend -L +2G /dev/vgdata/lvdata
```

## Grow XFS Filesystem

```bash
xfs_growfs /mountpoint
```
