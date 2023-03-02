# :squid: `worms.py`

Python library to query the [World Register of Marine Species](http://www.marinespecies.org/) (WoRMS).

## Requirements

- [suds](https://pypi.org/project/suds/) (Lightweight SOAP client)

## Basic usage

```
>>> from worms import Aphia
>>> aphia = Aphia()
>>> results = aphia.get_aphia_records('Priapulus caudatus')
>>> print(results)
>>>
    [(AphiaRecord){
       AphiaID = 101160
       url = "http://www.marinespecies.org/aphia.php?p=taxdetails&id=101160"
       scientificname = "Priapulus caudatus"
       authority = "Lamarck, 1816"
       rank = "Species"
       status = "accepted"
       unacceptreason = None
       valid_AphiaID = 101160
       valid_name = "Priapulus caudatus"
       valid_authority = "Lamarck, 1816"
       kingdom = "Animalia"
       phylum = "Cephalorhyncha"
       cls = "Priapulida"
       order = None
       family = "Priapulidae"
       genus = "Priapulus"
       citation = "van der Land, J.; Neuhaus, B. (2008). Priapulus caudatus Lamarck, 1816. Accessed through:  World Register of Marine Species at http://www.marinespecies.org/aphia.php?p=taxdetails&id=101160 on 2017-08-06"
       lsid = "urn:lsid:marinespecies.org:taxname:101160"
       isMarine = 1
       isBrackish = None
       isFreshwater = None
       isTerrestrial = None
       isExtinct = None
       match_type = "like"
       modified = "2008-01-04T17:28:45Z"
     }]
```
