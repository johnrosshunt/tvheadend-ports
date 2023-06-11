# tvheadend-ports

MacPorts software packages for tvheadend

## Super Quick Start

- Clone this repository
- Add the repository path to your sources.conf

```code
file:///path/to/tvheadend-ports
rsync://rsync.macports.org/macports/release/tarballs/ports.tar [default]
```

- Add the following lines to your variants.conf

```code
+perl5_34
+python311
+nonfree
```

- Update your MacPorts tree
- See available tvheadend options
- Build tvheadend with desired features (+adds/-subtracts a feature)

```code
sudo port -v selfupdate
port variants tvheadend
sudo port -v install tvheadend +addmuxes +native_cpu +nonfree +superuser +tv_grab_file +xmltv
```

## What Doesn't Work

- Dedicated hardware such as DVB cards
- Video hardware acceleration
- Apple Silicon
- PowerPC 😂

## Tested MacOS versions

- Mac OS X 10.7 Lion (with minimal pain & suffering)
- MacOS 10.15 Catalina
- MacOS 12.2 Monterey (No M1 support yet; x86_64 runs but not really tested)

## Builds successfully but untested

- Mac OS X 10.6 Snow Leopard (with moderate pain & suffering)
- Mac OS X 10.5 Leopard (with much pain & suffering)

## Caveat Emptor

This project is in it's early stages. Please be patient.  Hopefuly, more info soon.
