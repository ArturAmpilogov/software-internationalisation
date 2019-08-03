## 1
https://stackoverflow.com/questions/48067545/why-does-unicode-implement-the-turkish-i-the-way-it-does
http://www.i18nguy.com/unicode/turkish-i18n.html
https://en.wikipedia.org/wiki/Dotted_and_dotless_I

https://devblogs.microsoft.com/oldnewthing/?p=42643

string opMode = ConfigurationManager.AppSettings["Mode"] ?? string.Empty;
if (opMode.ToUpper() != "TESTING")
{

}

Figure 5-14. Uppercase Mapping for Turkish I (Unicode standard)

## 2
Character chart limitation fo the input field
(Chinese, German, Russian, English)?

Unicode vs UTF-8

## 3
Phone number input (Chinese symbols?) - international format

## 4
Address input (Amazon example) - international format


