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

By Default Qubes (4.01) uses the `C.UTF-8` locale, resulting in Thunderbird formatting dates as `MM/DD/YYYY`.

To utilise the more sensible date formatting of ISO-8601 and format dates as `DD/MM/YYY`, create the following files and restart the Qube once complete.
<!--more-->

### /rw/config/locale.conf

```shell
LANG=en_GB.UTF-8
```

### /rw/config/rc.local

```shell
rm -rf /etc/locale.conf
ln -s /rw/config/locale.conf /etc/locale.conf
localectl
```