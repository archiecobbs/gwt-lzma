**gwt-lzma** is a [GWT](http://code.google.com/webtoolkit/) module that implements the [Lempel-Ziv-Markov chain (LZMA)](http://en.wikipedia.org/wiki/Lzma) compression algorithm. This is a generic compression library, i.e., compression **in** Javascript, not just compression **of** Javascript (i.e., "minification").

The code is adapted from the Java LZMA implementation found in the [LZMA SDK](http://www.7-zip.org/sdk.html). The compressor and decompressor implement GWT's [Scheduler.RepeatingCommand](http://google-web-toolkit.googlecode.com/svn/javadoc/2.4/com/google/gwt/core/client/Scheduler.RepeatingCommand.html) interface so that other browser activity may continue while processing occurs.

See a working demo [here](http://archiecobbs.github.io/gwt-lzma/publish/demo/LZMADemo.html); the source code to the demo is [here](https://github.com/archiecobbs/gwt-lzma/tree/master/src/java/org/dellroad/lzma/demo).

View the Javadoc API [here](http://archiecobbs.github.io/gwt-lzma/publish/javadoc/index.html).

Note: The code works, but LZMA was not designed to run in a web browser as Javascript. Processing at higher compression levels (which use lots of memory) and/or with huge files may cause your browser to explode.

**Also:** A [standalone, non-GWT version](http://nmrugg.github.com/LZMA-JS/) of this code has been created as well.
