

# RSVP
check RSVP status in a nother form
```
=IF(ISERROR(VLOOKUP(INDIRECT(ADDRESS(ROW(),COLUMN()+4)), RSVP!B2:C133, 1, FALSE)), "", VLOOKUP(INDIRECT(ADDRESS(ROW(),COLUMN()+4)), RSVP!B2:C133, 2, FALSE))
```

### selected
```
=query(screening!A:L,"select D,E,F, H, I, J, K, L where A='yes' ")
```

### waitinglist
```
=query(screening!A:L,"select D,E,F, H, I, J, K, L where A!='yes' ")
```

### screening
colored marking participants by selected skills (total beginner vs. angular/programmer)
* right click column > conditional formatting
