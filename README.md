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

<!--
See following sections to find out more in detail.

## Identify Streets named after a Person
1. Find a Street in the [Workinglist](https://docs.google.com/spreadsheets/d/1ONbDBkYPxVkZ0lsC-Cm07OYaQsixLnNraNKnyIv4tWo/edit?usp=sharing) (Column B) which is not allready link to a Person (Column D).


## Find the Wikidata-Item of this street
* Search at [Wikidata.org](https://www.wikidata.org)
* Or: Take the Q-Nummer of the Street from Column A of the [Workinglist](https://docs.google.com/spreadsheets/d/1ONbDBkYPxVkZ0lsC-Cm07OYaQsixLnNraNKnyIv4tWo/edit?usp=sharing) and search for this at [Wikidata.org](https://www.wikidata.org)

Example: [Emilie-Kempin-Spyri-Weg](https://www.wikidata.org/wiki/Q27329833)

## Find the Wikidata-Item of the Person
This is the most tricky Part..
1. Read at Column G of the [Workinglist](https://docs.google.com/spreadsheets/d/1ONbDBkYPxVkZ0lsC-Cm07OYaQsixLnNraNKnyIv4tWo/edit?usp=sharing) an try to find out more about the Person
1. Or: search for the Street at [Strassennamen-Datenbank der Stadt Zürich](https://stadt-zuerich.ch/strassennamen-datenbank)
2. Search at [Wikidata.org](https://www.wikidata.org) for this Person.
3. Note the Q-Number of the Person

Example: Q119636 for [Emilie Kempin-Spyri](https://www.wikidata.org/wiki/Q119636)

## Link the Street-Wikidata-Item with the Person-Wikidata-Item
1. Return to the Wikidata-Entry of the Street
2. Click "add statement" (At the End of all Statements)
3. Choose as Property: "named after"
4. Add as the Value the Q-Number of the Person and choose the Name as the value
5. Click "add reference"
6. Choose as Property: "stated in" and as value "Street name directory Zurich"
7. Click "add" (to add an additional reference)
8. Choose as Property: "retrieved" and as value the Date of Today eg. "13.05.2006"
9. Click "publish"

Done :muscle:

-->



# Datasources

## Datenportal Kanton Basel-Stadt
On the OGD-Portal is an up to date List of all Streetnames and the meaning of there Names available: [Strassennamen](https://data.bs.ch/explore/dataset/100189/information/).

## Liste der Strassennamen von Basel
Wikipedia has a Site [Liste der Strassennamen von Basel](https://de.wikipedia.org/wiki/Liste_der_Strassennamen_von_Basel). This List contains explanations of the Namingsources. However, it seems this List is based on a [List published by the Bau- und Verkehrsdepartement](https://www.bvd.bs.ch/dam/jcr:b8733740-18a4-4bff-892f-d90b03c36681/Basler%20Strassennamen%20mit%20Kurzerklaerungen%202017-10-18.pdf) from 18. October 2017.  
Do not use this list for basel.equalstreetnames.eu.


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

