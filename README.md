#World countries in JSON, CSV, XML and YAML.
## Countries data
This repository contains lists of world countries in JSON, CSV and XML. Each line contains the country:

 - `name`
 	 - `common` - common name in english
 	 - `official` - official name in english
 	 - `native`
 	 	 - `common` - common name in the native language
 	 	 - `official` - official name in the native language
 - country code top-level domain (`tld`)
 - code ISO 3166-1 alpha-2 (`cca2`)
 - code ISO 3166-1 numeric (`ccn3`)
 - code ISO 3166-1 alpha-3 (`cca3`)
 - ISO 4217 currency code(s) (`currency`)
 - calling code(s) (`callingCode`)
 - capital city (`capital`)
 - alternative spellings (`altSpellings`)
 - relevance
 - region
 - subregion
 - native language (`nativeLanguage`) ISO 639-3 code of language used for the native names
 - list of official languages (`languages`)
 	- key: three-letter ISO 639-3 language code
 	- value: name of the language in english
 - name translations (`translations`)
 - latitude and longitude (`latlng`)
 - name of residents (`demonym`)
 - landlocked status (`landlocked`)
 - land borders (`borders`)
 - land area in km² (`area`)

#### Additional data
The [data](https://github.com/mledoze/countries/tree/master/data) folder contains additional data such as the countries
GeoJSON outlines and flags in SVG format.

##Examples
#####JSON
```json
{
	"name": {
		"common": "Austria",
		"official": "Republic of Austria",
		"native": {
			"common": "\u00d6sterreich",
			"official": "Republik \u00d6sterreich"
		}
	},
	"tld": [".at"],
	"cca2": "AT",
	"ccn3": "040",
	"cca3": "AUT",
	"currency": ["EUR"],
	"callingCode": ["43"],
	"capital": "Vienna",
	"altSpellings": ["AT", "\u00d6sterreich", "Osterreich", "Oesterreich"],
	"relevance": "0",
	"region": "Europe",
	"subregion": "Western Europe",
	"nativeLanguage": "deu",
	"languages": {
		"deu": "German"
	},
	"translations": {
		"cym": "Awstria",
		"deu": "\u00d6sterreich",
		"fra": "Autriche",
		"hrv": "Austrija",
		"ita": "Austria",
		"jpn": "\u30aa\u30fc\u30b9\u30c8\u30ea\u30a2",
		"nld": "Oostenrijk",
		"por": "\u00c1ustria",
		"rus": "\u0410\u0432\u0441\u0442\u0440\u0438\u044f",
		"spa": "Austria"
	},
	"latlng": [47.33333333, 13.33333333],
	"demonym": "Austrian",
	"landlocked": true,
	"borders": ["CZE", "DEU", "HUN", "ITA", "LIE", "SVK", "SVN", "CHE"],
	"area": 83871
},
{
	"name": {
		"common": "Niger",
		"official": "Republic of Niger",
		"native": {
			"common": "Niger",
			"official": "R\u00e9publique du Niger"
		}
	},
	"tld": [".ne"],
	"cca2": "NE",
	"ccn3": "562",
	"cca3": "NER",
	"currency": ["XOF"],
	"callingCode": ["227"],
	"capital": "Niamey",
	"altSpellings": ["NE", "Nijar", "Republic of Niger", "R\u00e9publique du Niger"],
	"relevance": "0",
	"region": "Africa",
	"subregion": "Western Africa",
	"nativeLanguage": "fra",
	"languages": {
		"fra": "French"
	},
	"translations": {
		"deu": "Niger",
		"fra": "Niger",
		"hrv": "Niger",
		"ita": "Niger",
		"jpn": "\u30cb\u30b8\u30a7\u30fc\u30eb",
		"nld": "Niger",
		"por": "N\u00edger",
		"rus": "\u041d\u0438\u0433\u0435\u0440",
		"spa": "N\u00edger"
	},
	"latlng": [16, 8],
	"demonym": "Nigerien",
	"landlocked": true,
	"borders": ["DZA", "BEN", "BFA", "TCD", "LBY", "MLI", "NGA"],
	"area": 1267000
}
```

#####GeoJSON outline
See an example for [Germany](https://github.com/mledoze/countries/blob/bb61a1cddfefd09ad5c92ad0a1effbfceba39930/data/deu.geo.json).

#####CSV
```csv
"name";"tld";"cca2";"ccn3";"cca3";"currency";"callingCode";"capital";"altSpellings";"relevance";"region";"subregion";"nativeLanguage";"languages";"translations";"latlng";"demonym";"landlocked";"borders";"area"
⋮
"Afghanistan,Islamic Republic of Afghanistan,افغانستان,د افغانستان اسلامي جمهوریت";".af";"AF";"004";"AFG";"AFN";"93";"Kabul";"AF,Afġānistān";"0";"Asia";"Southern Asia";"pus";"Dari,Pashto,Turkmen";"Affganistan,Afghanistan,Afghanistan,Afganistan,Afghanistan,アフガニスタン,Afghanistan,Afeganistão,Афганистан,Afganistán";"33,65";"Afghan";"1";"IRN,PAK,TKM,UZB,TJK,CHN";"652230"
"Åland Islands,Åland Islands,Åland,Landskapet Åland";".ax";"AX";"248";"ALA";"EUR";"358";"Mariehamn";"AX,Aaland,Aland,Ahvenanmaa";"0";"Europe";"Northern Europe";"swe";"Swedish";"Åland,Åland,Ålandski otoci,Isole Aland,オーランド諸島,Ålandeilanden,Alândia,Аландские острова,Alandia";"60.116667,19.9";"Ålandish";"";"";"1580"
"Albania,Republic of Albania,Shqipëria,Republika e Shqipërisë";".al";"AL";"008";"ALB";"ALL";"355";"Tirana";"AL,Shqipëri,Shqipëria,Shqipnia";"0";"Europe";"Southern Europe";"sqi";"Albanian";"Albania,Albanien,Albanie,Albanija,Albania,アルバニア,Albanië,Albânia,Албания,Albania";"41,20";"Albanian";"";"MNE,GRC,MKD,KOS";"28748"
"Algeria,People's Democratic Republic of Algeria,الجزائر,الجمهورية الديمقراطية الشعبية الجزائرية";".dz,الجزائر.";"DZ";"012";"DZA";"DZD";"213";"Algiers";"DZ,Dzayer,Algérie";"0";"Africa";"Northern Africa";"ara";"Arabic";"Algeria,Algerien,Algérie,Alžir,Algeria,アルジェリア,Algerije,Algéria,Алжир,Argelia";"28,3";"Algerian";"";"TUN,LBY,NER,ESH,MRT,MLI,MAR";"2381741"
⋮
```

#####XML
```xml
<?xml version="1.0" encoding="UTF-8"?>
<countries>
  <country name="Afghanistan,Islamic Republic of Afghanistan,افغانستان,د افغانستان اسلامي جمهوریت" tld=".af" cca2="AF" ccn3="004" cca3="AFG" currency="AFN" callingCode="93" capital="Kabul" altSpellings="AF,Afġānistān" relevance="0" region="Asia" subregion="Southern Asia" nativeLanguage="pus" languages="Dari,Pashto,Turkmen" translations="Affganistan,Afghanistan,Afghanistan,Afganistan,Afghanistan,アフガニスタン,Afghanistan,Afeganistão,Афганистан,Afganistán" latlng="33,65" demonym="Afghan" landlocked="1" borders="IRN,PAK,TKM,UZB,TJK,CHN" area="652230"/>
  <country name="Åland Islands,Åland Islands,Åland,Landskapet Åland" tld=".ax" cca2="AX" ccn3="248" cca3="ALA" currency="EUR" callingCode="358" capital="Mariehamn" altSpellings="AX,Aaland,Aland,Ahvenanmaa" relevance="0" region="Europe" subregion="Northern Europe" nativeLanguage="swe" languages="Swedish" translations="Åland,Åland,Ålandski otoci,Isole Aland,オーランド諸島,Ålandeilanden,Alândia,Аландские острова,Alandia" latlng="60.116667,19.9" demonym="Ålandish" landlocked="" borders="" area="1580"/>
  <country name="Albania,Republic of Albania,Shqipëria,Republika e Shqipërisë" tld=".al" cca2="AL" ccn3="008" cca3="ALB" currency="ALL" callingCode="355" capital="Tirana" altSpellings="AL,Shqipëri,Shqipëria,Shqipnia" relevance="0" region="Europe" subregion="Southern Europe" nativeLanguage="sqi" languages="Albanian" translations="Albania,Albanien,Albanie,Albanija,Albania,アルバニア,Albanië,Albânia,Албания,Albania" latlng="41,20" demonym="Albanian" landlocked="" borders="MNE,GRC,MKD,KOS" area="28748"/>
⋮
<countries>
```

#####YAML
```yaml
- { name: { common: Afghanistan, official: 'Islamic Republic of Afghanistan', native: { common: افغانستان, official: 'د افغانستان اسلامي جمهوریت' } }, tld: [.af], cca2: AF, ccn3: '004', cca3: AFG, currency: [AFN], callingCode: ['93'], capital: Kabul, altSpellings: [AF, Afġānistān], relevance: '0', region: Asia, subregion: 'Southern Asia', nativeLanguage: pus, languages: { prs: Dari, pus: Pashto, tuk: Turkmen }, translations: { cym: Affganistan, deu: Afghanistan, fra: Afghanistan, hrv: Afganistan, ita: Afghanistan, jpn: アフガニスタン, nld: Afghanistan, por: Afeganistão, rus: Афганистан, spa: Afganistán }, latlng: [33, 65], demonym: Afghan, landlocked: true, borders: [IRN, PAK, TKM, UZB, TJK, CHN], area: 652230 }
- { name: { common: 'Åland Islands', official: 'Åland Islands', native: { common: Åland, official: 'Landskapet Åland' } }, tld: [.ax], cca2: AX, ccn3: '248', cca3: ALA, currency: [EUR], callingCode: ['358'], capital: Mariehamn, altSpellings: [AX, Aaland, Aland, Ahvenanmaa], relevance: '0', region: Europe, subregion: 'Northern Europe', nativeLanguage: swe, languages: { swe: Swedish }, translations: { deu: Åland, fra: Åland, hrv: 'Ålandski otoci', ita: 'Isole Aland', jpn: オーランド諸島, nld: Ålandeilanden, por: Alândia, rus: 'Аландские острова', spa: Alandia }, latlng: [60.116667, 19.9], demonym: Ålandish, landlocked: false, borders: {  }, area: 1580 }
- { name: { common: Albania, official: 'Republic of Albania', native: { common: Shqipëria, official: 'Republika e Shqipërisë' } }, tld: [.al], cca2: AL, ccn3: '008', cca3: ALB, currency: [ALL], callingCode: ['355'], capital: Tirana, altSpellings: [AL, Shqipëri, Shqipëria, Shqipnia], relevance: '0', region: Europe, subregion: 'Southern Europe', nativeLanguage: sqi, languages: { sqi: Albanian }, translations: { cym: Albania, deu: Albanien, fra: Albanie, hrv: Albanija, ita: Albania, jpn: アルバニア, nld: Albanië, por: Albânia, rus: Албания, spa: Albania }, latlng: [41, 20], demonym: Albanian, landlocked: false, borders: [MNE, GRC, MKD, KOS], area: 28748 }
- { name: { common: Algeria, official: 'People''s Democratic Republic of Algeria', native: { common: الجزائر, official: 'الجمهورية الديمقراطية الشعبية الجزائرية' } }, tld: [.dz, الجزائر.], cca2: DZ, ccn3: '012', cca3: DZA, currency: [DZD], callingCode: ['213'], capital: Algiers, altSpellings: [DZ, Dzayer, Algérie], relevance: '0', region: Africa, subregion: 'Northern Africa', nativeLanguage: ara, languages: { ara: Arabic }, translations: { cym: Algeria, deu: Algerien, fra: Algérie, hrv: Alžir, ita: Algeria, jpn: アルジェリア, nld: Algerije, por: Algéria, rus: Алжир, spa: Argelia }, latlng: [28, 3], demonym: Algerian, landlocked: false, borders: [TUN, LBY, NER, ESH, MRT, MLI, MAR], area: 2381741 }
- { name: { common: 'American Samoa', official: 'American Samoa', native: { common: 'American Samoa', official: 'American Samoa' } }, tld: [.as], cca2: AS, ccn3: '016', cca3: ASM, currency: [USD], callingCode: ['1684'], capital: 'Pago Pago', altSpellings: [AS, 'Amerika Sāmoa', 'Amelika Sāmoa', 'Sāmoa Amelika'], relevance: '0.5', region: Oceania, subregion: Polynesia, nativeLanguage: eng, languages: { eng: English, smo: Samoan }, translations: { deu: Amerikanisch-Samoa, fra: 'Samoa américaines', hrv: 'Američka Samoa', ita: 'Samoa Americane', jpn: アメリカ領サモア, nld: 'Amerikaans Samoa', por: 'Samoa Americana', rus: 'Американское Самоа', spa: 'Samoa Americana' }, latlng: [-14.33333333, -170], demonym: 'American Samoan', landlocked: false, borders: {  }, area: 199 }
```

#### About the relevance factor
To understand the usefulness of the relevance parameter, please read this:
- http://uxdesign.smashingmagazine.com/2011/11/10/redesigning-the-country-selector/
- http://baymard.com/labs/country-selector

## Showcase
Projects using this dataset:

- [REST Countries](http://restcountries.eu/)
- [International Telephone Input](http://jackocnr.com/intl-tel-input.html)
- [Telephone JS](https://github.com/lukaswhite/telephones-js)
- [Countries of the World](http://countries.petethompson.net/)
- [Country Prefix Codes For Go](https://github.com/relops/prefixes)
- [Ask the NSA](http://askthensa.com/)
- [Country Info Mapper in Go](https://github.com/pirsquare/country-mapper)

## How to contribute?
Please refer to [CONTRIBUTING](https://github.com/mledoze/countries/blob/master/CONTRIBUTING.md).

## To do
 - add the type of the country (country, sovereign state, public body, territory, etc.)
 - add missing translations

## Sources
http://www.currency-iso.org/ for currency codes.

Relevance are inspired by https://github.com/JamieAppleseed/selectToAutocomplete.

Region and subregion are taken from https://github.com/hexorx/countries.

GeoJSON outlines come from http://thematicmapping.org/downloads/world_borders.php.

The rest comes from Wikipedia.

## Credits
Thanks to:
 - @Glazz for his help with country calling codes
 - @hexorx for his work (https://github.com/hexorx/countries)
 - @frederik-jacques for the capital cities
 - @fayer for the population, geolocation, demonym and area data
 - @ancosen for his help with the borders data
 - all the contributors: https://github.com/mledoze/countries/graphs/contributors

## License
See [LICENSE](https://github.com/mledoze/countries/blob/master/LICENSE).
