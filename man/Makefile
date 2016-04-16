#!/bin/sh
#
# Copyright (c) 2016 Mark Heily <mark@heily.com>
#
# Permission to use, copy, modify, and distribute this software for any
# purpose with or without fee is hereby granted, provided that the above
# copyright notice and this permission notice appear in all copies.
# 
# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
# WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
# MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
# ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
# WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
# ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
# OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
#

all: jailadm.8.html jailcfg.8.html jailadm.8.txt jailcfg.8.txt

jailadm.8.html: jailadm.8
	man2html < `echo $* | sed 's/\.html//'` > $*

jailadm.8.txt: jailadm.8
	man ./jailadm.8 | col -b > jailadm.8.txt

jailcfg.8.html: jailcfg.8
	man2html < `echo $* | sed 's/\.html//'` > $*

jailcfg.8.txt: jailcfg.8
	man ./jailcfg.8 | col -b > jailcfg.8.txt

clean:
	rm -f *.html *.txt
