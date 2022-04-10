```bash
$ file unk 
unk: Zip archive data, made by v4.5, extract using at least v2.0, last modified Mon Jan 26 00:44:48 1970, uncompressed size 1364, method=deflate
```
```bash
$ unzip unk                                                          
Archive:  unk
file #1:  bad zipfile offset (local header sig):  0
  inflating: _rels/.rels             
  inflating: word/_rels/document.xml.rels  
  inflating: word/document.xml       
  inflating: word/theme/theme1.xml   
 extracting: docProps/thumbnail.jpeg  
  inflating: word/settings.xml       
  inflating: word/fontTable.xml      
  inflating: word/webSettings.xml    
  inflating: docProps/core.xml       
  inflating: word/styles.xml         
  inflating: docProps/app.xml        
```
```bash
$ ls                                                                   
docProps  _rels  unk  word
```
#### I found a flag in docProps / thumbnail.jpeg
![](https://raw.githubusercontent.com/Rajchowdhury420/temp-files-for-writeup/main/flaaaggg.png)
