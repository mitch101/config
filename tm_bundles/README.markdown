Clone this repo to ~/bin, and symbolically link the textmate custom bundles directory there:

    $ ln -s ~/bin/tm_bundles ~/Library/Application\ Support/TextMate/Bundles

(If you have bundles already in that directory, you should move the ones you want over to the tm_bundles directory, and remove the Bundles directory.)

Reload bundles:

    $ Bundles > Bundle Editor > Reload Bundles, in TextMate

To install more bundles, clone them into the tm_bundles directory, e.g.

    $ cd ~/bin/tm_bundles
    $ git clone git://github.com/rspec/rspec-tmbundle.git RSpec.tmbundle