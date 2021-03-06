# download-geofabrik

[![Build Status](https://travis-ci.org/julien-noblet/download-geofabrik.svg?branch=master)](https://travis-ci.org/julien-noblet/download-geofabrik)
[![Join the chat at https://gitter.im/julien-noblet/download-geofabrik](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/julien-noblet/download-geofabrik?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Go Report Card](https://goreportcard.com/badge/github.com/julien-noblet/download-geofabrik)](https://goreportcard.com/report/github.com/julien-noblet/download-geofabrik)

## Version 2
Warning! command line have changed from V1
see [Usage](#usage)

## Usage
```shell
./download-geofabrik download element
```
where ```element``` is one of geofabrik's files.
```shell
./download-geofabrik --help-long
usage: download-geofabrik [<flags>] <command> [<args> ...]

A command-line tool for downloading OSM files.

Flags:
      --help        Show context-sensitive help (also try --help-long and
                    --help-man).
  -c, --config="./geofabrik.yml"  
                    Set Config file.
  -n, --nodownload  Do not download file (test only)
  -v, --verbose     Be verbose

Commands:
  help [<command>...]
    Show help.


  update [<flags>]
    Update geofabrik.yml from github

    --url="https://raw.githubusercontent.com/julien-noblet/download-geofabrik/master/geofabrik.yml"  
      Url for config source

  list [<flags>]
    Show elements available

    --markdown  generate list in Markdown format

  download [<flags>] <element>
    Download element

    -B, --osm.bz2  Download osm.bz2 if available
    -S, --shp.zip  Download shp.zip if available
    -P, --osm.pbf  Download osm.pbf (default)
    -H, --osh.pbf  Download osh.pbf (default)
    -s, --state    Download state.txt file
    -p, --poly     Download poly file
```

## List of elements
|                  SHORTNAME                  |         IS IN         |               LONG NAME                | FORMATS |
|---------------------------------------------|-----------------------|----------------------------------------|---------|
| afghanistan                                 | Asia                  | Afghanistan                            | sPBHpS  |
| africa                                      |                       | Africa                                 | sPBHp   |
| alabama                                     | us                    | Alabama                                | sPBHpS  |
| alaska                                      | us                    | Alaska                                 | sPBHpS  |
| albania                                     | Europe                | Albania                                | sPBHpS  |
| alberta                                     | Canada                | Alberta                                | sPBHpS  |
| algeria                                     | Africa                | Algeria                                | sPBHpS  |
| alps                                        | Europe                | Alps                                   | sPBHp   |
| alsace                                      | France                | Alsace                                 | sPBHpS  |
| andorra                                     | Europe                | Andorra                                | sPBHpS  |
| angola                                      | Africa                | Angola                                 | sPBHpS  |
| antarctica                                  |                       | Antarctica                             | sPBHpS  |
| aquitaine                                   | France                | Aquitaine                              | sPBHpS  |
| argentina                                   | South America         | Argentina                              | sPBHpS  |
| arizona                                     | us                    | Arizona                                | sPBHpS  |
| arkansas                                    | us                    | Arkansas                               | sPBHpS  |
| arnsberg-regbez                             | Nordrhein-Westfalen   | Regierungsbezirk Arnsberg              | sPBHpS  |
| asia                                        |                       | Asia                                   | sPBHp   |
| australia                                   | Australia and Oceania | Australia                              | sPBHp   |
| australia-oceania                           |                       | Australia and Oceania                  | sPBHp   |
| austria                                     | Europe                | Austria                                | sPBHpS  |
| auvergne                                    | France                | Auvergne                               | sPBHpS  |
| azerbaijan                                  | Asia                  | Azerbaijan                             | sPBHpS  |
| azores                                      | Europe                | Azores                                 | sPBHpS  |
| baden-wuerttemberg                          | Germany               | Baden-Württemberg                      | sPBHpS  |
| bangladesh                                  | Asia                  | Bangladesh                             | sPBHpS  |
| basse-normandie                             | France                | Basse-Normandie                        | sPBHpS  |
| bayern                                      | Germany               | Bayern                                 | sPBHpS  |
| belarus                                     | Europe                | Belarus                                | sPBHpS  |
| belgium                                     | Europe                | Belgium                                | sPBHpS  |
| belize                                      | Central America       | Belize                                 | sPBHpS  |
| benin                                       | Africa                | Benin                                  | sPBHpS  |
| berkshire                                   | England               | Berkshire                              | sPBHpS  |
| berlin                                      | Germany               | Berlin                                 | sPBHpS  |
| bhutan                                      | Asia                  | Bhutan                                 | sPBHpS  |
| bolivia                                     | South America         | Bolivia                                | sPBHpS  |
| bosnia-herzegovina                          | Europe                | Bosnia-Herzegovina                     | sPBHpS  |
| botswana                                    | Africa                | Botswana                               | sPBHpS  |
| bourgogne                                   | France                | Bourgogne                              | sPBHpS  |
| brandenburg                                 | Germany               | Brandenburg (mit Berlin)               | sPBHpS  |
| brazil                                      | South America         | Brazil                                 | sPBHpS  |
| bremen                                      | Germany               | Bremen                                 | sPBHpS  |
| bretagne                                    | France                | Bretagne                               | sPBHpS  |
| british-columbia                            | Canada                | British Columbia                       | sPBHpS  |
| british-isles                               | Europe                | British Isles                          | sPBHp   |
| buckinghamshire                             | England               | Buckinghamshire                        | sPBHpS  |
| bulgaria                                    | Europe                | Bulgaria                               | sPBHpS  |
| burkina-faso                                | Africa                | Burkina Faso                           | sPBHpS  |
| burundi                                     | Africa                | Burundi                                | sPBHpS  |
| california                                  | us                    | California                             | sPBHpS  |
| cambodia                                    | Asia                  | Cambodia                               | sPBHpS  |
| cambridgeshire                              | England               | Cambridgeshire                         | sPBHpS  |
| cameroon                                    | Africa                | Cameroon                               | sPBHpS  |
| canada                                      | North America         | Canada                                 | sPBHp   |
| canary-islands                              | Africa                | Canary Islands                         | sPBHpS  |
| cape-verde                                  | Africa                | Cape Verde                             | sPBHpS  |
| central-african-republic                    | Africa                | Central African Republic               | sPBHpS  |
| central-america                             |                       | Central America                        | sPBHp   |
| central-fed-district                        | Russian Federation    | Central Federal District               | sPBHpS  |
| centre                                      | France                | Centre                                 | sPBHpS  |
| centro                                      | Italy                 | Centro                                 | sPBHpS  |
| chad                                        | Africa                | Chad                                   | sPBHpS  |
| champagne-ardenne                           | France                | Champagne Ardenne                      | sPBHpS  |
| cheshire                                    | England               | Cheshire                               | sPBHpS  |
| chile                                       | South America         | Chile                                  | sPBHpS  |
| china                                       | Asia                  | China                                  | sPBHpS  |
| chubu                                       | Japan                 | Chūbu region                           | sPBHpS  |
| chugoku                                     | Japan                 | Chūgoku region                         | sPBHpS  |
| colombia                                    | South America         | Colombia                               | sPBHpS  |
| colorado                                    | us                    | Colorado                               | sPBHpS  |
| comores                                     | Africa                | Comores                                | sPBHpS  |
| congo-brazzaville                           | Africa                | Congo (Republic/Brazzaville)           | sPBHpS  |
| congo-democratic-republic                   | Africa                | Congo (Democratic                      | sPBHpS  |
|                                             |                       | Republic/Kinshasa)                     |         |
| connecticut                                 | us                    | Connecticut                            | sPBHpS  |
| cornwall                                    | England               | Cornwall                               | sPBHpS  |
| corse                                       | France                | Corse                                  | sPBHpS  |
| crimean-fed-district                        | Russian Federation    | Crimean Federal District               | sPBHpS  |
| croatia                                     | Europe                | Croatia                                | sPBHpS  |
| cuba                                        | Central America       | Cuba                                   | sPBHpS  |
| cumbria                                     | England               | Cumbria                                | sPBHpS  |
| cyprus                                      | Europe                | Cyprus                                 | sPBHpS  |
| czech-republic                              | Europe                | Czech Republic                         | sPBHpS  |
| dach                                        | Europe                | Germany, Austria, Switzerland          | sPBHp   |
| delaware                                    | us                    | Delaware                               | sPBHpS  |
| denmark                                     | Europe                | Denmark                                | sPBHpS  |
| derbyshire                                  | England               | Derbyshire                             | sPBHpS  |
| detmold-regbez                              | Nordrhein-Westfalen   | Regierungsbezirk Detmold               | sPBHpS  |
| devon                                       | England               | Devon                                  | sPBHpS  |
| district-of-columbia                        | us                    | District of Columbia                   | sPBHpS  |
| djibouti                                    | Africa                | Djibouti                               | sPBHpS  |
| dolnoslaskie                                | Poland                | Województwo dolnośląskie(Lower         | sPBHpS  |
|                                             |                       | Silesian Voivodeship)                  |         |
| dorset                                      | England               | Dorset                                 | sPBHpS  |
| duesseldorf-regbez                          | Nordrhein-Westfalen   | Regierungsbezirk Düsseldorf            | sPBHpS  |
| east-sussex                                 | England               | East Sussex                            | sPBHpS  |
| east-yorkshire-with-hull                    | England               | East Yorkshire with Hull               | sPBHpS  |
| ecuador                                     | South America         | Ecuador                                | sPBHp   |
| egypt                                       | Africa                | Egypt                                  | sPBHpS  |
| england                                     | Great Britain         | England                                | sPBHpS  |
| equatorial-guinea                           | Africa                | Equatorial Guinea                      | sPBHpS  |
| eritrea                                     | Africa                | Eritrea                                | sPBHpS  |
| essex                                       | England               | Essex                                  | sPBHpS  |
| estonia                                     | Europe                | Estonia                                | sPBHpS  |
| ethiopia                                    | Africa                | Ethiopia                               | sPBHpS  |
| europe                                      |                       | Europe                                 | sPBHp   |
| far-eastern-fed-district                    | Russian Federation    | Far Eastern Federal District           | sPBHpS  |
| faroe-islands                               | Europe                | Faroe Islands                          | sPBHpS  |
| fiji                                        | Australia and Oceania | Fiji                                   | sPBHpS  |
| finland                                     | Europe                | Finland                                | sPBHpS  |
| florida                                     | us                    | Florida                                | sPBHpS  |
| france                                      | Europe                | France                                 | sPBHp   |
| franche-comte                               | France                | Franche Comte                          | sPBHpS  |
| freiburg-regbez                             | Baden-Württemberg     | Regierungsbezirk Freiburg              | sPBHpS  |
| gabon                                       | Africa                | Gabon                                  | sPBHpS  |
| gcc-states                                  | Asia                  | GCC States                             | sPBHpS  |
| georgia-eu                                  | Europe                | Georgia (Europe country)               | sPBHpS  |
| georgia-us                                  | us                    | Georgia (US State)                     | sPBHpS  |
| germany                                     | Europe                | Germany                                | sPBHp   |
| ghana                                       | Africa                | Ghana                                  | sPBHpS  |
| gloucestershire                             | England               | Gloucestershire                        | sPBHpS  |
| great-britain                               | Europe                | Great Britain                          | sPBHp   |
| greater-london                              | England               | Greater London                         | sPBHpS  |
| greater-manchester                          | England               | Greater Manchester                     | sPBHpS  |
| greece                                      | Europe                | Greece                                 | sPBHpS  |
| greenland                                   | North America         | Greenland                              | sPBHpS  |
| guadeloupe                                  | France                | Guadeloupe                             | sPBHp   |
| guatemala                                   | Central America       | Guatemala                              | sPBHpS  |
| guinea                                      | Africa                | Guinea                                 | sPBHpS  |
| guinea-bissau                               | Africa                | Guinea-Bissau                          | sPBHpS  |
| guyane                                      | France                | Guyane                                 | sPBHp   |
| haiti-and-domrep                            | Central America       | Haiti and Dominican Republic           | sPBHpS  |
| hamburg                                     | Germany               | Hamburg                                | sPBHpS  |
| hampshire                                   | England               | Hampshire                              | sPBHpS  |
| haute-normandie                             | France                | Haute-Normandie                        | sPBHpS  |
| hawaii                                      | us                    | Hawaii                                 | sPBHpS  |
| herefordshire                               | England               | Herefordshire                          | sPBHpS  |
| hertfordshire                               | England               | Hertfordshire                          | sPBHpS  |
| hessen                                      | Germany               | Hessen                                 | sPBHpS  |
| hokkaido                                    | Japan                 | Hokkaidō                               | sPBHpS  |
| hungary                                     | Europe                | Hungary                                | sPBHpS  |
| iceland                                     | Europe                | Iceland                                | sPBHpS  |
| idaho                                       | us                    | Idaho                                  | sPBHpS  |
| ile-de-france                               | France                | Ile-de-France                          | sPBHpS  |
| illinois                                    | us                    | Illinois                               | sPBHpS  |
| india                                       | Asia                  | India                                  | sPBHpS  |
| indiana                                     | us                    | Indiana                                | sPBHpS  |
| indonesia                                   | Asia                  | Indonesia                              | sPBHpS  |
| iowa                                        | us                    | Iowa                                   | sPBHpS  |
| iran                                        | Asia                  | Iran                                   | sPBHpS  |
| iraq                                        | Asia                  | Iraq                                   | sPBHpS  |
| ireland-and-northern-ireland                | Europe                | Ireland and Northern Ireland           | sPBHpS  |
| isle-of-man                                 | Europe                | Isle of Man                            | sPBHpS  |
| isle-of-wight                               | England               | Isle of Wight                          | sPBHpS  |
| isole                                       | Italy                 | Isole                                  | sPBHpS  |
| israel-and-palestine                        | Asia                  | Israel and Palestine                   | sPBHpS  |
| italy                                       | Europe                | Italy                                  | sPBHp   |
| ivory-coast                                 | Africa                | Ivory Coast                            | sPBHpS  |
| jamaica                                     | Central America       | jamaica                                | sPBHpS  |
| japan                                       | Asia                  | Japan                                  | sPBHp   |
| jordan                                      | Asia                  | Jordan                                 | sPBHpS  |
| kaliningrad                                 | Russian Federation    | Kaliningrad                            | sPBHpS  |
| kansai                                      | Japan                 | Kansai region (a.k.a. Kinki            | sPBHpS  |
|                                             |                       | region)                                |         |
| kansas                                      | us                    | Kansas                                 | sPBHpS  |
| kanto                                       | Japan                 | Kantō region                           | sPBHpS  |
| karlsruhe-regbez                            | Baden-Württemberg     | Regierungsbezirk Karlsruhe             | sPBHpS  |
| kazakhstan                                  | Asia                  | Kazakhstan                             | sPBHpS  |
| kent                                        | England               | Kent                                   | sPBHpS  |
| kentucky                                    | us                    | Kentucky                               | sPBHpS  |
| kenya                                       | Africa                | Kenya                                  | sPBHpS  |
| koeln-regbez                                | Nordrhein-Westfalen   | Regierungsbezirk Köln                  | sPBHpS  |
| kosovo                                      | Europe                | Kosovo                                 | sPBHpS  |
| kujawsko-pomorskie                          | Poland                | Województwo                            | sPBHpS  |
|                                             |                       | kujawsko-pomorskie(Kuyavian-Pomeranian |         |
|                                             |                       | Voivodeship)                           |         |
| kyrgyzstan                                  | Asia                  | Kyrgyzstan                             | sPBHpS  |
| kyushu                                      | Japan                 | Kyūshū                                 | sPBHpS  |
| lancashire                                  | England               | Lancashire                             | sPBHpS  |
| languedoc-roussillon                        | France                | Languedoc-Roussillon                   | sPBHpS  |
| laos                                        | Asia                  | Laos                                   | sPBHpS  |
| latvia                                      | Europe                | Latvia                                 | sPBHpS  |
| lebanon                                     | Asia                  | Lebanon                                | sPBHpS  |
| leicestershire                              | England               | Leicestershire                         | sPBHpS  |
| lesotho                                     | Africa                | Lesotho                                | sPBHpS  |
| liberia                                     | Africa                | Liberia                                | sPBHpS  |
| libya                                       | Africa                | Libya                                  | sPBHpS  |
| liechtenstein                               | Europe                | Liechtenstein                          | sPBHpS  |
| limousin                                    | France                | Limousin                               | sPBHpS  |
| lithuania                                   | Europe                | Lithuania                              | sPBHpS  |
| lodzkie                                     | Poland                | Województwo łódzkie(Łódź Voivodeship)  | sPBHpS  |
| lorraine                                    | France                | Lorraine                               | sPBHpS  |
| louisiana                                   | us                    | Louisiana                              | sPBHpS  |
| lubelskie                                   | Poland                | Województwo lubelskie(Lublin           | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| lubuskie                                    | Poland                | Województwo lubuskie(Lubusz            | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| luxembourg                                  | Europe                | Luxembourg                             | sPBHpS  |
| macedonia                                   | Europe                | Macedonia                              | sPBHpS  |
| madagascar                                  | Africa                | Madagascar                             | sPBHpS  |
| maine                                       | us                    | Maine                                  | sPBHpS  |
| malawi                                      | Africa                | Malawi                                 | sPBHpS  |
| malaysia-singapore-brunei                   | Asia                  | Malaysia, Singapore, and Brunei        | sPBHp   |
| maldives                                    | Asia                  | Maldives                               | sPBHpS  |
| mali                                        | Africa                | Mali                                   | sPBHpS  |
| malopolskie                                 | Poland                | Województwo małopolskie(Lesser Poland  | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| malta                                       | Europe                | Malta                                  | sPBHpS  |
| manitoba                                    | Canada                | Manitoba                               | sPBHpS  |
| martinique                                  | France                | Martinique                             | sPBHp   |
| maryland                                    | us                    | Maryland                               | sPBHpS  |
| massachusetts                               | us                    | Massachusetts                          | sPBHpS  |
| mauritania                                  | Africa                | Mauritania                             | sPBHpS  |
| mauritius                                   | Africa                | Mauritius                              | sPBHpS  |
| mayotte                                     | France                | Mayotte                                | sPBHp   |
| mazowieckie                                 | Poland                | Województwo mazowieckie(Mazovian       | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| mecklenburg-vorpommern                      | Germany               | Mecklenburg-Vorpommern                 | sPBHpS  |
| mexico                                      | North America         | Mexico                                 | sPBHpS  |
| michigan                                    | us                    | Michigan                               | sPBHpS  |
| midi-pyrenees                               | France                | Midi-Pyrenees                          | sPBHpS  |
| minnesota                                   | us                    | Minnesota                              | sPBHpS  |
| mississippi                                 | us                    | Mississippi                            | sPBHpS  |
| missouri                                    | us                    | Missouri                               | sPBHpS  |
| mittelfranken                               | Bayern                | Mittelfranken                          | sPBHpS  |
| moldova                                     | Europe                | Moldova                                | sPBHpS  |
| monaco                                      | Europe                | Monaco                                 | sPBHpS  |
| mongolia                                    | Asia                  | Mongolia                               | sPBHpS  |
| montana                                     | us                    | Montana                                | sPBHpS  |
| montenegro                                  | Europe                | Montenegro                             | sPBHpS  |
| morocco                                     | Africa                | Morocco                                | sPBHpS  |
| mozambique                                  | Africa                | Mozambique                             | sPBHpS  |
| muenster-regbez                             | Nordrhein-Westfalen   | Regierungsbezirk Münster               | sPBHpS  |
| myanmar                                     | Asia                  | Myanmar (a.k.a. Burma)                 | sPBHpS  |
| namibia                                     | Africa                | Namibia                                | sPBHpS  |
| nebraska                                    | us                    | Nebraska                               | sPBHpS  |
| nepal                                       | Asia                  | Nepal                                  | sPBHpS  |
| netherlands                                 | Europe                | Netherlands                            | sPBHpS  |
| nevada                                      | us                    | Nevada                                 | sPBHpS  |
| new-brunswick                               | Canada                | New Brunswick                          | sPBHpS  |
| new-caledonia                               | Australia and Oceania | New Caledonia                          | sPBHpS  |
| new-hampshire                               | us                    | New Hampshire                          | sPBHpS  |
| new-jersey                                  | us                    | New Jersey                             | sPBHpS  |
| new-mexico                                  | us                    | New Mexico                             | sPBHpS  |
| new-york                                    | us                    | New York                               | sPBHpS  |
| new-zealand                                 | Australia and Oceania | New Zealand                            | sPBHpS  |
| newfoundland-and-labrador                   | Canada                | Newfoundland and Labrador              | sPBHpS  |
| nicaragua                                   | Central America       | Nicaragua                              | sPBHp   |
| niederbayern                                | Bayern                | Niederbayern                           | sPBHpS  |
| niedersachsen                               | Germany               | Niedersachsen                          | sPBHpS  |
| niger                                       | Africa                | Niger                                  | sPBHpS  |
| nigeria                                     | Africa                | Nigeria                                | sPBHpS  |
| nord-est                                    | Italy                 | Nord-Est                               | sPBHpS  |
| nord-ovest                                  | Italy                 | Nord-Ovest                             | sPBHpS  |
| nord-pas-de-calais                          | France                | Nord-Pas-de-Calais                     | sPBHpS  |
| nordrhein-westfalen                         | Germany               | Nordrhein-Westfalen                    | sPBHpS  |
| norfolk                                     | England               | Norfolk                                | sPBHpS  |
| north-america                               |                       | North America                          | sPBHp   |
| north-carolina                              | us                    | North Carolina                         | sPBHpS  |
| north-caucasus-fed-district                 | Russian Federation    | North Caucasus Federal District        | sPBHpS  |
| north-dakota                                | us                    | North Dakota                           | sPBHpS  |
| north-korea                                 | Asia                  | North Korea                            | sPBHpS  |
| north-yorkshire                             | England               | North Yorkshire                        | sPBHpS  |
| northumberland                              | England               | Northumberland                         | sPBHpS  |
| northwest-territories                       | Canada                | Northwest Territories                  | sPBHpS  |
| northwestern-fed-district                   | Russian Federation    | Northwestern Federal District          | sPBHpS  |
| norway                                      | Europe                | Norway                                 | sPBHpS  |
| nottinghamshire                             | England               | Nottinghamshire                        | sPBHpS  |
| nova-scotia                                 | Canada                | Nova Scotia                            | sPBHpS  |
| nunavut                                     | Canada                | Nunavut                                | sPBHpS  |
| oberbayern                                  | Bayern                | Oberbayern                             | sPBHpS  |
| oberfranken                                 | Bayern                | Oberfranken                            | sPBHpS  |
| oberpfalz                                   | Bayern                | Oberpfalz                              | sPBHpS  |
| ohio                                        | us                    | Ohio                                   | sPBHpS  |
| oklahoma                                    | us                    | Oklahoma                               | sPBHpS  |
| ontario                                     | Canada                | Ontario                                | sPBHpS  |
| opolskie                                    | Poland                | Województwo opolskie(Opole             | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| oregon                                      | us                    | Oregon                                 | sPBHpS  |
| oxfordshire                                 | England               | Oxfordshire                            | sPBHpS  |
| pakistan                                    | Asia                  | Pakistan                               | sPBHpS  |
| papua-new-guinea                            | Australia and Oceania | Papua New Guinea                       | sPBHpS  |
| paraguay                                    | South America         | Paraguay                               | sPBHpS  |
| pays-de-la-loire                            | France                | Pays de la Loire                       | sPBHpS  |
| pennsylvania                                | us                    | Pennsylvania                           | sPBHpS  |
| peru                                        | South America         | Peru                                   | sPBHpS  |
| philippines                                 | Asia                  | Philippines                            | sPBHpS  |
| picardie                                    | France                | Picardie                               | sPBHpS  |
| podkarpackie                                | Poland                | Województwo podkarpackie(Subcarpathian | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| podlaskie                                   | Poland                | Województwo podlaskie(Podlaskie        | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| poitou-charentes                            | France                | Poitou-Charentes                       | sPBHpS  |
| poland                                      | Europe                | Poland                                 | sPBHp   |
| pomorskie                                   | Poland                | Województwo pomorskie(Pomeranian       | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| portugal                                    | Europe                | Portugal                               | sPBHpS  |
| prince-edward-island                        | Canada                | Prince Edward Island                   | sPBHpS  |
| provence-alpes-cote-d-azur                  | France                | Provence Alpes-Cote-d'Azur             | sPBHpS  |
| puerto-rico                                 | us                    | Puerto Rico                            | sPBHpS  |
| quebec                                      | Canada                | Quebec                                 | sPBHpS  |
| reunion                                     | France                | Reunion                                | sPBHp   |
| rheinland-pfalz                             | Germany               | Rheinland-Pfalz                        | sPBHpS  |
| rhode-island                                | us                    | Rhode Island                           | sPBHpS  |
| rhone-alpes                                 | France                | Rhone-Alpes                            | sPBHpS  |
| romania                                     | Europe                | Romania                                | sPBHpS  |
| russia                                      |                       | Russian Federation                     | sPBHp   |
| rwanda                                      | Africa                | Rwanda                                 | sPBHpS  |
| saarland                                    | Germany               | Saarland                               | sPBHpS  |
| sachsen                                     | Germany               | Sachsen                                | sPBHpS  |
| sachsen-anhalt                              | Germany               | Sachsen-Anhalt                         | sPBHpS  |
| saint-helena-ascension-and-tristan-da-cunha | Africa                | Saint Helena, Ascension, and Tristan   | sPBHpS  |
|                                             |                       | da Cunha                               |         |
| sao-tome-and-principe                       | Africa                | Sao Tome and Principe                  | sPBHpS  |
| saskatchewan                                | Canada                | Saskatchewan                           | sPBHpS  |
| schleswig-holstein                          | Germany               | Schleswig-Holstein                     | sPBHpS  |
| schwaben                                    | Bayern                | Schwaben                               | sPBHpS  |
| scotland                                    | Great Britain         | Scotland                               | sPBHpS  |
| senegal-and-gambia                          | Africa                | Senegal and Gambia                     | sPBHpS  |
| serbia                                      | Europe                | Serbia                                 | sPBHpS  |
| seychelles                                  | Africa                | Seychelles                             | sPBHpS  |
| shikoku                                     | Japan                 | Shikoku                                | sPBHpS  |
| shropshire                                  | England               | Shropshire                             | sPBHpS  |
| siberian-fed-district                       | Russian Federation    | Siberian Federal District              | sPBHpS  |
| sierra-leone                                | Africa                | Sierra Leone                           | sPBHpS  |
| slaskie                                     | Poland                | Województwo śląskie(Silesian           | sPBHpS  |
|                                             |                       | Voivodeship)                           |         |
| slovakia                                    | Europe                | Slovakia                               | sPBHpS  |
| slovenia                                    | Europe                | Slovenia                               | sPBHpS  |
| somalia                                     | Africa                | Somalia                                | sPBHpS  |
| somerset                                    | England               | Somerset                               | sPBHpS  |
| south-africa                                | Africa                | South Africa                           | sPBHpS  |
| south-africa-and-lesotho                    | Africa                | South Africa (includes Lesotho)        | sPBHp   |
| south-america                               |                       | South America                          | sPBHp   |
| south-carolina                              | us                    | South Carolina                         | sPBHpS  |
| south-dakota                                | us                    | South Dakota                           | sPBHpS  |
| south-fed-district                          | Russian Federation    | South Federal District                 | sPBHpS  |
| south-korea                                 | Asia                  | South Korea                            | sPBHpS  |
| south-sudan                                 | Africa                | South Sudan                            | sPBHpS  |
| south-yorkshire                             | England               | South Yorkshire                        | sPBHpS  |
| spain                                       | Europe                | Spain                                  | sPBHpS  |
| sri-lanka                                   | Asia                  | Sri Lanka                              | sPBHpS  |
| staffordshire                               | England               | Staffordshire                          | sPBHpS  |
| stuttgart-regbez                            | Baden-Württemberg     | Regierungsbezirk Stuttgart             | sPBHpS  |
| sud                                         | Italy                 | Sud                                    | sPBHpS  |
| sudan                                       | Africa                | Sudan                                  | sPBHpS  |
| suffolk                                     | England               | Suffolk                                | sPBHpS  |
| suriname                                    | South America         | suriname                               | sPBHpS  |
| surrey                                      | England               | Surrey                                 | sPBHpS  |
| swaziland                                   | Africa                | Swaziland                              | sPBHpS  |
| sweden                                      | Europe                | Sweden                                 | sPBHpS  |
| swietokrzyskie                              | Poland                | Województwo                            | sPBHpS  |
|                                             |                       | świętokrzyskie(Świętokrzyskie          |         |
|                                             |                       | Voivodeship)                           |         |
| switzerland                                 | Europe                | Switzerland                            | sPBHpS  |
| syria                                       | Asia                  | Syria                                  | sPBHpS  |
| taiwan                                      | Asia                  | Taiwan                                 | sPBHpS  |
| tajikistan                                  | Asia                  | Tajikistan                             | sPBHp   |
| tanzania                                    | Africa                | Tanzania                               | sPBHpS  |
| tennessee                                   | us                    | Tennessee                              | sPBHpS  |
| texas                                       | us                    | Texas                                  | sPBHpS  |
| thailand                                    | Asia                  | Thailand                               | sPBHpS  |
| thueringen                                  | Germany               | Thüringen                              | sPBHpS  |
| togo                                        | Africa                | Togo                                   | sPBHpS  |
| tohoku                                      | Japan                 | Tōhoku region                          | sPBHpS  |
| tuebingen-regbez                            | Baden-Württemberg     | Regierungsbezirk Tübingen              | sPBHpS  |
| tunisia                                     | Africa                | Tunisia                                | sPBHpS  |
| turkey                                      | Europe                | Turkey                                 | sPBHpS  |
| turkmenistan                                | Asia                  | Turkmenistan                           | sPBHpS  |
| uganda                                      | Africa                | Uganda                                 | sPBHpS  |
| ukraine                                     | Europe                | Ukraine                                | sPBHpS  |
| unterfranken                                | Bayern                | Unterfranken                           | sPBHpS  |
| ural-fed-district                           | Russian Federation    | Ural Federal District                  | sPBHpS  |
| uruguay                                     | South America         | Uruguay                                | sPBHpS  |
| us                                          | North America         | us                                     |         |
| us-midwest                                  | North America         | US Midwest                             | sPBHp   |
| us-northeast                                | North America         | US Northeast                           | sPBHp   |
| us-pacific                                  | North America         | US Pacific                             | sPBHp   |
| us-south                                    | North America         | US South                               | sPBHp   |
| us-west                                     | North America         | US West                                | sPBHp   |
| utah                                        | us                    | Utah                                   | sPBHpS  |
| uzbekistan                                  | Asia                  | Uzbekistan                             | sPBHpS  |
| vermont                                     | us                    | Vermont                                | sPBHpS  |
| vietnam                                     | Asia                  | Vietnam                                | sPBHpS  |
| virginia                                    | us                    | Virginia                               | sPBHpS  |
| volga-fed-district                          | Russian Federation    | Volga Federal District                 | sPBHpS  |
| wales                                       | Great Britain         | Wales                                  | sPBHpS  |
| warminsko-mazurskie                         | Poland                | Województwo                            | sPBHpS  |
|                                             |                       | warmińsko-mazurskie(Warmian-Masurian   |         |
|                                             |                       | Voivodeship)                           |         |
| washington                                  | us                    | Washington                             | sPBHpS  |
| west-midlands                               | England               | West Midlands                          | sPBHpS  |
| west-sussex                                 | England               | West Sussex                            | sPBHpS  |
| west-virginia                               | us                    | West Virginia                          | sPBHpS  |
| west-yorkshire                              | England               | West Yorkshire                         | sPBHpS  |
| wielkopolskie                               | Poland                | Województwo wielkopolskie(Greater      | sPBHpS  |
|                                             |                       | Poland Voivodeship)                    |         |
| wiltshire                                   | England               | Wiltshire                              | sPBHpS  |
| wisconsin                                   | us                    | Wisconsin                              | sPBHpS  |
| worcestershire                              | England               | worcestershire                         | sPBHpS  |
| wyoming                                     | us                    | Wyoming                                | sPBHpS  |
| yemen                                       | Asia                  | Yemen                                  | sPBHpS  |
| yukon                                       | Canada                | Yukon                                  | sPBHpS  |
| zachodniopomorskie                          | Poland                | Województwo zachodniopomorskie(West    | sPBHpS  |
|                                             |                       | Pomeranian Voivodeship)                |         |
| zambia                                      | Africa                | Zambia                                 | sPBHpS  |
| zimbabwe                                    | Africa                | Zimbabwe                               | sPBHpS  |
