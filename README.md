TODO:
-----------
    - AJAX sa caute in avl pe srv local - Get()
    - JS - adaugat rows in result din json

    - startup - apelat din main (startup() - loadAvl(), initHTTP())
    - avl values - array[string]
    - indexat pagini (+weight / keyword / url)
    - salvat keywords in avl
    - merge 2 AVL trees
    - Hash key la avl
    - adaugat symspell
    - DHT - sharing indexes (hash->ip sau hash->urls)
    - peer protocol (get keyword(s), merge)

Docs:
    http://www.yacy-websearch.net/wiki/index.php/En:FAQ
    http://blog.notdot.net/2009/11/Implementing-a-DHT-in-Go-part-1
    http://blog.notdot.net/2009/11/Implementing-a-DHT-in-Go-part-2
    https://github.com/armon/go-chord

Use:
    - DHT
    - symspell - handle erori la search (https://github.com/heartszhang/symspell, https://github.com/sajari/fuzzy)
    - crawler - search: golang web crawler
    - indexer (Bleve, https://github.com/nassor/studies-blevesearch)
    - storage: avl tree


Beneficii:
   - ultimele tehnologii
   - concurent (multi-core), distribuit
   - modular
   - super-fast db - rocksdb/lmdb sau ceva
   - suport dark web
   - portal catre web si usor de facut portaluri personale (si pe tor)
   - separat algoritmul ca sa fie usor de modificat
   - protocol binar, custom (poate protobuf ???)
   - super-fast crawler - concurent
   - sa mearga chiar daca a cazut toata infrastructura (sa depinda de cat mai putine protocoale si infrastructura)
   - suport ML - distribuit - functionat ceva gen flink/storm ( stream processing ??? ) - nu ai puterea lui google dar poti distribui load-ul si sa ai rezultate asemanatoare
   - rezistent la caderea nodurilor
   - rezistent la hacking
   - algoritm search, ranking - votat printr-un mecanism de consens
   - extensibil
   - platforma - posibilitatea sa faci si altceva decat search peste platforma (cam ca la ethereum)
   - indexat si alte protocoale, nu doar http - ftp, samba, torrent?, etc.
   - securitate - un nod sa nu poata face rau (inside threat) - poate doar vedea ce se cauta dar trebuie mascat ip-ul si alte date de identificare
   - limitat resurse folosite
   - posibilitate sa il pui pe un raspberry si sa il accesezi de acolo
   - fiecare nod selecteaza ce resurse foloseste, ce protocoale indexeaza si limite (internet, intranet)
   - sa functioneze pe cat mai multe masini (linux, osx, win, mobile???)
   - sa fie cat mai usor de folosit

   - hash words in db
   - cryptat transferuri intre peers
   - db - word hash - urls
