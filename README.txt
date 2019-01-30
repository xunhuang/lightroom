setup


cd /Applications/Adobe\ Lightroom\ Classic\ CC/Adobe\ Lightroom\ Classic\ CC.app/Contents/PlugIns/layout_toolkit.agmodule/Contents/Resources

sudo mv layout_template_sizes.lua layout_template_sizes.lua.orignal
sudo ln -s /Users/xhuang/lightroom/layout_template_sizes.lua .

sudo mv 13x11-blurb 13x11-blurb.original
sudo ln -sf /Users/xhuang/lightroom/16x12-blurb 13x11-blurb


cd /Users/xhuang/Library/Application\ Support/Adobe/Lightroom/Layout\ Templates/13x11-blurb/
sudo mv custompages13x11-blurb custompages13x11-blurb.orginal
sudo ln -sf /Users/xhuang/lightroom/custompages16x12-blurb custompages13x11-blurb 



