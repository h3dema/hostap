# Extras

On *Ubuntu 18.04 LTS*, to compile the hostapd code, you need to install the dependencies and also make the config file.


```
cd hostapd
cp depconfig .config
```

In this repository there is already a __.config__ file. Check it out to see what we have enabled.
We need also to install the __libnl__ library, using

```
sudo apt-get install libnl-3-200 libnl-3-dev
sudo apt-get install libnl-genl-3-dev

```

To compile, run

```
cd hostapd
make -j4
```

