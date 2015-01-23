# The **CGS** project
The **CGS** project stands for Centralized genomics system. The goal of this project is to offer a big data infrastructure for genomics data, and in particular for variant information.

This project contains different modules that are related to each other but still can be used independently (up to some extent). Here are the modules available as github repositories:

- **cgs-vcf-hbase**: this modules defines a VCF table in HBase, how to build it, how to build a corresponding table in the metastore that will be accessible by tools like Hive, Impala, etc, allowing you to make SQL-like requests on your database. This also allows you to parametrize security on HBase (on column families, or even on HBASE cells).   
- **cgs-api**: this modules implements different APIs that allows you to access resources (or data) similar to the one you would access with Google Genomics. Graphical apps are also developed as plugins for [Hue](http://gethue.com/) and allows you for instance to import new VCF files into your database or to access data without having to know how to use the APIs.   
- **cgs-analysis**: this modules implements analysis tools that can be performed on data available in this project, for instance machine learning techniques distributed in the hadoop framework.  
- **cgs-benchmarks**: this modules presents different benchmark studies that have been performed using this system (CGS).

This project has been initiated within the BridgeIris project funded by [Innoviris](http://www.innoviris.be). 
