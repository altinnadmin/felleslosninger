---
title: Avsender  
permalink: sikkerdigitalpost_avsender.html
sidebar:
---  

  - Identifikator  
    http://begrep.difi.no/SikkerDigitalPost/1.3.0.RC1/1.3.0.RC1/begrep/Avsender
  - Term  
    Avsender
  - Definisjon  
    Juridisk organisasjon/entitet som er Behandlingsansvarlig for
    innholdet i den digitale posten,
  - Datatype  
    complexType
  - Kilde  
    DIFI
  - Kommentar  
    Avsender er den som er ansvarlig for innholdet i forsendelsen.  
    Kan være forskjellige frå Databehandler (for eksempel kan SvarUT
    være databehandler på vegne av en kommune)

#### Egenskaper

| --- | --- | --- |
| Identifikator | Kardinalitet | Datatype |                                                        
| ../felles/virksomhetsidentifikator | 1..1 | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |
| HER SKAL DET VÆRE LINK TIL /felles/avsenderifentifikator | 0..1 | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) |           
| fakturaReferanse | 0..1 | [xs:string](http://www.w3.org/TR/xmlschema-2/#string) \[maks 40\] |

#### Xml eksempel

``` brush: xml; toolbar: false
    <avsender>
        <organisasjon authority="iso6523-actorid-upis">9908:123456789</organisasjon>
        <avsenderidentifikator>12345</avsenderidentifikator>
        <fakturaReferanse>123</fakturaReferanse>        
    </avsender>
```