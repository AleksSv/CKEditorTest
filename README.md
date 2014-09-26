CKEditorTest
============

Often times we have forms used for user input. Sometimes that input needs to be very complex, for instance a journalist writing an article would want to be able to input pictures, have headers, links to other urls, bold statements et cetera. 

http://ckeditor.com/

This code shows the usage of the CKEditor, which is either GPL/LGPL/MPL Open Source, or commercially licsensed at $300 for a permenent single website liscense for two developers.

http://ckeditor.com/about/license

Objective
=================
Purpose of this exercise is to use CKEditor to create a dynamic HTML post, convert it to JSON, and then convert that such that it is posted on to the web page. Once that is accomplished, this task can be expanded to be stored on a Database and allow registered users to make posts that remain on the server, either as HTML files or stored in a database.

Useful Documentation located at:

http://docs.ckeditor.com/#

http://docs.ckeditor.com/#!/guide/dev_installation

Samples in the ckedit directory are useful too

Useful Precautions
==================
It is very important to make sure that scripts are disabled, otherwise a huge security risk will be allowed when writers submit their content.

http://docs.ckeditor.com/#!/guide/dev_disallowed_content

Problems
==================
The disallowedContent method does not seem to work, for instance, scripts can run known functions and still show up in the HTML shown in Development tools. While parsing of the HTML server side would need to be done as we can't depend on the client side for security, it would be more user freindly if it got rid of disallowed content.
