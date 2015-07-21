Könnun falla
============

.. todo:: 
    stækka letur/ása á myndum? 
Inngangur
---------

.. warning::
    **Frávik frá bókinni**

    Það sem á eftir kemur er eitt af fáum atriðum þar sem mín nálgun og
    skilgreiningar eru frábrugðnar þeim í bókinni.

Hver er munurinn?
~~~~~~~~~~~~~~~~~

+---------------------------------------+--------------------------------------+ 
|.. _figa:                              |.. _figb:                             | 
|                                       |                                      | 
|.. image:: ./myndir/kafli05/01_f1.png  |.. image:: ./myndir/kafli05/01_g1.png | 
|   :width: 95 %                        |   :width: 95 %                       | 
|   :align: center                      |   :align: center                     | 
|                                       |                                      | 
+---------------------------------------+--------------------------------------+ 

Skoðum föllin tvö að ofan, þau eru augljóslega ekki eins, þannig að
spurningin er hvernig getum við lýst því muninum á þeim?

Þau hugtök sem við höfum skoðað hingað til geta ekki greint á milli
þessara falla:

(i)   Þau hafa sama skilgreiningarmengið :math:`[A,B]`

(ii)  Þau taka sömu gildin í endapunktunum

(iii) Þau hafa bæði hágildi í :math:`A` og lággildi í :math:`B`

(iv)  Þau eru bæði minnkandi (neikvæð afleiða)

Drögum sniðil
~~~~~~~~~~~~~

+---------------------------------------+--------------------------------------+ 
|.. _figa:                              |.. _figb:                             | 
|                                       |                                      | 
|.. image:: ./myndir/kafli05/01_f2.png  |.. image:: ./myndir/kafli05/01_g2.png | 
|   :width: 95 %                        |   :width: 95 %                       | 
|   :align: center                      |   :align: center                     | 
|                                       |                                      | 
+---------------------------------------+--------------------------------------+ 

Ef við veljum nú tvo punkta á :math:`[A,B]` af handahófi, köllum þá
:math:`x_1` og :math:`x_2`, og drögum línu (sniðil) í gegnum punktana á
grafum :math:`f` og :math:`g` þá sjáum við að sniðillinn lendir fyrir
neðan :math:`g` en ofan :math:`f`.

Sérhvern punkt á milli :math:`x_1` og :math:`x_2`, getum við skrifað
:math:`\alpha x_1 + (1-\alpha)x_2`, :math:`\alpha \in [0,1]`. Þá er
:math:`y`-hnit punktsins á sniðlinum með þetta :math:`x`-hnit gefið með

.. math:: \alpha f(x_1) + (1-\alpha) f(x_2), \qquad \alpha \in [0,1],

á fyrri myndinni og

.. math:: \alpha g(x_1) + (1-\alpha) g(x_2), \qquad \alpha \in [0,1],

á myndinni fyrir :math:`g`.

Ef :math:`f` liggur fyrir neðan sniðilinn þá þýðir það að fallgildi
:math:`f` í punktunum :math:`\alpha x_1 + (1-\alpha)x_2` liggur fyrir
neðan punktinum á sniðlinum, það er

.. math:: f(\alpha x_1+(1-\alpha)x_2)\leq \alpha f(x_1)+(1-\alpha)f(x_2).

Eins, ef :math:`g` liggur fyrir ofan sniðilinn þá gildir að

.. math:: g(\alpha x_1+(1-\alpha)x_2)\geq \alpha g(x_1)+(1-\alpha)g(x_2).


+---------------------------------------+--------------------------------------+ 
|.. _figa:                              |.. _figb:                             | 
|                                       |                                      | 
|.. image:: ./myndir/kafli05/01_f3.png  |.. image:: ./myndir/kafli05/01_g3.png | 
|   :width: 95 %                        |   :width: 95 %                       | 
|   :align: center                      |   :align: center                     | 
|                                       |                                      | 
+---------------------------------------+--------------------------------------+ 

Kúpni
-----

.. index::
    kúpni
    fall; kúpt
    fall; hvelft

Skilgreining
~~~~~~~~~~~~

Látum :math:`f:[a, b]\rightarrow {\mathbb  R}` vera fall.

