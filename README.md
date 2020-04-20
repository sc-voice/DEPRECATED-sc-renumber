# sc-renumber
Scripts to renumber SuttaCentral bilara-data

### Installation
Open a Linux terminal window and change to the directory
where you want to install `scv-bilara`. For example:

```bash
mkdir -p ~/dev
cd ~/dev
```

Now install `sc-renumber`:

```bash
git clone https://github.com/sc-voice/sc-renumber
cd sc-renumber
./scripts/install.sh
```

The installation script has been known to fail if it cannot install 
NodeJS v10.17.0. If you encounter this, install NodeJS v10.17.0 manually
and repeat the installation above.

##### bilara-data
By default, `sc-renumber` works with the `sc-voice/bilara-data` fork of 
[SuttaCentral bilara-data](https://github.com/suttacentral/bilara-data). 
To use `sc-renumber` with any other fork of `bilara-data`, simply clone
the desired repository into the `local` subdirectory before using any scripts. Notice that
any existing bilara-data must be removed.

```
rm -rf local/bilara-data
git clone https://github.com/suttacentral/bilara-data local/bilara-data
```

For those who prefer Git over SSH:

```
rm -rf local/bilara-data
git clone git@github.com:suttacentral/bilara-data local/bilara-data
```

