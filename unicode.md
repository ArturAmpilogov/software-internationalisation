# Unicode
The Unicode Standard encodes a single, very large set of characters, encompassing all the
characters needed for worldwide use. This single repertoire is intended to be universal in
coverage, containing all the characters for textual representation in all modern writing systems, in most historic writing systems, and for symbols used in plain text.




# Two users who are familiar with the standard and who are presented with
the same text ideally will choose the same sequence of character codes to encode the text

# Glyph VS Character
Characters are the abstract representations of the smallest components of written language that have semantic value.
Glyphs represent the shapes that characters can have when they are rendered or displayed.

A repertoire of glyphs makes up a font. 

Figure 2-2. Characters Versus Glyphs
p.15-16


## Figure 2-4. Bidirectional Ordering
## Figure 2-5. Writing Direction and Numbers (p. 20)

The Unicode Standard avoids duplicate encoding of characters by unifying them within
scripts across language. Common letters are given one code each, regardless of language, as
are common Chinese/Japanese/Korean (CJK) ideographs (p.21) Han

## 1,114,112
In the Unicode Standard, the codespace consists of the integers from 0 to 10FFFF16, comprising 1,114,112 code points available for assigning the repertoire of abstract characters.

# Swedish “ä” and “ö” are individual characters

In French diaeresis on a vowel merely marks it as being pronounced in
isolation.

Good for search

## Encoded points with similar glyphs
U+0061 latin small letter a
U+10330 gothic letter ahsa
U+201DF cjk unified ideograph-201df
p.30

## https://unicode.org/faq/utf_bom.html

## https://stackoverflow.com/questions/496321/utf-8-utf-16-and-utf-32
UTF-8: Variable-width encoding, backwards compatible with ASCII. ASCII characters (U+0000 to U+007F) take 1 byte, code points U+0080 to U+07FF take 2 bytes, code points U+0800 to U+FFFF take 3 bytes, code points U+10000 to U+10FFFF take 4 bytes. Good for English text, not so good for Asian text.
UTF-16: Variable-width encoding. Code points U+0000 to U+FFFF take 2 bytes, code points U+10000 to U+10FFFF take 4 bytes. Bad for English text, good for Asian text.
UTF-32: Fixed-width encoding. All code points take four bytes.

## Self-synchronization
Another aspect of non-overlap in the Unicode encoding forms is that all Unicode characters have determinate boundaries when expressed in any of the encoding forms. That is,
the edges of code unit sequences representing a character are easily determined by local
examination of code units; there is never any need to scan back indefinitely in Unicode text
to correctly determine a character boundary. This property of the encoding forms has
sometimes been referred to as self-synchronization. This property has another very important implication: corruption of a single code unit corrupts only a single character; none of
the surrounding characters are affected.
For example, when randomly accessing a string, a program can find the boundary of a
character with limited backup. In UTF-16, if a pointer points to a leading surrogate, a single backup is required. In UTF-8, if a pointer points to a byte starting with 10xxxxxx (in
binary), one to three backups are required to find the beginning of the character.
For example, when randomly accessing a string, a program can find the boundary of a
character with limited backup. In UTF-16, if a pointer points to a leading surrogate, a single backup is required. In UTF-8, if a pointer points to a byte starting with 10xxxxxx (in
binary), one to three backups are required to find the beginning of the character.
(p. 34)

## UTF history
http://lucumr.pocoo.org/2014/1/9/ucs-vs-utf8/


# UNICODE NORMALIZATION FORMS
https://unicode.org/reports/tr15/

The W3C Character Model for the World Wide Web 1.0: Normalization [CharNorm] and other W3C Specifications (such as XML 1.0 5th Edition) recommend using Normalization Form C for all content, because this form avoids potential interoperability problems arising from the use of canonically equivalent, yet different, character sequences in document formats on the Web. See the W3C Character Model for the Word Wide Web: String Matching and Searching [CharMatch] for more background.
https://www.w3.org/TR/charmod/

# Ohm and Omega example
https://en.wiktionary.org/wiki/%CE%A9
Ohm is left only for compatability

## Recognise a unicode symbol
http://shapecatcher.com/

## C# String.Normalize method
https://docs.microsoft.com/en-us/dotnet/api/system.string.normalize?view=netframework-4.8


##5.4 Handling Surrogate Pairs in UTF-16
The method used by UTF-16 to address the 1,048,576 supplementary code points that cannot
be represented by a single 16-bit value is called surrogate pairs. A surrogate pair consists
of a high-surrogate code unit (leading surrogate) followed by a low-surrogate code
unit (trailing surrogate), as described in the specifications in Section 3.8, Surrogates, and
the UTF-16 portion of Section 3.9, Unicode Encoding Forms.


## 5.20 Unicode Security (p245)
Spoofing

Table 6-2. Unicode Space Characters
Table 6-3. Unicode Dash Characters

UNICODE SECURITY CONSIDERATIONS http://unicode.org/reports/tr36/