

CLI::LaTeX::Table - provides a quick command tool that transforms almost any table to LaTeX snippet.

It rovides a quick tool to transform into suitable LaTeX snippets
from (almost) any tables from Excel, SQL outputs used as a LaTeX table. Note that
it also has functions to transform lengthy SQL sentences into suitable LaTeX snippets
usable inside the footnote and the caption of a table. 

Given the TSV formatted table
such as copied region of an Excel worksheet or SQL output, you can
easily get the LaTeX commands to produce same table even if it contains
any alphabetical, numeral, symbolic characters unless they are ASCII or
UTF-8. You can save a lot of time to draw tables by utilizing many
option swithes for magnifying, rotating partly or totally, treating well
on large numbers, hankaku-kana and so on.

PROVIDED COMMAND LINE INTERFACE programs : 
  
  1. latextable -- snippet generator from worksheet/scripts into LaTeX table/table-caption/text.
  2. transpose -- flips a matrix over its diagonal. Input is copied from Excel/SQL output and so on.
  3. saikoro -- random number/matrix generators of (various) uniform distributions.
  4. csel -- an command line interface to handle TSV/CSV files easier than cut/AWK commands.
  5. csv2tsv -- TSV formatter for regular CSV format files by Text::CSV_XS module.

  All programs provides help-manual that is availble such as by "latextable --help". 
  If you want to see only "switch options", do "latextable --help opt(ions)". 
  If you want to see Japanese or English manual as you wish, do "latextable --help en" or "--help ja".

 Please try : 

```bash
saikoro  
saikoro -g 12x5 
saikoro -g 12x5 -s123 
saikoro -g 12x5 -s123 | csel -d 3 
saikoro -g 12x5 -s123 | transpose
saikoro -g 12x5 -s123 | latextable 
saikoro -g 12x5 -s123 | latextable -Cmn
latextable    # After opening some Excel or SQL ouput files, and copy and paste it.
```
