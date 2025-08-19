
```dataview
TABLE l.link AS Segment, l.location AS Location, l.subject AS Subject, l.type AS Type, l.text AS Story
FROM "Daily News"
FLATTEN file.lists as l
WHERE l.annotated
AND contains(l.subject, "Israel-Palestine")
SORT file.ctime desc
```

```dataview
TABLE l.link AS Segment, l.location AS Location, l.subject AS Subject, l.type AS Type, l.text AS Story
FROM "Daily News"
FLATTEN file.lists as l
WHERE l.annotated
AND contains(l.subject, "Ukraine War")
SORT file.ctime desc

```