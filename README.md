# detect-adblocker
You can use this to detect if the ad blocker is enabled on the visitor browser. See the result in action on the [Example][3] page.

## Installation

Using this tool is very simple you only need to place the following before any script tag in your web page as the following:

> **When you use my servers for the ads file I will show one ad per user every 24 hours to support the project. If you don't want to support me you can host the file on your own server.**

    <!--adBlocker detection code - START-->
    <script src="//adblocker.fortiapp.com/ads.js"></script>
    <script>
        (function (i, o, g, r) {
            i[o] = (typeof i[o] == typeof undefined) ? g : r
        })(window, 'adblocker', true, false);
    </script>
    <!--adBlocker detection code - END-->

## Usage

Now you only need to check for adblocker variable in your code

    if (adblocker) {
        // the add blocker is enabled
    }else{
        // ad blocker is not enabled
    }
    
> To see this in action check the example page [Example][3]

## Contributing

I'm will be very happy if any one wants to contribute to this repo


## Credits

I got the idea from an answer on [stackoverflow][1] check it out.
                                                           
                                                           
## License

MIT [http://rem.mit-license.org][2]


[1]: http://stackoverflow.com/a/20505898/5751341
[2]: http://rem.mit-license.org
[3]: http://fortiapp.github.io/detect-adblocker/example.html