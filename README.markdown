## Setup

Clone into ~/config as 'shared'. This contains your shared system config. 

Create ~/config/local/bashrc and a new local repository in that directory. This contains your custom config for this system.

Quit textmate.

Symbolically link textmate's custom bundles directory:

    $ ln -s ~/config/shared/tm_bundles ~/Library/Application\ Support/TextMate/Bundles

(If you have bundles already in that directory, you should move the ones you want over to the tm_bundles directory, and remove the Bundles directory.)

Reload bundles:

    $ Bundles > Bundle Editor > Reload Bundles, in TextMate

To install more bundles, clone them into the tm_bundles directory, e.g.

    $ cd ~/bin/tm_bundles
    $ git clone git://github.com/rspec/rspec-tmbundle.git RSpec.tmbundle
    
Symbolically link textmate's custom plugins directory:

    $ ln -s ~/config/shared/tm_plugins ~/Library/Application\ Support/TextMate/PlugIns
    
(If you have plugins already in that directory, you should move the ones you want over to the tm_plugins directory, and remove the PlugIns directory.)

To install more plugins, move the .tmplugin file (directory) into the tm_plugins directory, e.g.    