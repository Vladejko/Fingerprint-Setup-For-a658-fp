# Steps for installation 

_This guide is only for devices having a658 fingerprint scanners. Thanks to [libfprint team](https://gitlab.freedesktop.org/libfprint) for the drivers._

## Debain based systems

- `sudo apt install fprintd libpam-fprintd`
- `sudo pam-auth-update`
- Check the (aestrik mark should appear) on fingerprint auth
- Download the drivers from this repo *.deb for debian
- `sudo dpkg -i *.deb`
- Restart the device and you will be able to use fingerprint

## Fedora

- `sudo dnf install fprintd fprintd-pam libfprint`
- `sudo rpm -e --nodeps libfprint `
- Download the drivers from this repo *.rpm for Fedora
- `sudo rpm -i *.rpm`
- Mark the package as dependency so it is not removed
- `sudo dnf mark dependency libfprint-2-2-0:1.94.4+tod1-FT9366_20240627.x86_64`
-  Restart the device and you will be able to use fingerprint

# References

- Discussion on [libprintf's gitlab](https://gitlab.freedesktop.org/libfprint/libfprint/-/merge_requests/413#note_2256055)
