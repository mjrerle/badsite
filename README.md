# Purpose
[:)](https://www.youtube.com/watch?v=ZB62oaOeqR0)

# Description
**A bad site**
This is an example of a vulnerable site ripe with php/sql injection and several questionable design choices. 

# Challenges
Don't edit the source files (beside the config)
Yes you do have all of the files at your disposal, the challenge is to __fix__ them
Show tables
Get admin
Find/document all of the vulnerabilities

# Configuration

**change lib/config.php to match your local environment**

## Windows
### Option 1 - Using XAMPP and Git Bash
* make a development folder inside of <XAMPP installation folder>\htdocs\
* `cd <XAMP installation folder>/htdocs/<development folder>`
* `git clone https://github.com/mjrerle/badsite`
* edit lib/config.php:
* change public $url_local=''; to `public $url_local = "<path/to/dev/folder>"`
* run xampp
* start apache server
* open web browser goto "localhost:80"

### Option 2 - Using (only) XAMPP
* make a development folder inside of <XAMPP installation folder>\htdocs\
* navigate to <development folder>
* goto https://github.com/mjrerle/badsite
* click on "# releases"
* download source code, save to <XAMP installation folder>\htdocs\<development folder>
* change public $url_local=''; to `public $url_local = "<path/to/dev/folder>"`
* run xampp
* start apache server
* open web browser goto "localhost:80"

### Option 3 - Using CSU public folder and PuTTY
* start PuTTY
* use default settings and enter <username>@<hostname>.cs.colostate.edu under "Host Name or IP Address"
* enter password, say "yes/no" to the prompt
* `mkdir -p public_html/<development folder>`
* `cd public_html/<development folder>`
* `git clone https://github.com/mjrerle/badsite`
* change public $url_public=''; to `public $url_public = "~<username>"`
* run perms.sh (gives appropriate permissions)
* open web browser goto "http://www.cs.colostate.edu/~<username>"

## Linux
### Option 1 - Using XAMPP
* make a development folder inside of <XAMPP installation folder>/htdocs/
* `cd <XAMP installation folder>/htdocs/<development folder>`
* `git clone https://github.com/mjrerle/badsite`
* change public $url_local=''; to `public $url_local = "<path/to/dev/folder>"`
* run xampp
* start apache server
* open web browser goto "localhost:80"

### Option 2 - Using CSU public folder
* `mkdir -p public_html/<development folder>`
* `cd public_html/<development folder>`
* `git clone https://github.com/mjrerle/badsite`
* change public $url_public=''; to `public $url_public = "~<username>"`
* run perms.sh (gives appropriate permissions)
* open web browser goto "http://www.cs.colostate.edu/~<username>"

## Mac
### Option 1 - Using MAMP and git
* make a development folder inside of Applications/<MAMP installation folder>/htdocs/
* `cd Applications/<MAMP installation folder>/htdocs/<development folder>`
* `git clone https://github.com/mjrerle/badsite`
* change public $url_local=''; to `public $url_local = "<path/to/dev/folder>"`
* run mamp
* start apache server
* open web browser goto "localhost:8888"

### Option 2 - Using CSU public folder
* `mkdir -p public_html/<development folder>`
* `cd public_html/<development folder>`
* `git clone https://github.com/mjrerle/badsite`
* change public $url_public=''; to `public $url_public = "~<username>"`
* run perms.sh (gives appropriate permissions)
* open web browser goto "http://www.cs.colostate.edu/~<username>"
