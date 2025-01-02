---
title: "Json hi iem ani?"
date: "2024-12-31"
excerpt: "JSON hi data storage format chi khat ana , data format lai chun ama hi hmang rawn tak ana, 
a hming lam tluon chun **Javascript Object Notation** anih. Kum 2000 lai kha software engineer **Douglas Crockford** siem suok ana. Hi data format hi tulai a ding chun data exchange trulna reng reng anchun an hmang tak anih."
categories: 
  - "hmar"
  - "technology"
tags: 
  - "informational"
---
### Thuhmahruoi
JSON hi data storage format chi khat ana , data format lai chun ama hi hmang rawn tak ana, 
a hming lam tluon chun **Javascript Object Notation** anih. Kum 2000 lai kha software engineer **Douglas Crockford** siem suok ana. Hi data format hi tulai a ding chun data exchange trulna reng reng anchun an hmang tak anih. 

JSON hi hrietthiem a awlsam hle lei hin an lar em-ema, a hrie naw ramsam khawm an um naw a, anachu a hrie naw hai ta ding chun hi ka hung hril ve na nisien.

Chu el khelah lekhaziek nei — dictionary siem le linguistic data siem tam tak ei uma , computer le programming hriet naw khawma JSON annaw le CSV bekin hi data hi mani a siem chun data indik lem suok ata chun I dit dan takkin data I siem thei ding ana , hi lei hin JSON hi iem ani hang hriet chieng khawm hi apoi bekin ka hriet naw anih.


JSON hin a hnuoia structure hi aneia.

**Tekhina:1**

---

```Json

{
  "name": "Eunicky Lungtau",
  "age": 33,
  "active": true
}

```

---

Hi structure hi , "key  le value " pair an na, `name` hi key ana a value chu `Eunicky Lungtau` ti hi anih.

Database ahai apps a dingin backend ah data le Machine Learning a ding dataset ahai khom   an hmang tak anih.

---

### Basics anthawk hang hril lang.

Iengkim digital hi binary data a sie thrat hlak ana , hi binary data hi 1 le 0 ana ,  thla ei lak le hla ei ngai hai khawm hi binary data a sie thrat hlak an na , a lim ei hmu le ri ei hriet thei hai hi software hmanga hi binary data hi inlet sawng ani hlak anih.

Pdf , Jpg , Mp3, Mp4 le Json khawm hi data format an na ei hmang dan a dang senga chu an sin thaw hi angkhat vawng ana, thla ei lak le hla ei ngai hai hi binary data hmangin software in digital logic anthawk electricity a manipulate a ei hmu a ei ngai thei hlak anih.

---

### JSON Sunzawmna 

Json structure hi a flexible hle ,  google sheets le excel ahai first row hi header a ei hmang a data ei siem hin row le column chou a um theia , Json a ruok hinchu ei nuom dan takkin hi structure hi ei siem thei anih.

**Tekhina:2**

---

```Json

{
  "name": "Eunicky Lungtau",
  "age": 33,
  "active": true,
  "address": {
    "street": "Muolhoi,Vengsak",
    "city": "Haflong",
    "state": "Assam",
    "country": "India"
  },
  "contact": {
    "email": "eunickylungtau@gmail.com",
    "phone": "+91 123 456 7890"
  },
  "hobbies": ["reading", "traveling", "music"],
  "work": {
    "occupation": "Teacher",
    "yearsExperience": 10,
    "isRemote": false
  }
}

```

---

Tekhina in a chunga structure ahin `name` hi key ana, Eunicky Lungtau hi value anih ka hung ti a khan , value ahin key le value a um sa theia.

**note:** hi structure hi , hiva data pakhat a ding cho hin a valid asanchu coherence anei nawh.
Tekhina ding a ka hung suklang ana , data hi midang data belsa inla query thaw ding chun `contact` hi tu contact am ani ti information a um naw leiin.
Andik lai zingin data dang belsa ding chun an dik nawh.

---

Achunga data popo hi andik naw na chu  object pakhat an na , hieng popo data hi mi tamtak ta dingin i siem nuom chun a hnuoia structure ang hin ,  `people` mani data izir le ei hmang nuom dan izir in hming sie eita , curly brackets in ei tran a ,  `people` ti hi key a hung ni ta a square brackets [square] in ei khar khum nawka , curly brackets {curly} in a khum let nawk a.

