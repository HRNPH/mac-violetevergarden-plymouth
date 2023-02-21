# Origin
forked from https://github.com/fathyar/mac-plymouth

A macOS-like boot screen theme for Plymouth
customized to violet evergarden theme

## Installation
for fedora you can follow in this article
https://fedoramagazine.org/howto-change-the-plymouth-theme/

1. Clone this repo and then `cd` to it.

        $ git clone https://github.com/HRNPH/mac-violetevergarden-plymouth/ && cd mac-violetevergarden-plymouth
        
2. Copy **mac-violetevergarden** folder to `/usr/share/plymouth/themes` directory and `cd` to there.

        $ sudo cp -r mac /usr/share/plymouth/themes && cd /usr/share/plymouth/themes

3. Run the command below.
        
        $ sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/mac-violetevergarden-plymouth/mac-violetevergarden.plymouth 100
        
4. And then run:
        
        $ sudo update-alternatives --config default.plymouth
        
   to choose and set the default theme.

5. Finally, run:
        
        $ sudo update-initramfs -u

