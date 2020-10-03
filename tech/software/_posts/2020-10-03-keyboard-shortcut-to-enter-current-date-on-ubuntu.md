---
layout: post
title:  Keyboard Shortcut to Enter Current Date on Ubuntu
author: Adam Berg
---

Tired of typing and remembering the date all the time? Find out how to use Autokey to insert today's date with a keyboard shortcut.

<!--more-->

## [AutoKey](https://github.com/autokey/autokey)

### Installation

Either search for AutoKey in the Ubuntu Software store or run `sudo apt-get install autokey-gtk` from the terminal

### Running

You can run from the terminal with `autokey-gtk` or search for it in the application launcher under AutoKey.

### Configuration

Autokey provides some sample scripts and Insert Date is one of them. By default it doesn't have a hotkey registered and outputs in an overly verbose format "Sat Oct  3 10:58:48 PDT 2020". Below I have the tweaks I've made to suit my needs.

![Autokey]({{"/assets/images/autokey.png" | relative_url}})

#### Hotkey

Clicking the Set button lets you choose the keyboard shortcut that will run this script. I had problems getting it to work at first - restarting cleared that up. Once working, you need to remember to save before any hotkey changes are usable. I first found the feature in One Note, but unsurprisingly it exists in others like Google Sheets and Excel. Now I'm able to have a consistent shortcut across all my apps.

#### Custom Date Formatting

```
output = system.exec_command("date '+%F'")
keyboard.send_keys(output)
```

If you aren't familiar with Python syntax, this is essentially calling the linux date program and using that output as the date to display. I was looking for YYYY-MM-DD which is where the '+%F' comes in. If you prefer a different format you can run `man date` from the terminal to get a list of all the formatting options or if that's too much effort check it out [below](#date-formatting).

#### Abbreviations

![Abbreviations]({{"/assets/images/abbr.png" | relative_url}})

Abbreviations let you type a set of characters and have the script trigger off of that. Particularly useful if you aren't found of remembering millions of keyboard shortcuts.

#### Window Filter

![AutoKey Window Filter]({{"/assets/images/autokey-window-filter.png" | relative_url}})

The window filter allows you to only match a certain program or specific window title. I could for example only allow this shortcut to be enabled within Google Chrome.

## Conclusion

I've barely scratched the surface of what you can configure, but I'm happy to have a simple and consistent way to add the date to any document I'm working on. Across all of my digital note taking, this tends to be several times a day.

2020-10-03

## Appendix

### Date Formatting

```
%%     a literal %
%a     locale's abbreviated weekday name (e.g., Sun)
%A     locale's full weekday name (e.g., Sunday)
%b     locale's abbreviated month name (e.g., Jan)
%B     locale's full month name (e.g., January)
%c     locale's date and time (e.g., Thu Mar  3 23:05:25 2005)
%C     century; like %Y, except omit last two digits (e.g., 20)
%d     day of month (e.g., 01)
%D     date; same as %m/%d/%y
%e     day of month, space padded; same as %_d
%F     full date; same as %Y-%m-%d
%g     last two digits of year of ISO week number (see %G)
%G     year of ISO week number (see %V); normally useful only with %V
%h     same as %b
%H     hour (00..23)
%I     hour (01..12)
%j     day of year (001..366)
%k     hour, space padded ( 0..23); same as %_H
%l     hour, space padded ( 1..12); same as %_I
%m     month (01..12)
%M     minute (00..59)
%n     a newline
%N     nanoseconds (000000000..999999999)
%p     locale's equivalent of either AM or PM; blank if not known
%P     like %p, but lower case
%q     quarter of year (1..4)
%r     locale's 12-hour clock time (e.g., 11:11:04 PM)
%R     24-hour hour and minute; same as %H:%M
%s     seconds since 1970-01-01 00:00:00 UTC
%S     second (00..60)
%t     a tab
%T     time; same as %H:%M:%S
%u     day of week (1..7); 1 is Monday
%U     week number of year, with Sunday as first day of week (00..53)
%V     ISO week number, with Monday as first day of week (01..53)
%w     day of week (0..6); 0 is Sunday
%W     week number of year, with Monday as first day of week (00..53)
%x     locale's date representation (e.g., 12/31/99)
%X     locale's time representation (e.g., 23:13:48)
%y     last two digits of year (00..99)
%Y     year
%z     +hhmm numeric time zone (e.g., -0400)
%:z    +hh:mm numeric time zone (e.g., -04:00)
%::z   +hh:mm:ss numeric time zone (e.g., -04:00:00)
%:::z  numeric time zone with : to necessary precision (e.g., -04, +05:30)
%Z     alphabetic time zone abbreviation (e.g., EDT)
```