Curly {curly} in a khar khum po hi object an na , object sunga um hai hi key value pair an na , hi curly brackets {curly} pahnina hi `"isRemote":false` zoa curly brackets {curly} pahni na hin a khar khuma , hi hnung chi a comma (,) hin `name` anthawk `isRemote` chen hin object pakhat an ni tir anih.

**Tekhina:3**

---

```Json

{
  "people": [
    {
      "name": "Eunicky Lungtau",
      "age": 33,
      "active": true,
      "address": {
        "street": "Muolhoi,Vengsak",
        "city": "Haflong",
        "state": "Assam",
        "country": "India"
      },
      "contact": {
        "email": "eunickylungtau@gmail.com",
        "phone": "+91 123 456 7890"
      },
      "hobbies": ["reading", "traveling", "music"],
      "work": {
        "occupation": "Teacher",
        "yearsExperience": 10,
        "isRemote": false
      }
    },
    {
      "name": "Aaron Pulamte",
      "age": 33,
      "active": true,
      "address": {
        "street": "Muolhoi, Vengsak",
        "city": "Haflong",
        "state": "Assam",
        "country": "India"
      },
      "contact": {
        "email": "a3@gmail.com",
        "phone": "+91 987 654 3210"
      },
      "hobbies": ["sports", "music"],
      "work": {
        "occupation": "Stay at home dad",
        "yearsExperience": 6,
        "isRemote": true
      }
    }
  ]
}

```

---

Achunga ang hin mi tamtak data ei siem thei anih .

Ahnuoia hi hrietthiem a awlsam deua anachu ama hi flat structure anih.

**Tekhina:4**

Square brackets in ei tran a , square brackets bawkin ei tawp a , data kar thre na ding ahin comma (,) ei hmang anih.

---

```Json

[
  {
    "name": "Eunicky Lungtau",
    "age": 33,
    "active": true
  },
  {
    "name": "Niengkim Hengna",
    "age": 31,
    "active": true
  },
  {
    "name": "Aaron Pulamte",
    "age": 33,
    "active": true
  }
]

```

---

JSON hi flexible hle sienkhawm dataset ahai hin dan naran chun structure mumal deu a trul hlaka , amruokchu dataset hi local server ah i host ding apoi bek chuong naw anih asanchu query dan ding nangin i siem ding ani leiin.

JSON hi a flexible el khelah , a lightweight hle a a hrietthiem khawm a awlsam hle a , tekhina dang hung bel sa lang.

Bible data siem na ding khawma hmang thei ana.

**Tekhina:5**

---


```Json

{
  "book": "Johan",
  "chapter": 3,
  "verse": 16,
  "text": "Pathienin khawvêl a hmangai bêk bêk a, chuongchun, a Naupa khât nei sun chu a pêk a, ama chu tûkhawm a ring taphawt chu an bohmang nawh a, chatuona hringna an nei lemna dingin."
}

```

**Tekhina:6**

```Json

{
  "reference": {
    "book": "Johan",
    "chapter": 3,
    "verse": 16
  },
  "text": "Pathienin khawvêl a hmangai bêk bêk a, chuongchun, a Naupa khât nei sun chu a pêk a, ama chu tûkhawm a ring taphawt chu an bohmang nawh a, chatuona hringna an nei lemna dingin.",
  "translation": "HMARCLBSI"
}

```

Hieng tilo khawma parallel translation data siem ding khawma a structure hi ei nuom dan taka siem   thei ana.

**Tekhina:7**

```Json

{
  "reference": {
    "book": "John",
    "chapter": 3,
    "verse": 16
  },
  "translations": [
    {
      "translation": "CLBSI",
      "text": "Pathienin khawvêl a hmangai bêk bêk a, chuongchun, a Naupa khât nei sun chu a pêk a, ama chu tûkhawm a ring taphawt chu an bohmang nawh a, chatuona hringna an nei lemna dingin."
    },
    {
      "translation": "KJV",
      "text": "For God so loved the world, that he gave his only begotten Son, that whosoever believeth in him should not perish, but have everlasting life."
    },
    {
      "translation": "NIV",
      "text": "God so loved the world that he gave his one and only Son. Anyone who believes in him will not die but will have eternal life."
    }
  ]
}

```

---


**Tekhina:8**

