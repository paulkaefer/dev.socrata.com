---
layout: with-sidebar
sidebar: documentation
title: to_multiline
---

##### Function: `to_multiline`
```
  convert a line into a multiline


  parse a WKT (text) representation of a multiline into a multiline value

Examples:

  to_multiline(to_line('LINESTRING (30 10, 10 30, 40 40)'))
  -- Result: {"type":"MultiLineString","coordinates":[[[30,10],[10,30],[40,40]]]}


  to_multiline('MULTILINESTRING ((10 10, 20 20, 10 40),(40 40, 30 30, 40 20, 30 10))')
  -- Result: {"type":"MultiLineString","coordinates":[[[10,10],[20,20],[10,40]],[[40,40],[30,30],[40,20],[30,10]]]}

  to_multiline(a_wkt_multiline)
  -- Result: {"type":"MultiLineString","coordinates":[[[10,10],[20,20],[10,40]],[[40,40],[30,30],[40,20],[30,10]]]}




```

###### Signatures
    line -> multiline
    text -> multiline
    multiline -> multiline

