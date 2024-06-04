# SQLHomeworkP2

mysql> SELECT COUNT(*) AS USACitiesCount
    -> FROM city
    -> WHERE CountryCode = 'USA';
+----------------+
| USACitiesCount |
+----------------+
|            274 |
+----------------+
1 row in set (0.04 sec)

mysql> SELECT Population, LifeExpectancy
    -> FROM country
    -> WHERE Code = 'ARG';
+------------+----------------+
| Population | LifeExpectancy |
+------------+----------------+
|   37032000 |           75.1 |
+------------+----------------+
1 row in set (0.01 sec)

mysql> SELECT Name
    -> FROM city
    -> WHERE CountryCode = 'FRA';
+----------------------+
| Name                 |
+----------------------+
| Paris                |
| Marseille            |
| Lyon                 |
| Toulouse             |
| Nice                 |
| Nantes               |
| Strasbourg           |
| Montpellier          |
| Bordeaux             |
| Rennes               |
| Le Havre             |
| Reims                |
| Lille                |
| St-Étienne           |
| Toulon               |
| Grenoble             |
| Angers               |
| Dijon                |
| Brest                |
| Le Mans              |
| Clermont-Ferrand     |
| Amiens               |
| Aix-en-Provence      |
| Limoges              |
| Nîmes                |
| Tours                |
| Villeurbanne         |
| Metz                 |
| Besançon             |
| Caen                 |
| Orléans              |
| Mulhouse             |
| Rouen                |
| Boulogne-Billancourt |
| Perpignan            |
| Nancy                |
| Roubaix              |
| Argenteuil           |
| Tourcoing            |
| Montreuil            |
+----------------------+
40 rows in set (0.00 sec)

mysql> SELECT Name, Population
    -> FROM city
    -> ORDER BY Population DESC
    -> LIMIT 5;
+-----------------+------------+
| Name            | Population |
+-----------------+------------+
| Mumbai (Bombay) |   10500000 |
| Seoul           |    9981619 |
| São Paulo       |    9968485 |
| Shanghai        |    9696300 |
| Jakarta         |    9604900 |
+-----------------+------------+
5 rows in set (0.01 sec)

mysql> -- List every unique world language.
mysql> SELECT DISTINCT Language
    -> FROM countrylanguage;
