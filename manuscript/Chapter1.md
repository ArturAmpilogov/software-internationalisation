# Internationalisation vs Localisation vs Globalisation

The terms internationalisation, localisation and globalisation have no well defined defenitions these days. The difference in the notion can be found even in one company, for example Microsoft oficial documents and unofficial discussions in the MSDN blogs.

The author tried his best to get the mostly used defenitions of these words used today in the sofware development.

## Internationalisation (i18n)

In the software design and development, internationalisation implies the process of enabling localisation easily. Internationalisation is also written as _i18n_, where 18 is the number of letters between i and n.

Usually it includes the next points, but not requires them:

- Global support for almost any human language symbols. Unicode as the text encoding standard.
  Alloweness for the clients to post and read data in their languages.

- Support of world numeric, date, time and currency formats.
  For example, The application correctly understands the difference between European "DD/MM/YYY" ("DD-MM-YYYY") and the American "MM/DD/YYY" date formats.
  The product treats the Chilean "1,5" and Australian "1.5" as the same number value "one and a half".

- Easy addition of UI localization resources
  If the business requests tomorrow to add software localisation for a new country, the software has an easy ready process of implementation.
  For example, Netflix operates in more than 190 countries and for UI localisation created the product called Hydra.

## Localisation (l10n)

Localisation is the process of a product adaptation to meet the language, cultural and other requirements of a specific target market. Localisation is also known as _l10n_, where 10 is the number of letters between l and n.

The next points can be often found during the localisation process:

- Translating an application's resources into localised versions.
  Updating UI text to the targeted language, verification of the UI items position and layout correctness.

- Conforming to local standars.
  In 2016, the EU General Data Protection Regulation (GDPR) was adopted to protect EU citizens data privacy. In two years later, the Barreiro Hospital in Portugal was fined 400,000 € for too broad data access.
  
  Many companies The famous popup "We use cookies for good" is the outcome of this law.

  In 2018, the Russian goverment signed the bill demanding local regional data storage for private citizens data (Yarovaya Law or Russian GDPR). While Microsft and Facebook immediately moved personal citizens information to their in-state data centers, LinkedIn was not ready for such changes and was blocked in the country.

  Another example involves the tax support for a new region. The sales tax, as it is known in the USA, varies from state to state. In Germany the VAT rate is the same across the country, and the calculation logic is different ("value-added tax" is another name for "sales tax"). Reaching a new market in this case assumes that the software is ready for the new logic addition.

## Globalisation (g11n, going global)

Globalisation, also called _g11n_ or _going global_, is the process by which organizations connect with their customers and partners around the world.

The process often includes:

- Neutral product names and text titles, no offence meaning in the targeted markets.
- Neutral visualisation
  Globalisation trends suggest to visual graphics and prospects ....
  
- Unified process for coming to a new region.
  It is not always possible to find the world neutral word, and the company should be ready to change the name for a local market.

## References

[W3C Internationalization notion](https://www.w3.org/International/questions/qa-i18n)

[internationalizaton vs. localizability, Michael S. Kaplan, MSDN blog archive, 2005-09-09](http://archives.miloush.net/michkap/archive/2005/09/09/462862.html)

[Globalizing and localizing .NET applications, .NET Guide](https://docs.microsoft.com/en-us/dotnet/standard/globalization-localization/index)

[Yarovaya Law and new telecoms data storage requirements, International Law Office, August 08 2018](http://www.gorodissky.com/upload/articles/files/Yarovaya_Law_and_new_telecoms_data_storage_requirements.pdf)

[GDPR](https://eugdpr.org)

[Portuguese Data Protection Authority Imposes 400,000 € Fine on Hospital](https://www.datenschutz-notizen.de/portuguese-data-protection-authority-imposes-400000-e-fine-on-hospital-4821441/)

[Hydra, Medium Netflix blog, June 4, 2015](https://medium.com/netflix-techblog/localization-technologies-at-netflix-d033e7b13cf)
