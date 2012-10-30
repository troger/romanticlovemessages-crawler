# romanticlovemessages-crawler

## Overview

This scripts crawls the given URL from [romanticlovemessages](http://www.romanticlovemessages.com/) to extract messages and post them to the specified SosMessage API URL.

Sample usage:

    ./romanticlovemessages-crawler.rb -u http://www.romanticlovemessages.com/cat/flirty -s http://localhost:3000 -c 4f6a4f80744e34609b3c8127

The crawler will try itself all the available URLs: flirty1.htm, flirty2.htm, ... until it found a 404 page.

Full options:

    Usage: romanticlovemessages-crawler.rb [options]
    -u, --messages-url URL           The romanticlovemessages category url
    -s, --sosmessage-url URL         The SosMessage API url
    -c, --category-id CATEGORY_ID    The category id where to post the messages
    -m, --max-characters MAX         MAX characters of the message
    -n, --dry-run                    Don't actually post the messages, only display them
    -h, --help                       Display this screen
