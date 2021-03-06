= ninajansen-cloud

* http://wiki.github.com/ninajansen/cloud

== DESCRIPTION:

Generates pdf-files with word clouds based on input. Inspired by wordle, but probably uses an entirely different algorithm, since Wordle is not Open Source. Also:

* Outputs only in pdf (if there was a decend svg writer for ruby, I'd use that). 
* Can't put words inside other words like wordle, and also a big word has a big space surrounding it while a small word has a small space.

But it is open source so feel free and encouraged to hack away and make this gem better.

The algortihm is a bin-packing algorithm. This means that clouds aim to take up as small an area as possible. A word has a surrounding box and that box is placed as close to the "center" as possible, where is does not collide with other boxes. The "center" is computed by a radial function, of which I have implemented several, making is possible to generate clouds of different shapes.

This is a beta in the original sense of the word, not in the google sense.

My blog-post introducing "cloud" is here: http://ninajansen.dk/2009/04/23/introducing-cloud-an-open-source-ruby-wordcloud-generator/

If you have used cloud to generate a cool wordcloud, please upload it to scribd and tag it with "wordcloud". Documents with this tag are here: http://www.scribd.com/tag/wordcloud 

== FEATURES/PROBLEMS:

* Can generate a word cloud from text, rss-feed or del.icio.us name
* Can use a number of different color palettes
* Can use a number of cloud shapes
* Can ignore common English and Danish words (feel free to add your own language(s))

Problems:

== SYNOPSIS:

Please clone this repository and try the examples:

git clone git://github.com/ninajansen/cloud_examples.git 

The README file (http://github.com/ninajansen/cloud_examples/tree/master) describes all the options

== REQUIREMENTS:

PDF::Writer
RubyInline

== INSTALL:

* sudo gem install ninajansen-cloud

== LICENSE:

(The MIT License)

Copyright (c) 2009 Nina Jansen

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.