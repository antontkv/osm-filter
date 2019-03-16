# Filter OSM files by custom area

This is a tool for extracting address and coordinates of the buildings from .osm file. But OpenStreetMap doesn't allow you to choose custom shape for import, only square shape, so with that tool you can create a shape of the area that you need in Yandex Maps, and it will filter out all the buildings that outside of this shape.

# Usage

First argument should a path to .osm file, second path to the .geojson file from Yandex Maps with the coordinates of the custom shape.

`python main.py [osm file] [geoJson file]`

Example of .geojson file:

```json
{"type":"FeatureCollection","metadata":{"name":"Без названия","creator":"Yandex Map Constructor"},"features":[{"type":"Feature","id":0,"geometry":{"type":"Polygon","coordinates":[[[55.12287586791966,51.762607093170594],[55.122414527969084,51.76253386120151],[55.12211412055935,51.762287534610444],[55.11907785995453,51.761155746414914],[55.11801458657766,51.76203266314263],[55.11810065093858,51.76233463681616],[55.11603621827392,51.76428643090953],[55.111067895058675,51.76973228466188],[55.10783410434231,51.77438515854291],[55.10381554825519,51.77591276489537],[55.10330280548439,51.7760276462115],[55.10216901643668,51.77193189479633],[55.102216460443245,51.77110530585406],[55.0992802197723,51.77105590910171],[55.09808568475629,51.77098628134899],[55.09685896323218,51.77085674751459],[55.095796659014134,51.77056689350851],[55.09476274727166,51.769836208641344],[55.09270495233663,51.76879522912351],[55.090033712513545,51.76666611020025],[55.088612261913426,51.76562814088939],[55.088328067935926,51.7654821971523],[55.08895104987841,51.76082120496614],[55.089734262348586,51.75892848548792],[55.09180778542035,51.75573945768243],[55.09258311932891,51.7551471138353],[55.0928273758526,51.754747862318226],[55.09285294458994,51.749187709651245],[55.093221836081185,51.74722326503862],[55.0948372407858,51.73964598355074],[55.08513452839382,51.73607282753211],[55.07622574987031,51.729954466646895],[55.07302611328147,51.7283715910524],[55.070477403856565,51.727482829963215],[55.06797160977592,51.726807259854525],[55.06326042902431,51.72622898492036],[55.06369488932572,51.7249061148094],[55.07095023593159,51.72509753783418],[55.0719184846065,51.72201065627716],[55.072191426909335,51.71767002244652],[55.074138067637485,51.715488296271445],[55.07660249827204,51.71471474736369],[55.07910071624436,51.716807130779976],[55.08672275384988,51.715107602200945],[55.08989004248906,51.714857624764555],[55.09002740564923,51.71377544543804],[55.09059392225176,51.7124533051285],[55.09105315049377,51.71139772811709],[55.09104673022146,51.710496682500256],[55.09073990253947,51.70996887413844],[55.09237318670408,51.7093766756361],[55.095179089969065,51.71078566493158],[55.102469646707014,51.709528564778005],[55.10065709868387,51.707707484829136],[55.10499186108734,51.70725684923112],[55.11209466319427,51.70697951734966],[55.111912585616714,51.704349119775166],[55.118918828199064,51.70391844897652],[55.11971798520094,51.71256391804961],[55.13281010662247,51.71171900599668],[55.139729252279615,51.71954045424803],[55.12119680563967,51.72100048186221],[55.092583339391844,51.72435571639559],[55.09401335380607,51.72869857240093],[55.09472836101316,51.733514964041085],[55.10105109746583,51.732911912451236],[55.10288209002077,51.73630092007102],[55.1061292889356,51.736452386167386],[55.103260864898864,51.73096946665459],[55.102151969975964,51.72787115030756],[55.10306550907843,51.7275732799439],[55.104889847588005,51.72657683019524],[55.10716523359153,51.7258365061863],[55.10832569340372,51.72582168290111],[55.1088441685701,51.726298413993504],[55.10941251431228,51.728950768003315],[55.110105965276226,51.73156130397699],[55.109340294536075,51.73395851477003],[55.10657467390979,51.7353931686868],[55.10819946417011,51.74857584589139],[55.09884409207598,51.750248032517504],[55.093522935289954,51.74765219254053],[55.093266135023725,51.75220987775974],[55.09839590225855,51.75210874737266],[55.10867689440026,51.754237086773465],[55.12360542877171,51.76015708608734],[55.12287586791966,51.762607093170594]]]},"properties":{"fill":"#1e98ff","fill-opacity":0.6,"stroke":"#177bc9","stroke-width":"5","stroke-opacity":0.9}}]}
```