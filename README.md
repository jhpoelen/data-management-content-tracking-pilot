# data-management-content-tracking-pilot


How this Preston archive was produced:

```
$ history
2036  preston track https://riojournal.com/article/60614/download/xml/
 2037  preston ls
 2038  preston history
 2039  preston ls | preston grep -o --no-line
 2040  preston ls | preston grep -o --no-line -l tsv | head
 2041  preston ls | preston grep -o --no-line -l tsv | grep "http://www.w3.org/ns/prov#value"
 2042  preston ls | preston grep -o --no-line -l tsv | grep "http://www.w3.org/ns/prov#value" | cut -f3
 2043  preston ls | preston grep -o --no-line -l tsv | grep "http://www.w3.org/ns/prov#value" | cut -f3 | xargs preston track
 2044  preston cat hash://sha256/dc80b6ea5bfac887b10fa6b462a3e376047412ee3e23b48c9c9b43297e50f484
 2045  preston cat hash://sha256/dc80b6ea5bfac887b10fa6b462a3e376047412ee3e23b48c9c9b43297e50f484 > figure.png
 2046  xdg-open figure.png
 2047  preston history
 2048  preston ls | preston grep -o --no-line | preston process
 2049  preston cat 'cut:hash://sha256/0cb5182627fd01ad1df2774dc93c3657829970eeac0e96e3fc60d075639a7898!/b117212-117331'
 2050  preston cat 'hash://sha256/0cb5182627fd01ad1df2774dc93c3657829970eeac0e96e3fc60d075639a7898' | less
 2051  ls
```
