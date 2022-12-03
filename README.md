# Install-CHROMIUM-ON-PARROT
Install CHROMIUM ON PARROT



root@cyberghazi-vmwarevirtualplatform:/# apt-get install synaptic
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
synaptic is already the newest version (0.90.2).
synaptic set to manually installed.
The following packages were automatically installed and are no longer required:
  figlet insserv libio-pty-perl libipc-run-perl lshw-gtk moreutils startpar sysv-rc
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 530 not upgraded.

Now Menu > Goto System Tools > Synaptic Manager
Choose all chromium packages and install them all by pressing apply.
Now Menu > Internet > Chromium is installed already.

Now Go back to TERMINAL again.

# pluma /etc/chromium.d/default-flags

If these linese are there, then dont change and close the file.

# A set of command line flags that we want to set by default.

# Do not hide any extensions in the about:extensions dialog
export CHROMIUM_FLAGS="$CHROMIUM_FLAGS --show-component-extension-options"

# Enable GPU rasterization.
export CHROMIUM_FLAGS="$CHROMIUM_FLAGS --enable-gpu-rasterization"

# Don't display any warnings about not being the default browser
export CHROMIUM_FLAGS="$CHROMIUM_FLAGS --no-default-browser-check"

# Disable pinging
export CHROMIUM_FLAGS="$CHROMIUM_FLAGS --disable-pings"

# Disable the builtin media router (bug #833477)
export CHROMIUM_FLAGS="$CHROMIUM_FLAGS --media-router=0"

OR

If you see nothing is there then add these line, save and exit this file.
# Do not hide any extensions in the about:extensions dialog
export CHROMIUM_FLAGS="chromium --no-sandbox --user-data-dir"
#"$CHROMIUM_FLAGS --show-component-extension-options"

The End :-)
