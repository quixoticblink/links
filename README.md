DBpedia-Links
=============
A repo that contains links and alternative classifications for DBpedia.

# About

Links are the key enabler for retrieval of related information on the Web of Data and DBpedia is one of the central interlinking hubs in the Linked Open Data (LOD) cloud. The DBpedia-Links repository maintains linksets between DBpedia and other LOD datasets. System for maintenance, update and quality assurance of the linksets are in place and can be explored further.

In this README, we will include descriptions on how to download and use the links, run all available tools as well as pointers to the most important documentation. if questions remain please use the [GitHub Issue tracker](http://github.com/dbpedia/dbpedia-links/issues). If you want to give us more feedback, feel free to use the [DBpedia Discussion mailinglist](http://lists.sourceforge.net/lists/listinfo/dbpedia-discussion).

## Why upload your links?
All links you are contributing will be loaded (after a quality check) into the main DBpedia datasets and therefore will link to your data. Users of DBpedia can then better find your data. Also we will be able to tell you, which other external databases link to your data. 

# Repository license
All data in the repository is provided as CC-0. All software is provided under Apache 2.0 License.

# How to contribute links to DBpedia?
If you're interested in contributing links and to learn more about the project, please visit the [how to wiki page](https://github.com/dbpedia/links/wiki/How-To-Contribute-Links-to-DBpedia) for more detailed informations. 

You can read more in our [paper](http://ceur-ws.org/Vol-1695/paper21.pdf):

# How to download the monthly link release
If you want to download the current, or older, releases of the given links, please go [here](http://downloads.dbpedia.org/links/) and click at the corresponding month.

The publishing process is automated via a cronjob which will run all given scripts, LIMES/SILK configurations, patches, etc. to generate the linksets. It is executed currently monthly on our own server

Please check out the [how to](https://github.com/dbpedia/links/wiki/How-To-Contribute-Links-to-DBpedia#automated-process) for more informations regarding the automated process, how to set it up, run it and customize it.

# How to update links for one dataset
If you want to update links for one dataset, either create a new pullrequest to update the old linkset or follow the [how to](https://github.com/dbpedia/links/wiki/How-To-Contribute-Links-to-DBpedia) to learn more about how to create a patch for the dataset which will be applied automatically on the next release.

To make sure that your dataset is following proper conventions as mentioned in the [how to](https://github.com/dbpedia/links/wiki/How-To-Contribute-Links-to-DBpedia), you can run the `validate.sh` script in `tools/backend/bin/`.

For more information regarding the validating, generating and patching aspects check out the README from the [backend](https://github.com/dbpedia/links/tree/master/tools/backend)

# Overview of current linksets

## dbpedia.org
* [dati.camera.it](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/dati.camera.it)
* [eunis.eea.europa.eu](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/eunis.eea.europa.eu)
* [gadm.geovocab.org](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/gadm.geovocab.org)
* [learning-provider.data.ac.uk](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/learning-provider.data.ac.uk)
* [lobid.org](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/lobid.org)
* [rdfdata.eionet.europa.eu](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/rdfdata.eionet.europa.eu)
* [transparency.270a.info](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/transparency.270a.info)
* [viaf.org](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/viaf.org)
* [worldbank.270a.info](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/worldbank.270a.info)
* [www.bbc.co.uk:things](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/www.bbc.co.uk:things)
* [www.geonames.org](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/www.geonames.org)
* [www4.wiwiss.fu-berlin.de](https://github.com/dbpedia/links/tree/master/links/dbpedia.org/www4.wiwiss.fu-berlin.de)

## xxx.dbpedia.org
* de
    * [lobid.org-manifestation](https://github.com/dbpedia/links/tree/master/links/xxx.dbpedia.org/de/lobid.org-manifestation)
    * [lobid.org-organization](https://github.com/dbpedia/links/tree/master/links/xxx.dbpedia.org/de/lobid.org-organization)
    * [vocabulary.wolterskluwer.de-arbeitsrecht](https://github.com/dbpedia/links/tree/master/links/xxx.dbpedia.org/de/vocabulary.wolterskluwer.de-arbeitsrecht)
    * [vocabulary.wolterskluwer.de-courts](https://github.com/dbpedia/links/tree/master/links/xxx.dbpedia.org/de/vocabulary.wolterskluwer.de-courts)
* it
    * [dati.camera.it](https://github.com/dbpedia/links/tree/master/links/xxx.dbpedia.org/it/dati.camera.it)
* ja
    * [geonames.jp](https://github.com/dbpedia/links/tree/master/links/xxx.dbpedia.org/ja/geonames.jp)
* nl
    * [test.rce.rnatoolset.net](https://github.com/dbpedia/links/tree/master/links/xxx.dbpedia.org/nl/test.rce.rnatoolset.net)

# description of further tools in the repo and how to access/execute them
All tools are being kept in the `tools` folder and have their own respective Readme to explain what their use is and how to use them. Currently there the following tools available: 
* [Backend](https://github.com/dbpedia/links/blob/master/tools/backend/)
* [Frontend](https://github.com/dbpedia/links/tree/master/tools/frontend)

# Contributors (alphabetically)

- Sarven Capadisli, AKSW, Uni Leipzig (Csarven)
- Pascal Christoph, (dr0i)
- Christopher Gutteridge (cgutteridge)
- Amy Guy, BBC / Uni Edinburgh (rhiaro)
- Sebastian Hellmann, AKSW, Uni Leipzig (kurzum)
- Anja Jentzsch, HPI Potsdam (ajeve)
- Barry Norton (BarryNorton)
- Heiko Paulheim, Uni Mannheim (HeikoPaulheim)
- Petar Ristoski, Uni Mannheim (petarR)
- Robert Rößling, AKSW, Uni Leipzig (rpod)
- Søren Roug, (sorenroug)
