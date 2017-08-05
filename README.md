# worms.py

Python library to access the web services of the [WoRMS
database](http://www.marinespecies.org/).

Code based on [itis.py](https://github.com/nelas/itis.py) and the [python
client](http://marinespecies.org/aphia.php?p=webservice&type=python) from
WoRMS.

## Requirements

- [SUDS](https://pypi.python.org/pypi/suds/0.4) (Lightweight SOAP client)

## Basic usage

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
