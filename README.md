GDAL(Geospatial Data Abstraction Library) document Japanese translation project 
===============================================================================

Here is a repository for JA translation team to translate GDAL document in Japanese.
We use OmegaT(https://omegat.org/) for computer aided translation.


Tools required
--------------

* OmegaT version 4.0 or later  (https://omegat.org)

* Okapi filter plugin (https://bintray.com/okapi/Distribution/OmegaT_Plugin)


Preparation
------------

* Install OmegaT in your computer platform

* Install Okapi pkugin for OmegaT

  - Extract okapi plugin distribution

  - Copy jar file into <HOME DIR>/.omegat/plugins/

* Configure Okapi pkugin

  - Launch OmegaT

  - Open " 設定″ー”ファイルフィルター”

  - Select "Doxygen filter (Okapi)" and push "Edit" button

  - Add '*.dox' file as a target.


Team translation
-----------------

* Download team translation project from Github.

  - Open "Project" - "Download team project"

  - Enter URL: https://github.com/miurahr/gdal_docs_ja.git

* Start translation.

Generate localization sources
-----------------------------

* install doc tools

```
$ cd gdal/doc
$ pip install -r requirements.txt
$ pip install sphinx-intl
```

* generate gettext files

```
$ make gettext
```

* generate message catalog

```
$ sphinx-intl update -l ja
```

Generate translated documents
-----------------------------

```
$ make -e SPHINXOPTS="-D language='ja'" html
```

