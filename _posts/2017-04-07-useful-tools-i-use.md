---
layout: post
title: "Useful Tools I Use"
---

# [k2pdfopt](http://www.willus.com/k2pdfopt/)
A tool, transforms pdf files to easy-read pdf in mobile device.
K2pdfopt optimizes PDF/DJVU files for mobile e-readers (e.g. the Kindle) and smartphones. It works well on multi-column PDF/DJVU files and can re-flow text even on scanned PDF files. It can also be used as a general PDF copying/cropping/re-sizing/OCR-ing manipulation tool. 



# [Coherent PDF](http://community.coherentpdf.com)
The Coherent PDF Command Line Tools allow you to manipulate existing PDF files in a variety of ways. E.g.:
* Merge PDF files together, or split them apart
* Encrypt and decrypt
* Scale, crop and rotate pages
* Read and set document info and metadata
* Copy, add or remove bookmarks
* Stamp logos, text, dates, page numbers
* Add or remove attachments
* Losslessly compress PDF files


GNU Aspell is a Free and Open Source spell checker.


## Basic usage
1. For any files: `aspell -c [file]`
2. For tex files: `aspell -t -c [file]`

# [htop](http://hisham.hm/htop/)
An interactive text-mode process viewer for Unix systems.

## Basic usage
1. Run it: `htop`
2. Sort by a column: `<F6>`
3. Filter to locate your interested process: `<F4>`
4. Setup all things: `<F2>`

# [AutoIt](https://www.autoitscript.com/site/autoit/)(For windows)
AutoIt is a freeware BASIC-like scripting language designed for automating the Windows GUI and general scripting. 

## What I use it for?
1. Game automation.
2. Auto fillout web form.


# Online markdown editor: [dillinger](http://dillinger.io)
Well, a perfect online markdown editor, except not supporting chinese.


# [Expect](http://expect.sourceforge.net/)
Expect is a tool for automating interactive applications such as telnet, ftp, passwd, fsck, rlogin, tip, etc. Expect really makes this stuff trivial. Expect is also useful for testing these same applications. And by adding Tk, you can also wrap interactive applications in X11 GUIs.

## My example
~~~
#!/usr/bin/expect
set timeout 2
# This line login your server
spawn ssh [your-server]

# After login your sever, run a script, which need a sudo priviledge
expect "$"
send "./startRun.sh\r"

# Send the password.
expect "Password:"
send "[yourPassword]\r"

expect "$"
send "cd ~/Projects\r"
interact
#expect eof
~~~

