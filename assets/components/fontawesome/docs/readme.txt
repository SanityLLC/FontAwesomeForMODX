--------------------
FontAwesomeForMODX
--------------------

Version: 4.3.0
Since: April 30, 2015
Author: Shawn Wilkerson <shawn@shawnwilkerson.com>

Details
A reusable means to load Font Awesome from MaxCDN (Bootstrap), CloudFlare, or local storage with the intent of being used with HTML5 sites.

Versions can also be specified in the Template at the `FontAwesome4` chunk call.

Properties
cdn The repository to use: bootstrap, maxcdn, cloudflare, local
fontAwesomeVersion The version of Font Awesome to use. Defaults to 4.3.0

Example Chunk Calls
[[$FontAwesome4:strip?cdn=`cloudflare`&fontAwesomeVersion=`4.3.0`]] Uses Cloudflare CDN and version 4.30.
[[$FontAwesome4]] Uses the local filesystem and version 4.3.0
[[$FontAwesome4:strip?cdn=`maxcdn`&fontAwesomeVersion=`4.1.0`]] Uses MaxCDN and an older version.
[[$FontAwesome4:strip?cdn=`bootstrap`]] Loads version 4.3.0 from the MaxCDN (default for Bootstrap

Update Collision Disclaimer
The MODX Revolution Font Awesome package will overwrite itself during updates, which is intended. Updates to the vendor's product should transparently pass to the site when updated.

Major product releases will have a corresponding include chunk, which will be automatically upgraded to the latest version.
Font Awesome 4.x.x will use the tpl.Fa4.include as the base.
Upon release of Font Awesome 5.x.x the package will include a tpl.fA5.include and corresponding chunk to be included in templates.

Links
Vendor: [Font Awesome] (http://fortawesome.github.io/Font-Awesome/)