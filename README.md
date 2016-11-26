# xliffEditServerlessTM
100% javascript serverless basic translation memory tool

Simple translation memory (TMM) tool in 100% javascript. Called xliffEdit. Its size is all of 10 KB, which might qualify it for the title of world's smallest.


It bills itself as a "proof of concept", with the concept being that modern web browser features and power can replace some of the more common standalone programs with ease.


Here is what the tool does:

1) It provides a translation workbench for bilingual XLIFF source files.
2) It allows using one bilingual TMX file as a read-only translation memory.
3) The latest version allows adding a multilingual term base .tbx. TBD: A search feature for the tbx.Right now, only the
browser search or scrolling are available.


Here are some notes and caveats:

1) The "Store in browser" button will store the translation (upper table contents) in a local temporary location. Once you clicked this button, you can close the tab. If you then open the xliffEdit.html again, the translation will be reloaded automatically.

But you should not close the browser and expect the same behavior. The local storage behaves differently depending on the browser, some specific browser settings, and on the operating system.

Before closing the browser, always save the translation using the "Export" button. If it is not automatically reloaded when you start xliffEdit next time, load this exported.xml to continue.


2) The current version has only been tested with Xliffs and TMX files produced by Memsource Cloud (tm).

3) The current version has only been tested with Firefox.

4) The only changes the tool makes to the XLIFF base file is adding or modifying translations, i.e. the contents of "target" elements. No other xml elements or attributes are modified.

5) Existing context information or alternative translations are not shown.


