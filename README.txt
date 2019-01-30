Tested on Lightroom Classic CC 8.1 for MacOS

The following hijacks layout template for 13x11-blurb (large scape) and use
that to fit the 16x12 canvas. Two steps:

1) Change the canvas size for the layout_template_sizes.lua file
2) Change the page sizes for each layout. Only the size of each page have
changed, the individual layout are most certainly off (except for a few full
size ones)

cd /Applications/Adobe\ Lightroom\ Classic\ CC/Adobe\ Lightroom\ Classic\ CC.app/Contents/PlugIns/layout_toolkit.agmodule/Contents/Resources

sudo mv layout_template_sizes.lua layout_template_sizes.lua.orignal
sudo ln -s /Users/xhuang/lightroom/layout_template_sizes.lua .

sudo mv 13x11-blurb 13x11-blurb.original
sudo ln -sf /Users/xhuang/lightroom/16x12-blurb 13x11-blurb


3) Following allows you to save "Custom Pages". The idea is to allow you to
start from a slightly messy template (due to canvas size change), visually fix
it, and then save it as custom page for you.

cd /Users/xhuang/Library/Application\ Support/Adobe/Lightroom/Layout\ Templates/13x11-blurb/
sudo mv custompages13x11-blurb custompages13x11-blurb.orginal
sudo ln -sf /Users/xhuang/lightroom/custompages16x12-blurb custompages13x11-blurb 

