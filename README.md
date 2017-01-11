# EPFImporter

As described by Apple:

> The EPFImporter is a command-line based tool, available to EPF partners, that
> allows for ingestion of the EPF-Relational files into a relational database.
> The tool is written in Python and the source code is available for modification
> by partners to fit their specific needs and platform.

More information, and the original version, can be found here:
https://www.apple.com/itunes/affiliates/resources/documentation/epfimporter.html

This version has been modified to run cleanly with MySQL 5.6 and the EPF data
as provided by Apple in 2014.

## Install

```python
pip install -r requirements.txt
```

## Known Issue

+ use utf8mb4 will cause row size issue on a few columns, by updating the row size will fix it
