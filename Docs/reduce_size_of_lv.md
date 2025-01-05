# Reducing Size of Running LV

First of all you can't reduce size of a running volume. So you have to boot up from another and then can reduce the size of that volume.
# Step-1 Boot from a Bootable USB

**Boot from a Live CD/USB:** You cannot resize a mounted root volume. Boot into a live environment (e.g., a Linux live USB).
# Step-2 Check the Current State

```bash
sudo vgdisplay
sudo pvdisplay
sudo lvdisplay
```
# Step-3 Shrink the Root Logical Volume

```bash
sudo e2fsck -f /dev/<vg_name>/root
```

Resizing the `root lv` to 100GB

```bash
sudo resize2fs /dev/<vg_name>/root 100G
```

Reduce the Logical Volume

```bash
sudo lvreduce -L 100G /dev/<vg_name>/root
```

# Step-4 Verify Free Space

```bash
sudo vgdisplay <vg_name>
```

Look at `Free PE / Size` if the value is your desired space you want to free then you're done with **Reducing Size** and this free space can be used to create new logical volumes.

[Goto Main](../README.md)
