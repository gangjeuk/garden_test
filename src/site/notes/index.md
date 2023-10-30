```dataview
LIST WITHOUT ID "[" + embed(cover) + "](<" + file.folder + "/" + file.name + ">)" + "<div class=content-name>"  + file.name + "</div>" + "<div class=content-tags>" + filter(file.etags), (x) => regexmatch(x, "TODO") + "</div>"
FROM "CTF"
WHERE dg-publish = true
SORT file.ctime ASC
LIMIT 5
```