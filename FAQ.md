# Frequently asked questions

Q: MacPorts sucks! Why not use Homebrew?  
A: Ruby is for punks.  All the cool kids use TCL.  Also, my target platform is Mac OS X 10.7 Lion, which requires [MacPorts Support for Legacy OSX Versions](https://github.com/macports/macports-legacy-support).  Tvheadend won't compile on older systems without it.

Q: Where is the hts user home directory?  
A: */opt/local/var/lib/tvheadend* by default.  MacPorts puts home directories for non-interactive users in */opt/local/var* or */opt/local/var/lib*.

Q: That's dumb.  Why?  
A: The MacPorts philosophy is install everything under */opt/local* prefix.  If recordings are saved elsewhere (and they probably should be), the home directory will only contain configuration files.

Q: I don't like it.  How do I uninstall everything?  
A: [See here to completely uninstall MacPorts](https://guide.macports.org/chunked/installing.macports.uninstalling.html).  The following will remove the hts user from your system.

```code
sudo dscl . -delete /Users/hts
sudo dscl . -delete /Groups/hts
```
