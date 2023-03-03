# :squid: `worms.py`

Python library to query the [World Register of Marine Species](http://www.marinespecies.org/) (WoRMS).

## Requirements

- [suds](https://pypi.org/project/suds/) (Lightweight SOAP client)

## Basic usage

```
>>> from worms import Aphia
>>> aphia = Aphia()
>>> results = aphia.get_aphia_records('Priapulus caudatus')
>>> print(results[0])
>>>
(AphiaRecord){
   AphiaID = 101160
   url = "https://www.marinespecies.org/aphia.php?p=taxdetails&id=101160"
   scientificname = "Priapulus caudatus"
   authority = "Lamarck, 1816"
   taxonRankID = 220
   rank = "Species"
   status = "accepted"
   unacceptreason = None
   valid_AphiaID = 101160
   valid_name = "Priapulus caudatus"
   valid_authority = "Lamarck, 1816"
   parentNameUsageID = 101095
   kingdom = "Animalia"
   phylum = "Priapulida"
   cls = None
   order = "Priapulomorpha"
   family = "Priapulidae"
   genus = "Priapulus"
   citation = "Paulay, G. (2023). World List of Priapulida. Priapulus caudatus Lamarck, 1816. Accessed through: World Register of Marine Species at: https://www.marinespecies.org/aphia.php?p=taxdetails&id=101160 on 2023-03-03"
   lsid = "urn:lsid:marinespecies.org:taxname:101160"
   isMarine = 1
   isBrackish = None
   isFreshwater = None
   isTerrestrial = None
   isExtinct = None
   match_type = "like"
   modified = "2008-01-04T16:28:44.880Z"
 }
```
