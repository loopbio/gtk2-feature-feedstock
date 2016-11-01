A good conda package for gtk2 is in the "mw" channel. 
It would be best that we do provide it and/or try to make it into conda-forge.

In general, we can use system's gtk2 at runtime.
At the moment this is used a trick to compile our opencv conda package against gtk2,
given that conda-forge's centos image gtk2 does not play well with conda-forge's
newer libpng. As an alternative, we could instruct cmake to use libpng from
the container's centos system. Bother if bothered.
