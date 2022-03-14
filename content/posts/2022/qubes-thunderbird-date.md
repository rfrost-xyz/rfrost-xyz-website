+++
author = "Richard Frost"
title = "ISO-8601 in Thunderbird and Qubes"
description = "A brief description of Hugo Shortcodes"
date = "2022-03-14"
tags = [
	"qubes",
	"thunderbird"
]
+++

Thunderbird pulls the its date format from `/etc/locale.conf`. By Default Qubes (4.01) uses the `C.UTF-8` locale, resulting in Thunderbird formatting dates as MM/DD/YYYY. Create the following files, and restart the Qube once complete.
<!--more-->

### /rw/config/locale.conf

```shell
LANG=en_GB.UTF-8
```

### /rw/config/rc.local

```shell
# Date format
rm -rf /etc/locale.conf
ln -s /rw/config/locale.conf /etc/locale.conf
localectl
```