# vicons

## Users

To build the iconset, install inkscape (a free as beer and speech svg editor) and run

    ./generate_kde_icons.sh

in the source directory.

This will create a subdirectory "vicons" which you probably want to symlink
to /usr/share/icons/vicons

*Notice* that it (currently) inherits the breeze icon theme.


## Pros

The icon images are created into a pool and symlinked to their actual name.  
This is automized by alias.txt  
If you believe an existing icon should be used for another action/place/mime
all that's required is to extend the entry in alias.txt (the structure isn't very
complex, but check alias.README in doubt)

## Artists

You're encouraged to extend and improve the icon theme, but to not waste your time,
please stick to some basic

### Design rules
- All icons must be usable on bright and dark backgrounds. No exception.
- Colors are permitted =)
    - However, please use the core breeze colors
    - See https://techbase.kde.org/Projects/Usability/HIG/Color
    - You can download a palette for inkscape [here](http://denilson.sa.nom.br/gimp-palettes/index.html) ([direct link](https://raw.githubusercontent.com/denilsonsa/gimp-palettes/master/palettes/Breeze.gpl))
- Try to stay away from gradients and glosses ;-)
- Icons should be created on a 32x32 px document
- For straight lines, ensure to align to a 2px grid
- For everything that could end up as 22px icon (toolbar actions), at least try to align to a 4px grid
    - In case of an outline, align the inner border, ie. the shape would start at eg. 3px instead of at 4px
- Most icons have a global opacity of 80% to pick the background color.
- Most icons have an outline with 196/256 alpha - this blends between icon and background and lowers aliasing.
- No svgz please, git sucks on binary data. Save as plain, uncompressed svg.
- In doubt, just look at some present icons ;-)