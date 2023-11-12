# 🤍🖤 Welcome to EqualStreetNames Basel 🤍🖤

> Street names reflect the commemorative decisions of each municipality over time, and as such can be understood as the city’s manifesto about its social, cultural and political values. (Oto-Peralías D, [2018](https://doi.org/10.1093/jeg/lbx030)).

> Die deutliche Absenz von konkreten Frauenfiguren im öffentlichen Raum spiegeln [...] die Schweizer Geschichtsvergessenheit in Bezug auf Frauen und ihren Ausschluss aus der politischen und wirtschaftlichen Sphäre.
>
> -- <cite>Essay der Historikerinnen Tiziana Bonetti und Rachel Huber. [In blick.ch](https://www.blick.ch/life/wissen/geschichte/schweizer-erinnerungskultur-wieso-es-mehr-frauendenkmaeler-braucht-id17408231.html)</cite>  

---

🌟 [basel.equalstreetnames.eu](https://basel.equalstreetnames.eu) shows soon all Streets named after a Person. 🌟  
🚧 This means, work is still ongoing 🚧
  
Follow us on Twitter: https://twitter.com/EqualsnBasel



# Overview 
The aim of this section is to provide an Overview on how to prepare the required data so it will be shown on the map of [basel.equalstreetnames.eu](https://basel.equalstreetnames.eu)

Basic steps are:
1. Identifiy the Street, named after a Person, on [Strassennamen](https://data.bs.ch/explore/dataset/100189/information/)
2. Find the Wikidata-Item of this street
3. Find the Wikidata-Item of the Person
4. Link the Street-Wikidata-Item with the Person-Wikidata-Item
5. Link the Street-Wikidata-Item with the Geometry on OpenStreetMap


See following sections to find out more in detail.

## Identify Streets named after a Person
1. Find a Street that you know it is named after a Person (or something else).
2. Doublecheck with description from [offizielle Strassenverzeichnis des Kanton Basel-Stadt](https://data.bs.ch/explore/dataset/100189/information/)


## Find the Wikidata-Item of this street
* Search at [Wikidata.org](https://www.wikidata.org)
* Or: Take a look at the List of all Streets in Basel in Wikidata: [Wikidata Query Service](https://query.wikidata.org/#SELECT%20%3Fsubject%20%3FsubjectLabel%20%3Fstrkey%20%3Fnamedafter%20%3FnamedafterLabel%20WHERE%20%7B%0A%20%20%3Fsubject%20wdt%3AP1945%20%3Fstrkey.%0A%20%20%0A%20%20%3Fsubject%20p%3AP1945%20%5B%20prov%3AwasDerivedFrom%20%5B%20pr%3AP248%20wd%3AQ111770447%20%5D%20%5D%20.%0A%20%20Optional%20%7B%3Fsubject%20wdt%3AP138%20%3Fnamedafter.%7D%0A%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22de%22%20.%20%7D%20%20%20%0A%7D%0A)

Example: [Meret Oppenheim-Strasse](https://www.wikidata.org/wiki/Q111633069)

## Find the Wikidata-Item of the Person
This is the most tricky Part..
1. Search at [Wikidata.org](https://www.wikidata.org) for this Person.
2. Note the Q-Number of the Person

Example: Q61594 for [Meret Oppenheim](https://www.wikidata.org/wiki/Q61594)

## Link the Street-Wikidata-Item with the Person-Wikidata-Item
1. Return to the Wikidata-Entry of the Street
2. Click "add statement" (At the End of all Statements)
3. Choose as Property: "named after"
4. Add as the Value the Q-Number of the Person and choose the Name as the value
5. Click "add reference"
6. Choose as Property: "stated in" and as value "Streetnames Canton Basel-Stadt"
7. Click "add" (to add an additional reference)
8. Choose as Property: "retrieved" and as value the Date of Today eg. "13.05.2006"
9. Click "publish"

Done :muscle:


# Datasources

## Datenportal Kanton Basel-Stadt
On the OGD-Portal, the Dataset [Strassennamen](https://data.bs.ch/explore/dataset/100189/information/) is the official List of all Streetnames and the meaning of there Names in the Canton Basel-Stadt.

## Liste der Strassennamen von Basel
⚠️Do not use this list for basel.equalstreetnames.eu.⚠️  
Wikipedia has a Site [Liste der Strassennamen von Basel](https://de.wikipedia.org/wiki/Liste_der_Strassennamen_von_Basel). This List contains explanations of the Namingsources. However, it seems this List is based on a [List published by the Bau- und Verkehrsdepartement](https://www.bvd.bs.ch/dam/jcr:b8733740-18a4-4bff-892f-d90b03c36681/Basler%20Strassennamen%20mit%20Kurzerklaerungen%202017-10-18.pdf) from 18. October 2017.  
⚠️Do not use this list for basel.equalstreetnames.eu.⚠️


## Historisches Lexikon der Schweiz (HLS)
To add more informationen about a Person on Wikidata, HLS is an excelent source.
More about [HLS on Wikipedia](https://de.wikipedia.org/wiki/Historisches_Lexikon_der_Schweiz).

[HLS](https://hls-dhs-dss.ch) is published under [Creative Commons BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). See also Nutzungsbedingungen of HLS: [Urheberrechte und Verwendung der HLS-Inhalte](https://hls-dhs-dss.ch/de/about/usage#HUrheberrechteundVerwendungderHLS-Inhalte)

You may use HLS to add Information on Wikidata / Wikipedia and even create a Wikipedia-article entirely based on an HLS-article.  
:warning: If you do so, Cite all Informations!

# 🤍❤️ Streetnames in Basel-Landschaft ❤️🤍
[Prix Promenade – «Frauennamen ins Strassennetz!»](https://www.gruppe14juni.ch/prix-promenade)

---
# ToDo
- [x] Add Statement "coordinate location" to all Streetobjects ['Innerortsstraße' 'Straßenbrücke' 'Platz' 'Bogenbrücke'] in Wikidata e.g.: https://www.wikidata.org/wiki/Q27077277
- [ ] Take a look at https://github.com/d-gurtovoy/streetnameLinks