Hi anhnuoia structure hi a chunga mi lehin an ang naw achu purpose — parallel translation data structure an suk puitling veve anih.

---

```Json

{
  "John_3_16": {
    "CLBSI": {
      "text": "Pathienin khawvêl a hmangai bêk bêk a, chuongchun, a Naupa khât nei sun chu a pêk a, ama chu tûkhawm a ring taphawt chu an bohmang nawh a, chatuona hringna an nei lemna dingin.",
      "language": "Hmar"
    },
    "KJV": {
      "text": "For God so loved the world, that he gave his only begotten Son, that whosoever believeth in him should not perish, but have everlasting life.",
      "language": "English"
    },
    "NIV": {
      "text": "God so loved the world that he gave his one and only Son. Anyone who believes in him will not die but will have eternal life.",
      "language": "English"
    }
  }
}

```

---
### CSV hang hril met inla

JSON tilo chun CSV (comma seperated values) format a um ve a , JSON nek hin a simple lema ananchu a simple ang tak hin dataset a data tamtak a um ding hin structure maintain aharsa ta hlak anih.

Achunga hming ka hung hmang hai CSV format tekhina dingin hang hmang nawk vat lang ,  ahnuoia ang hin a um ding anih.

**Tekhina:9**

---

```CSV

Name,Age,Active
Eunicky,33,True

```

---


**Tekhina:10**

***A ziek dan dang chu double inverted commas (") hmangin.***

---

```CSV

Name,Age,Active
"Eunicky Lungtau","33","True"

```

---

double inverted comma hmanga CSV file siem hi a tangkaina chu , column pakhat sungah value dang khawm i sie sa thei anih.

Tekhina in translation data lo siem nila.

**Tekhina:11**

---


```CSV

hmar-phrase,english-translation
"iem I hming,iem ani I hming","what is your name"
"tum ini,tu'm ini","who are you"

```

---


Hi achunga data tekhina ahin `what is your name` le `who are you` hin parallel translation pahni ve ve in an nei anih .

---

### TXT , PDF , JSON le CSV

Txt format le hieng CSV le Json hai hi an thau na chu txt format a data siem ding hin dan le dun tak-tak anei thei naw a , row hmasatak hi header lo in ni tir inla khawm row tin hin value pakhat cho anei thei anih.

Chun chuonga row pakhat a value tamtak ei sie a custom rules ei siem ding anichun hieng CSV le Json hai hi Industry standard an na , anni hai hmang hi alo tangkai nawk lem antah.

Hi lei hin TXT hi data sie thrat na ding chun a tha bek naw a hmang thei ani lai zingin Csv mani JSON hmang hi a tangkai lem anih.

Pdf a data sie that khawm hi thil thei ani lai zingin data loss a um theia chun ama hi thlakak ang ani lei hin file size hai hi a rik hlak a , tekhina in Bible pumpui CSV format chun dan naran in 5 Mb lai vel ani hlak lai , PDf a chun compression tam hle sien khawm 100 Mb chu a tlawm tieng ana. 

Platform dang dang ah pdf file i upload a download a upload nawk a cycle hi vel tam an lawn hnung chun compression leiin tiem thei khurin a suok ta naw ding anih.
CSV , Txt le Json hai hi pdf nekin a tiem loin tak met sien khawm software annawle script indik naw leiin file a overwrite tinaw chun data loss a um thei naw anih.

Chun Pdf hichu human readable data format ana ana hi thlalak mani annaw le visual data tienga (equations, formulas, image) ahai hmang ani dan naran hlak anih.

---

### Atawpna Dingin 

JSON hi a flexible em em a , computer le programming inhnik hai chun hi thil hi hriet chieng a tha a , 
data mani dictionary siem hai khawma hieng JSON structure tak tak eilo hrietthiem naw a structure eilo siem theinaw anikhawma CSV structure bek a data siem hi a tha a andik dan tak lem anih.

Hi thil thu hi hrietthiem a harsa naw a , anachu eini trawng a inchuk na ding le tiem na ding ala um ngai naw leiin basic information khawm nisien, ka thei tawp in ka hung ziek ve anih.

Hi po hin JSON hi hrilfie lem chu a hrilfie zo nawh amruokchu hipo hi lo ni phawt sien a trul dan izir in post dang ahai hung sunzawm nawk katih.

