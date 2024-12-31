# Steps for installation 

_This guide is only for devices having a658 fingerprint scanners. Thanks to [libfprint team](https://gitlab.freedesktop.org/libfprint) for the drivers._

## Debain based systems

- `apt install fprintd libpam-fprintd`
- `sudo pam-auth-update`
- Check the (aestrik mark should appear) on fingerprint auth
- Download the drivers from this repo *.deb for debian
- `dpkg -i *.deb`
- Restart the device and you will be able to use fingerprint

## Fedora/Redhat systems

- Follow [this](https://gist.github.com/7ka-Hiira/1785df8563ef9fd6138a585bc106d6c5) guide from [7ka-Hiira](https://github.com/7ka-Hiira/)


# References

- Discussion on [libprintf's gitlab](https://gitlab.freedesktop.org/libfprint/libfprint/-/merge_requests/413#note_2256055)