## Adding icons

YOU SHOULD ONLY USE ACTUALLY NEEDED ICON FONTS.

1. git clone git@github.com:Nurego/icomoon-rails.git
2. Go to [IcoMoon App](http://icomoon.io/app/)
3. Load our current fonts:  
    Click on the red button "Import icons"
    Choose icomoon.dev.svg file (icomoon-rails/vendor/assets/fonts/icomoon-free/icomoon.dev.svg)
4. Select the fonts you needed, and click 'Font->' button.  
5. Click 'Download' to download your font pack as zip file
6. Update icomoon-free source files:  
     cd icomoon-rails  
     rake update-icomoon NAME=icomoon-free ZIP=~/Downloads/icomoon.zip
7. Commit & Push:  
    git add .  
    git commit -am "[SOME TEXT]"  
    git push git@github.com:Nurego/icomoon-rails.git 
8. Update gem:  
    cd website  
    bundle update --source icomoon-rails
9. Restart server:  
    rails s
 

## License

The assets from [IcoMoon](http://icomoon.io/) free icon pack use CC License [(CC BY-SA 3.0)](http://creativecommons.org/licenses/by-sa/3.0/).

Other parts of gem use MIT license.
