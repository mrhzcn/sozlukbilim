---
layout: post
title:  "How to use TEI for encoding Turkish dictionary"
date:   2019-08-17 19:09:21 +0300
categories: TEI Turkish
---
In order to have machine-readable dictionaries, we need to encode that dictionary in such a format or machine to read. XML is seems to be the best way to build this bridge between dictionaries and machines. TEI also come in handy in this respect, as there is a whole chapter for "Dictionaries" in the [TEI guideline][TEI_guideline]{: target="_blank"}.

During the LexMC 2017, I tried to encode the Turkish dictionary in TEI and you can read about my results here in [this post][post_link]{: target="_blank"}.

An example encoding in TEI can be seen in the following example for the lemma **ve (and)**.

~~~xml
	<entry>
            <form type="lemma">
               <orth>ve</orth>
            </form>
            <sense n="ve (I)">
               <sense>
                  <def>Türk alfabesinin yirmi yedinci harfinin adı, okunuşu.</def>
               </sense>
            </sense>
            <sense n="ve (II)">
               <gramGrp>
                  <pos>bağlaç</pos>
               </gramGrp>
               <sense>
                  <def>İki kelime veya iki cümle arasına girerek aralarında bir bağ olduğunu anlatan
                     bir söz</def>
                  <cit type="example">
                     <quote>
                        <bibl> Galiba bir vehme kapılıyorum ve galiba bir hastalık beynimi
                           kemiriyor. <author>A. Gündüz</author>
                        </bibl>
                     </quote>
                  </cit>
               </sense>
               <re type="collocation">
                  <form>
                     <orth>ve benzerleri</orth>
                  </form>
                  <form>
                     <orth>ve devamı</orth>
                  </form>
                  <form>
                     <orth>vesair</orth>
                  </form>
                  <form>
                     <orth>vesaire</orth>
                  </form>
                  <form>
                     <orth>veya</orth>
                  </form>
                  <form>
                     <orth>veyahut</orth>
                  </form>
               </re>
            </sense>
         </entry>
         <entry>
~~~

_Last updated_: {{ site.time }}

[TEI_guideline]: https://tei-c.org/release/doc/tei-p5-doc/en/html/DI.html
[post_link]:   https://digilex.hypotheses.org/275#more-275