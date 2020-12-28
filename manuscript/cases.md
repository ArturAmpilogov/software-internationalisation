# Cases and examples

## HTML encoding security

Internet Explorer may incorrectly guess that the page is encoded in UTF-7, and insert malicous script.
 The string <script>alert(1)</script> can be encoded in UTF-7 as +ADw-script+AD4-alert(1)+ADw-/script+AD4-
https://code.google.com/archive/p/doctype-mirror/wikis/ArticleUtf7.wiki