(i)  Segjum að fallið :math:`f` sé *kúpt* (e. convex, concave up) ef um
     alla punkta :math:`x_1, x_2\in [a, b]` og sérhverja tölu
     :math:`0\leq
     \alpha\leq 1` gildir að

     .. math:: f(\alpha x_1+(1-\alpha)x_2)\leq \alpha f(x_1)+(1-\alpha)f(x_2).

(ii) Segjum að fallið :math:`f` sé *hvelft* (e. concave, concave down)
     ef um alla punkta :math:`x_1, x_2\in [a, b]` og sérhverja tölu
     :math:`0\leq
     \alpha\leq 1` gildir að

     .. math:: f(\alpha x_1+(1-\alpha)x_2)\geq \alpha f(x_1)+(1-\alpha)f(x_2).

.. note::

    Hér erum við komin með hugtak sem getur útskýrt muninn á myndunum í byrjun
    kaflans, :math:`f` er kúpt og :math:`g` er hvelft.

Auðkenning á kúpni með afleiðum
-------------------------------

+---------------------------------------+--------------------------------------+ 
|.. _figa:                              |.. _figb:                             | 
|                                       |                                      | 
|.. image:: ./myndir/kafli05/01_f1.png  |.. image:: ./myndir/kafli05/01_g1.png | 
|   :width: 95 %                        |   :width: 95 %                       | 
|   :align: center                      |   :align: center                     | 
|                                       |                                      | 
+---------------------------------------+--------------------------------------+ 

Athugasemd
~~~~~~~~~~

Ef við skoðum afleiður fallanna :math:`f` og :math:`g` betur þá sjáum
við að:

(i)  Afleiða :math:`f` er mjög neikvæð nálægt :math:`A` og nálgast svo 0
     í :math:`B`, það er afleiðan er vaxandi.

(ii) Afleiða :math:`g` er u.þ.b. 0 í :math:`A` og minnkar svo þegar við
     nálgumst :math:`B`, það er afleiðan er minnkandi.

Með öðrum orðum

