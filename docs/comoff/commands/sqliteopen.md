---
title: "SQLiteOpen"
description: "Opens an SQLite database file in read and write mode. If the database does not exist, DIAdem creates a new database property. Since only one database can be ope"
---

# SQLiteOpen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SQLiteOpen

Opens an SQLite database file in read and write mode. If the database does not exist, DIAdem creates a new database property. Since only one database can be open at a time, DIAdem first closes an already open database before opening the new database.

## Signature

```python
dd.SQLiteOpen( SQLiteDatabase )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SQLiteDatabase</td>
<td>Specifies the name of the SQLite database.<div id="exp_SQLiteDatabase">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.SQLiteOpen(dd.DataReadPath + "Cities_1000_V4.4.sqlite")
dd.SQLiteAddExtension("mod_spatialite4.dll", "sqlite3_modspatialite_init")
SQLQuery("SELECT Name FROM cities1000 LIMIT 10;", True)
SQLQuery("SELECT Name FROM cities1000 ORDER BY Distance(geom_wsg84, MakePoint(cast(12.4876180 AS DOUBLE), cast(41.9029000 AS DOUBLE), 4326)) LIMIT 5;", True)
SQLQuery("SELECT * FROM knn WHERE f_table_name = 'cities1000' and ref_geometry = MakePoint(cast(12.4876180 AS DOUBLE), cast(41.9029000 AS DOUBLE)) LIMIT 5;", True)
SQLQuery("SELECT Name FROM cities1000 LIMIT 10;", False)
SQLQuery("SELECT Name FROM cities1000 ORDER BY Distance(geom_wsg84, MakePoint(cast(12.4876180 AS DOUBLE), cast(41.9029000 AS DOUBLE), 4326)) LIMIT 5;", False)
SQLQuery("SELECT * FROM knn WHERE f_table_name = 'cities1000' and ref_geometry = MakePoint(cast(12.4876180 AS DOUBLE), cast(41.9029000 AS DOUBLE)) LIMIT 5;", False)
dd.SQLiteClose()

def SQLQuery(sQuery, bOutputHeader):
    dd.LogFileWrite("sQuery: " + sQuery)
    dd.LogFileWrite("-----------------------------")
    Result = dd.SQLiteQuery(sQuery, bOutputHeader)
    if isinstance(aResult, tuple) :
        for iRow in range( 0, len(aResult,1)-1):
            sText = ""
            for iColumn in range( 0, len(aResult,2)-1):
                sText = sText + Left(aResult(iRow, iColumn) + Space(25), 20)
            dd.LogFileWrite(sText)
    dd.LogfileWrite(" ")
    dd.LogfileWrite(" ")
```

---

*Source: `ComOff/SQLiteOpen.htm`*
