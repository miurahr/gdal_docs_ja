GDAL(Geospatial Data Abstraction Library) document Japanese translation project 
===============================================================================

Here is a repository for JA translation team to translate GDAL document in Japanese.
We use OmegaT(https://omegat.org/) for computer aided translation.

このリポジトリでは、フォークやPull-Requestのワークフローに対応しません。
かならず、直接の書き込み権限


Tools required
--------------

* OmegaT version 4.0 or later  [ダウンロード](https://omegat.org/ja/download)



Team translation
-----------------

1. Download team translation project from Github.

  1. Launch OmegaT

  2. Open "Project" - "Download team project"

  3. Enter URL: https://github.com/miurahr/gdal_docs_ja.git

2. Start translation.

3. Generate target document.

  * Open "Porject" > "Generate target document"
  
  * You will see PO files on target folder.


Generate translated documents
-----------------------------

```
$ make -e SPHINXOPTS="-D language='ja'" html
```

GDALへのパッチ提案と採択がまだですので、ドキュメントの生成は、少々おまちください。