.. math::

   (f')' = f'' \geq 0 \qquad   \text{og} \qquad
       (g')' = g'' \leq 0.


Setning
~~~~~~~

Fyrir tvídiffranlegt fall :math:`f` þá er eftirfarandi jafngilt

(i)   :math:`f` er kúpt

(ii)  :math:`f'` er vaxandi

(iii) :math:`f'' \geq 0`

Setning
~~~~~~~

Fyrir tvídiffranlegt fall :math:`g` þá er eftirfarandi jafngilt

(i)   :math:`g` er hvelft

(ii)  :math:`g'` er minnkandi

(iii) :math:`g'' \leq 0`

.. warning::
    Hvort fall er kúpt eða hvelft er **algjörlega óháð** því hvort það er
    vaxandi eða minnkandi. Til dæmis er :math:`f(x) = x^2` kúpt en það er
    vaxandi þegar :math:`x>0` og minnkandi þegar :math:`x<0`.


.. warning::
    Fall þarf eru ekki alltaf annað hvort kúpt eða hvelft alls staðar. Alveg
    eins og það eru til föll sem eru sums staðar vaxandi og sums staðar
    minnkandi, þá eru mörg föll sums staðar kúpt og sums staðar hveld, til
    dæmis hornaföllin.

Beygjuskilapunktar
------------------

.. index:: beygjuskilapunktar

Skilgreining
~~~~~~~~~~~~

Punktur :math:`(x_0, f(x_0))` er sagður vera *beygjuskilapunktur*
(e. inflection point) grafsins :math:`y=f(x)` ef

(i)  grafið hefur snertilínu í :math:`x_0`, og

(ii) grafið er kúpt öðru megin við :math:`x_0` og hvelft hinum megin við
     :math:`x_0`.

Setning
~~~~~~~

Ef fallið :math:`f` er tvídiffranlegt þá er punkturinn :math:`x_0`
beygjuskilapunktur fallsins :math:`f` ef og aðeins ef
:math:`f''(x_0) =0` og :math:`f''` skiptir um formerki í :math:`x_0`.

.. image:: ./myndir/kafli05/05_beygjuskilapunktur.png


.. index:: 
    útgildi; út frá annarri afleiðu

Útgildi
-------

Hvar á að leita útgilda
~~~~~~~~~~~~~~~~~~~~~~~

Sjá kafla 3 fyrir skilgreinginu á útgildi.
.. todo::  Búa til tilvísun milli kafla
Punktar sem koma til greina fyrir staðbundin útgildi falls :math:`f` eru

(i)   punktar :math:`x_0` þar sem :math:`f'(x_0)=0`,

(ii)  punktar :math:`x_0` þar sem :math:`f'(x_0)` er ekki skilgreint,

(iii) þeir endapunktar skilgreiningarmengisins þar sem fallið er
      skilgreint.

Hágildi/lágildi út frá formerki afleiðu
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Látum :math:`x_0` vera innri punkt á skilgreiningarsvæði :math:`f`.
Gerum ráð fyrir að :math:`f` sé diffranlegt í öllum punktum í einhverju
bili utan um :math:`x_0` og að :math:`f'(x_0)=0`.

(i)   Ef formerki :math:`f'` breytist úr plús í mínus í :math:`x_0`
      (farið frá vinstri til hægri eftir rauntalnaásnum) þá er
      staðbundið hágildi í :math:`x_0`.

(ii)  Ef formerki :math:`f'` breytist úr mínus í plús í :math:`x_0` þá
      er staðbundið lággildi í :math:`x_0`.

(iii) Ef formerki :math:`f'` breytist ekki í :math:`x_0` þá er hvorki
      há- né lággildi í :math:`x_0`.

Útgildi og önnur afleiðan
~~~~~~~~~~~~~~~~~~~~~~~~~

(i)  Ef :math:`f'(x_0)=0` og :math:`f''(x_0)<0` þá er :math:`x_0`
     staðbundið hágildi.

(ii) Ef :math:`f'(x_0)=0` og :math:`f''(x_0)>0` þá er :math:`x_0`
     staðbundið lággildi.

.. warning::
    Athugið að ef :math:`f''(x_0)=0` þá getur :math:`x_0` verið hvort sem er
    staðbundið hágildi, staðbundið lággildi eða beygjuskilapunktur.

    
.. index::
    aðfellur
    aðfellur; lóðrétt 
    aðfellur; lárétt
    aðfellur; skáfella
    see: skáfella; aðfellur
    
Aðfellur
--------

Skilgreining: Lóðrétt aðfella
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Fallið :math:`f` hefur *lóðrétta aðfellu* í punktinum :math:`a` ef
:math:`\lim_{x\to a^-} f(x) = \pm \infty` og/eða
:math:`\lim_{x\to a^+} f(x) = \pm \infty`.

Aðfellan er þá línan :math:`x=a`.

.. image:: ./myndir/kafli05/06_lodfellur.png

*Fallið* :math:`\frac{1}{sin(x)}` *hefur lóðréttar aðfellur í öllum punktum þar sem* :math:`sin(x)=0`. 

Skilgreining: Lárétt aðfella
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Fallið :math:`f` hefur *lárétta aðfellu* ef
:math:`\lim_{x\to \infty} f(x) = L` og/eða
:math:`\lim_{x\to -\infty} f(x) = L`.

Aðfellan er þá línan :math:`y=L`.

.. image:: ./myndir/kafli05/06_arctanadfellur.png

*Fallið* :math:`\arctan(x)` *hefur tvær láréttar aðfellur,* :math:`y=\frac{\pi}{2}` *og* :math:`y=\frac{\pi}{2}


Skáfella
~~~~~~~~

Fallið :math:`f` hefur *skáfellu* ef til eru :math:`a` og :math:`b`
þannig að :math:`\lim_{x\to \infty} f(x) -ax-b = 0` og/eða
:math:`\lim_{x\to -\infty} f(x) -ax-b= 0`.

Skáfellan er þá línan :math:`y=ax+b`.

.. image:: ./myndir/kafli05/06_lodogskafellur.png

*Fallið* :math:`\frac{x^2}{2x-4}` *hefur skáfelluna* :math:`y=\frac{1}{2}x+1` *auk lóðréttu aðfellunnar* :math:`x=2`.

Að teikna graf falls
--------------------

.. todo:: þýða og staðfæra

Uppkast að þýðingu:

Þegar teikna á graf fallsins :math:`f` er gagnlegt að fara í gegnum atriðin á eftirfarandi lista:

1. Ákvarðið :math:`f'` og :math:`f''`, og þáttið útkomurnar ef hægt er. 
2. Kannið :math:`f` til að ákvarða skilgreiningarmengi þess auk eftirfarandi eiginleika:
    (a) Lóðréttar aðfellur. (Leitið að rótum nefnara)
    (b) Láréttar aðfellur og skáfellur. (Finnið :math:`\lim_{x \to \pm\infty}f(x)`.)
    (c) Samhverfa (er :math: `f` jafnstætt eða oddstætt?)
    (d) Skurðpunktar við ása (punktar með hnit :math:`(x,0)` eða :math:`(0,y)`), endapunktar ferilsins eða aðrir punktar á grafinu þar sem einfalt er að reikna út bæði hnitin.
3. Kannið :math:`f'` til að ákvarða eftirfarandi:
    (a) Útgildispunktar.
    (b) Punktar þar sem :math:`f'` er ekki skilgreint (sérstöðupunktar(?), endapunktar skilgreiningarmengis :math:`f` og lóðfellur)
    (c) Bilin þar sem :math:`f'` er jákvætt
        og neikvætt. Það er góð hugmynd að setja þessar upplýsingar fram í töflu. Á töfluna má svo líka merkja inn niðurstöður um hvar :math:`f` er vaxandi og minnkandi og hvort útgildispunktar séu staðbundin hágildi eða lággildi.
4. Kannið :math:`f''` til að ákvarða eftirfarandi:
    (a) Punktar þar sem :math:`f''(x)=0`.
    (b) Punktar þar sem :math:`f''` er ekki skilgreint (sérstöðupunktar, endapunktar skilgreiningarmengis :math:`f` og lóðfellur, e.t.v. auk fleiri punkta þar sem :math:`f'` er skilgreint en ekki :math:`f''`.)
    (c) Bilin þar sem :math:`f''` er jákvætt og neikvætt og :math:`f` þar af leiðandi kúpt og hvelft. Hér er gagnlegt að teikna töflu.
    (d) Beygjuskilapunktar.

.. image:: ./myndir/kafli05/08_checklist.png

.. index:: 
    útgildisverkefni

Útgildisverkefni
----------------

Markmiðið
~~~~~~~~~

Þessi verkefni sem við skoðum snúast um það að finna fall fyrir stærð
sem við höfum áhuga á (verð, rúmmál, lengd,...) og hámarka/lágmarka
hana.

Til þess að þetta sé mögulegt má fallið bara vera háð einni breytu og
það þarf helst að vera diffranlegt.

Þá getum við fundið útgildi með þeim aðferðum sem við erum búin að koma
okkur upp.

Að leysa útgildisvandamál
~~~~~~~~~~~~~~~~~~~~~~~~~

Sjá einnig bls. 259 (238 í 6. útgáfu) í kennslubók.

(i)    Lesið vandamálið vandlega og áttið ykkur á því hvert það er og
       hvað á að finna.

(ii)   Teiknið mynd ef mögulegt er, hún gefur oft upplýsingar um skorður
       sem hjálpa okkur við að útbúa fallið.

(iii)  Skilgreinið aukabreytur.

(iv)   Skilgreinið fallið, sem fall af einni eða fleiri breytum.

(v)    Finnið skorður (jöfnur) sem hægt er að stinga inn í fallið

(vi)   Skrifið fallið sem fall af einni breytu.

(vii)  Finnið útgildi

(viii) Dragið ályktanir af niðurstöðunni, og athugið hvort hún sé
       raunhæf miðað við verkefnið (rúmmál á ekki að vera neikvætt og
       þess háttar).

Dæmi: Gosdós
~~~~~~~~~~~~

Hvert er hagkvæmasta formið á sívalningslaga gosdós?

.. image:: ./myndir/kafli05/09_cylinder.png

Dæmi: Kassi
~~~~~~~~~~~

Hver er stærsti (mesta rúmmálið) loklausi kassinn sem hægt er búa til úr
örk sem er :math:`12 \times 12`?

.. image:: ./myndir/kafli05/09_kassi.png
