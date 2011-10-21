!SLIDE 

# BBQ #

 * <a href="http://benalman.com/projects/jquery-bbq-plugin/">http://benalman.com/projects/jquery-bbq-plugin/</a>
 * Bookmark/history support

!SLIDE

# BBQ functionality #

 * Event listener for when the URL's hash value changes
 * Uses HTML5 hashchange event or adds this feature for older browsers

!SLIDE

 * Treat the hash the same as a request string
 * Ex. #tab=classes&partner=2
 * Retrieve individual params with deparam()
 * Change or add with pushState()


!SLIDE

# Warning #

 * Uses an iframe with IE7 and earlier
 * Stuck on 1.3pre release for over a year
 * Other alternatives may be a better choice - search on Single Page Applications