+---------------------------+
| Language                  |
+---------------------------+
| Dutch                     |
| English                   |
| Papiamento                |
| Spanish                   |
| Balochi                   |
| Dari                      |
| Pashto                    |
| Turkmenian                |
| Uzbek                     |
| Ambo                      |
| Chokwe                    |
| Kongo                     |
| Luchazi                   |
| Luimbe-nganguela          |
| Luvale                    |
| Mbundu                    |
| Nyaneka-nkhumbi           |
| Ovimbundu                 |
| Albaniana                 |
| Greek                     |
| Macedonian                |
| Catalan                   |
| French                    |
| Portuguese                |
| Arabic                    |
| Hindi                     |
| Indian Languages          |
| Italian                   |
| Armenian                  |
| Azerbaijani               |
| Samoan                    |
| Tongan                    |
| Creole English            |
| Canton Chinese            |
| German                    |
| Serbo-Croatian            |
| Vietnamese                |
| Czech                     |
| Hungarian                 |
| Polish                    |
| Romanian                  |
| Slovene                   |
| Turkish                   |
| Lezgian                   |
| Russian                   |
| Kirundi                   |
| Swahili                   |
| Adja                      |
| Aizo                      |
| Bariba                    |
| Fon                       |
| Ful                       |
| Joruba                    |
| Somba                     |
| Busansi                   |
| Dagara                    |
| Dyula                     |
| Gurma                     |
| Mossi                     |
| Bengali                   |
| Chakma                    |
| Garo                      |
| Khasi                     |
| Marma                     |
| Santhali                  |
| Tripuri                   |
| Bulgariana                |
| Romani                    |
| Creole French             |
| Belorussian               |
| Ukrainian                 |
| Garifuna                  |
| Maya Languages            |
| Aimará                    |
| Guaraní                   |
| Ket?ua                    |
| Japanese                  |
| Bajan                     |
| Chinese                   |
| Malay                     |
| Malay-English             |
| Asami                     |
| Dzongkha                  |
| Nepali                    |
| Khoekhoe                  |
| Ndebele                   |
| San                       |
| Shona                     |
| Tswana                    |
| Banda                     |
| Gbaya                     |
| Mandjia                   |
| Mbum                      |
| Ngbaka                    |
| Sara                      |
| Eskimo Languages          |
| Punjabi                   |
| Romansh                   |
| Araucan                   |
| Rapa nui                  |
| Dong                      |
| Hui                       |
| Mant?u                    |
| Miao                      |
| Mongolian                 |
| Puyi                      |
| Tibetan                   |
| Tujia                     |
| Uighur                    |
| Yi                        |
| Zhuang                    |
| [South]Mande              |
| Akan                      |
| Gur                       |
| Kru                       |
| Malinke                   |
| Bamileke-bamum            |
| Duala                     |
| Fang                      |
| Maka                      |
| Mandara                   |
| Masana                    |
| Tikar                     |
| Boa                       |
| Luba                      |
| Mongo                     |
| Ngala and Bangi           |
| Rundi                     |
| Rwanda                    |
| Teke                      |
| Zande                     |
| Mbete                     |
| Mboshi                    |
| Punu                      |
| Sango                     |
| Maori                     |
| Arawakan                  |
| Caribbean                 |
| Chibcha                   |
| Comorian                  |
| Comorian-Arabic           |
| Comorian-French           |
| Comorian-madagassi        |
| Comorian-Swahili          |
| Crioulo                   |
| Moravian                  |
| Silesiana                 |
| Slovak                    |
| Southern Slavic Languages |
| Afar                      |
| Somali                    |
| Danish                    |
| Norwegian                 |
| Swedish                   |
| Berberi                   |
| Sinaberberi               |
| Bilin                     |
| Hadareb                   |
| Saho                      |
| Tigre                     |
| Tigrinja                  |
| Basque                    |
| Galecian                  |
| Estonian                  |
| Finnish                   |
| Amhara                    |
| Gurage                    |
| Oromo                     |
| Sidamo                    |
| Walaita                   |
| Saame                     |
| Fijian                    |
| Faroese                   |
| Kosrean                   |
| Mortlock                  |
| Pohnpei                   |
| Trukese                   |
| Wolea                     |
| Yap                       |
| Mpongwe                   |
| Punu-sira-nzebi           |
| Gaeli                     |
| Kymri                     |
| Abhyasi                   |
| Georgiana                 |
| Osseetti                  |
| Ewe                       |
| Ga-adangme                |
| Kissi                     |
| Kpelle                    |
| Loma                      |
| Susu                      |
| Yalunka                   |
| Diola                     |
| Soninke                   |
| Wolof                     |
| Balante                   |
| Mandyako                  |
| Bubi                      |
| Greenlandic               |
| Cakchiquel                |
| Kekchí                    |
| Mam                       |
| Quiché                    |
| Chamorro                  |
| Korean                    |
| Philippene Languages      |
| Chiu chau                 |
| Fukien                    |
| Hakka                     |
| Miskito                   |
| Haiti Creole              |
| Bali                      |
| Banja                     |
| Batakki                   |
| Bugi                      |
| Javanese                  |
| Madura                    |
| Minangkabau               |
| Sunda                     |
| Gujarati                  |
| Kannada                   |
| Malajalam                 |
| Marathi                   |
| Orija                     |
| Tamil                     |
| Telugu                    |
| Urdu                      |
| Irish                     |
| Bakhtyari                 |
| Gilaki                    |
| Kurdish                   |
| Luri                      |
| Mazandarani               |
| Persian                   |
| Assyrian                  |
| Icelandic                 |
| Hebrew                    |
| Friuli                    |
| Sardinian                 |
| Circassian                |
| Ainu                      |
| Kazakh                    |
| Tatar                     |
| Gusii                     |
| Kalenjin                  |
| Kamba                     |
| Kikuyu                    |
| Luhya                     |
| Luo                       |
| Masai                     |
| Meru                      |
| Nyika                     |
| Turkana                   |
| Kirgiz                    |
| Tadzhik                   |
| Khmer                     |
| T?am                      |
| Kiribati                  |
| Tuvalu                    |
| Lao                       |
| Lao-Soung                 |
| Mon-khmer                 |
| Thai                      |
| Bassa                     |
| Gio                       |
| Grebo                     |
| Mano                      |
| Mixed Languages           |
| Singali                   |
| Sotho                     |
| Zulu                      |
| Lithuanian                |
| Luxembourgish             |
| Latvian                   |
| Mandarin Chinese          |
| Monegasque                |
| Gagauzi                   |
| Malagasy                  |
| Dhivehi                   |
| Mixtec                    |
| Náhuatl                   |
| Otomí                     |
| Yucatec                   |
| Zapotec                   |
| Marshallese               |
| Bambara                   |
| Senufo and Minianka       |
| Songhai                   |
| Tamashek                  |
| Maltese                   |
| Burmese                   |
| Chin                      |
| Kachin                    |
| Karen                     |
| Kayah                     |
| Mon                       |
| Rakhine                   |
| Shan                      |
| Bajad                     |
| Buryat                    |
| Dariganga                 |
| Dorbet                    |
| Carolinian                |
| Chuabo                    |
| Lomwe                     |
| Makua                     |
| Marendje                  |
| Nyanja                    |
| Ronga                     |
| Sena                      |
| Tsonga                    |
| Tswa                      |
| Hassaniya                 |
| Tukulor                   |
| Zenaga                    |
| Bhojpuri                  |
| Chichewa                  |
| Ngoni                     |
| Yao                       |
| Dusun                     |
| Iban                      |
| Mahoré                    |
| Afrikaans                 |
| Caprivi                   |
| Herero                    |
| Kavango                   |
| Nama                      |
| Ovambo                    |
| Malenasian Languages      |
| Polynesian Languages      |
| Hausa                     |
| Kanuri                    |
| Songhai-zerma             |
| Bura                      |
| Edo                       |
| Ibibio                    |
| Ibo                       |
| Ijo                       |
| Tiv                       |
| Sumo                      |
| Niue                      |
| Fries                     |
| Maithili                  |
| Newari                    |
| Tamang                    |
| Tharu                     |
| Nauru                     |
| Brahui                    |
| Hindko                    |
| Saraiki                   |
| Sindhi                    |
| Cuna                      |
| Embera                    |
| Guaymí                    |
| Pitcairnese               |
| Bicol                     |
| Cebuano                   |
| Hiligaynon                |
| Ilocano                   |
| Maguindanao               |
| Maranao                   |
| Pampango                  |
| Pangasinan                |
| Pilipino                  |
| Waray-waray               |
| Palau                     |
| Papuan Languages          |
| Tahitian                  |
| Avarian                   |
| Bashkir                   |
| Chechen                   |
| Chuvash                   |
| Mari                      |
| Mordva                    |
| Udmur                     |
| Bari                      |
| Beja                      |
| Chilluk                   |
| Dinka                     |
| Fur                       |
| Lotuko                    |
| Nubian Languages          |
| Nuer                      |
| Serer                     |
| Bullom-sherbro            |
| Kono-vai                  |
| Kuranko                   |
| Limba                     |
| Mende                     |
| Temne                     |
| Nahua                     |
| Sranantonga               |
| Czech and Moravian        |
| Ukrainian and Russian     |
| Swazi                     |
| Seselwa                   |
| Gorane                    |
| Hadjarai                  |
| Kanem-bornu               |
| Mayo-kebbi                |
| Ouaddai                   |
| Tandjile                  |
| Ane                       |
| Kabyé                     |
| Kotokoli                  |
| Moba                      |
| Naudemba                  |
| Watyi                     |
| Kuy                       |
| Tokelau                   |
| Arabic-French             |
| Arabic-French-English     |
| Ami                       |
| Atayal                    |
| Min                       |
| Paiwan                    |
| Chaga and Pare            |
| Gogo                      |
| Ha                        |
| Haya                      |
| Hehet                     |
| Luguru                    |
| Makonde                   |
| Nyakusa                   |
| Nyamwesi                  |
| Shambala                  |
| Acholi                    |
| Ganda                     |
| Gisu                      |
| Kiga                      |
| Lango                     |
| Lugbara                   |
| Nkole                     |
| Soga                      |
| Teso                      |
| Tagalog                   |
| Karakalpak                |
| Goajiro                   |
| Warrau                    |
| Man                       |
| Muong                     |
| Nung                      |
| Tho                       |
| Bislama                   |
| Futuna                    |
| Wallis                    |
| Samoan-English            |
| Soqutri                   |
| Northsotho                |
| Southsotho                |
| Venda                     |
| Xhosa                     |
| Bemba                     |
| Chewa                     |
| Lozi                      |
| Nsenga                    |
+---------------------------+
457 rows in set (0.01 sec)
