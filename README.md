# katana-releases

## Supported platforms
  * Ubuntu 18.04

## Ubuntu 18.04 Instructions

Add appache arrow apt repository:
```bash
curl -o /tmp/arrow-keyring.deb https://apache.bintray.com/arrow/ubuntu/apache-arrow-archive-keyring-latest-bionic.deb
sudo apt update
sudo apt install /tmp/arrow-keyring.deb ca-certificates
rm /tmp/arrow-keyring.deb
```

Make sure ssh is installed (ensures at least one MPI supported transport is installed):
```bash
sudo apt update
sudo apt install ssh
```

Download the katana package from [here](#releasepage).

Install katana:
```bash
sudo apt update
sudo apt install ./${package_name}.deb
```
