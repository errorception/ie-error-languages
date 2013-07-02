Internet Explorer's i18n Strings For Error Messages
===

This is a repository of the i18n resources of error messages in Internet Explorer (10).

These have been extracted painstakingly by the awesome [Rajasekharan Vengalil](http://blogorama.nerdworks.in/), from IE's DLLs. I've detailed the process below, to the best of my understanding.

* Get a Windows 7 box
* Put IE10 on it
* Download and install all the language packs [from here](http://www.microsoft.com/en-us/download/details.aspx?id=36804)
* Use [Resource Hacker](http://angusj.com/resourcehacker/) to extract the “String Table” resources from all the *jscript.dll.mui* files

In addition to the steps above, I've also converted the files from their original encoding of UCS2 (UTF16LE) to UTF8 before putting it up here.

Read the [blog post](http://blog.errorception.com/2013/07/ies-i18n-strings-for-error-messages.html).

Format of the files
---

* The files are named by their locale names.
* Everything before the first `,` (comma) is the ID of the error message, and helps you build a mapping between the language files.
* The stuff after that first comma is the i18n error string.

Easy peasy!