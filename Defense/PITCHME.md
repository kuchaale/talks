
### Coupling processes of various timescales in the middle atmosphere
<br><br>
**Mgr. Aleš Kuchař** 
<br>@size[x-large](supervised by doc. RNDr. Petr Pišoft, Ph.D.)

@size[small](2018-09-17)


---
### Thesis highlights
@ul
- attribution of top-down and bottom-up coupling processes of various timescales in the middle atmosphere
- timescales tackled: 
  - **decadal:** 11-yr solar cycle (SC)
  - **intraseasonal:** orographic gravity waves (oGWs)
- adoption of open-science (tools, datasets)
@ulend

Note:

- precist


---?image=assets/gray2010_layers.png&transition=none&size=auto 90%

Note:

- stredni atmosfera (MA) od tropopauzy po homopauzu oddelujici homosferu (v níž se podstatně nemění relativní zastoupení plynů ve vzdušné směsi) od hereosfery 
- my se vsak zamerime na stratosferu a mezosferu kvuli dostupnosti data CCM a reanalyz

---?image=assets/gray2010_topdown.png&transition=none&size=auto 90%

Note:

- top-down coupling procesy obecne + vysvetleni na prikladu jedenactileteho slunecniho cyklu (**Kodera&Kuroda**) + dalsi (volk. erupce)
- nelinearni interakce, napr. s QBO

---?image=assets/gray2010.png&size=auto 90%

Note:

- bottom-up coupling processy, tj. sireni atmosferickych vln ruzneho meritka + TSI mechanismus

+++
### Thesis targets
@ul
- (non)linear assessment of 11-yr SC in the middle atmosphere (MA)
- aliasing of 11-yr SC in the tropical lower stratosphere (TLS)
- role of parametrized oGWs 
@ulend

Note:

- predstaveni struktury samotne prace
- vzhledem k nelinear. interakcim v atmosfere (SC-QBO)=>nelinear. metody
- aliasing zde chapeme jako nerozlisitelne pusobeni urcitych fenomenu v tomto pripade na dek. cas. skale
- roli orogr. gravitacnich vln zde reprezentuje coupling nizkomeritkove (parametrizovane) procesy na mezisezonni cas. skale


---?image=assets/motivation_fig1.png&transition=none&size=auto 90%

Note:

- proc se vubec zabyvame atribuci prislusnych?
- patricna detekce a atribuce signalu=>odhaleni zakladnich mechanismu (tezke: kratke rady+male amplitudy)

---?image=assets/motivation_fig2.png&transition=none&size=auto 90%

Note:

- pochopeni na datech z pozorovani=>validaci modelu, jenz muzeme posleze pouzit k predikci budouciho klimatu

---?image=assets/motivation_fig3.png&transition=none&size=auto 90%
---?image=assets/motivation_fig4.png&transition=none&size=auto 90%
---?image=assets/motivation_fig5.png&transition=none&size=auto 90%



---
### The 11-year solar cycle in current reanalyses: a (non)linear attribution study of the middle atmosphere
![ACP cover](assets/nnet_fig.png)

Note:

- atribuce jeden. SC v radach teploty, ozony a cirk. charakteristikach (revize top-down)
- v nekolika reanalyzach (**MERRA**, ERA-I, JRA-55)
- cil: porovnani MLR a nelin. metod
- vysvetleni rozdilu mezi MLR a MLP (sigmoid jako aktivacni fce)


+++
#### Attribution of SC using multiple techniques
<br>
@div[left-50]
@ul
- multiple linear regression (**MLR**)
- support vector regression (**SVR**)
- multiple layer perceptron (**MLP**)
@ulend
@divend

@div[right-50 fragment]
`$$RI = \frac{I_k}{\sum I_k}$$` 
where `$I_{k} = \sigma (\hat{y}-\hat{y_{k}})$`
`\begin{align}
\hat{y} \ldots   &\text{original model output} \\
\hat{y}_k \ldots &\text{model output when} \\ 
                 &k\text{-variable held constant}
\end{align}`
@divend

Note:

- SVR vyuziva jadrove (nelin.) transformace prom. do vice-dim. prostoru, kde je mozne provest provest v zasade lin. regresi
- krosvalidace
- RI pro porovnani dopadu jedn. fenomenu (x regr. koef.)
- median


---?image=assets/te_merra_relimpact_all_final2.png&size=90% auto

@snap[north-west]
@css[headline1](Relative impact of SC in strat. temperature (MERRA))
@snapend

Note:

- nejvetsi dopad v mezosfere
- isolovane signaly kolem v horni stratosfere (~diskontinuity)
- @TLS RI nepresahne 20% (dominance QBO a vulkanu)
- porovnatelne RI napric metodami

+++

@div[left-50 fragment]
Relative impact (MLR)
![RI](assets/te_merra_relimpact_mlr2.png)
@divend

@div[right-50 fragment]
Regression coefficients
![coefs](assets/te_merra_coefs.png)
@divend

@snap[south-east]
@size[large](@color[red](**||||**)`$\ldots$` p values of <0.05; @color[yellow](**||||**)`$\ldots$` p values of <0.01)
@snapend

Note:

- stat. vyznamnost regr. koef. (t-test overeno bootstrapem)
- normalizace na Smax-Smin
- koresponduji (prepocet RI na regr. koef.)


+++
#### Maximum RI of individual phenomena 
![maxRI](assets/max_rel_impact_SVR2.png)

Note:

- dominance SC v horni strato. a mezo.
- dominance QBO a volk. v TLS


+++
#### Summary of (non)linear attribution
@div[left-50 fragment]
![RI](assets/te_merra_relimpact_mlr2.png)
@divend

@div[right-50]
@ul
- novel MLP & SVR contributed to robustnes of signals by MLR
- MLP & SVR required rigorous cross-validation (~computing time)
- MLP & SVR explains more variance of MA time-series
@ulend
@divend

Note:

- precist


+++
#### Monthly response
Revision of mechanism by [Kodera & Kuroda (2002)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2002JD002224)
![](assets/teue_merra_coefs_monthly.png)
@snap[south-east]
@size[large](@color[red](**||||**)`$\ldots$` p values of <0.05; @color[yellow](**||||**)`$\ldots$` p values of <0.01)
@snapend

Note:

- sireni indukovaneho signalu SC smerem doly 
- ne uplne zrejmy vliv na BDC zpocatku zimy, i pres detekci stat. vyznamnych signalu



+++
#### Monthly response
Elliassen-palm flux diagnostics

@div[left-40]
![RI](assets/epfd_monthly.png)
@divend

@div[right-60 fragment]
<br>
`\begin{align}
\bar{u}_t&-f\bar{v}^{*} \\
&= \\
(a \cos\varphi)^{-1} \nabla & \cdot \vec{F}  + R 
\end{align}`
@divend

Note:

- vysvetlit rovnici vzhledem k obrazku
- interakce planetarnich vln se zakladnim zonalnim proudenim a meridionalni velkoprostorovou cirk.


+++
#### Monthly response
<br>
@div[left-40]
![RI](assets/epfd_monthly.png)
@divend
@div[right-60 fragment]
@ul
- @size[xx-large](enhanced downwelling in polar latitudes and upwelling in the equatorial region)
- @size[xx-large](possible aliasing with internal variability or volc. signal)
- @size[xx-large](not reproduced by GCMs \[<a href="https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2009JD012542" target="_blank">Schmidt et al, 2010</a>; <a href="https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/qj.2530" target="_blank">Mitchell et al, 2015</a>\] or CCMs \[<a href="https://www.atmos-chem-phys.net/18/11323/2018/acp-18-11323-2018.html" target="_blank">Maycock et al, 2018</a>\]) 
@ulend
@divend

Note:

- prestoze jsou urcite dynamicke signaly detekovany (kratka rada mereni)
- vyvstava dulezitost robustnich metod
- ne uplne zrejma reprodukce soucasnymi modely



---
### On the aliasing of the solar cycle in the lower-stratospheric tropical temperature
![JGR cover](assets/aliasing.png)

Note:

- zamereni na dopad SC v dolni tropicke stratosfere a moznou misatribuci tohoto signalu vzhledem k dalsi fenomenum projevujici se s dek. periodicitou

+++
#### Tropical temperature response to SC (MLR)
@div[left-50]
<br>
![RI](assets/profile.png)
@divend
@div[right-50 fragment]
@ul
- @size[xx-large](concerns about the origin of the lower peak [<a href="https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2007GL030935" target="_blank">Marsh & Garcia, 2007</a>; <a href="https://www.atmos-chem-phys.net/14/5251/2014/" target="_blank">Chiodo et al, 2014</a>])
- @size[xx-large](confirmed aliasing of SC with major volc. eruptions using:)
  - @size[xx-large](MLR and wavelet analysis)
  - @size[xx-large](sensitivity simulations with CCM SOCOLv3)
- @size[xx-large](possibility of decadal variation from SST interannual variability)
@ulend
@divend

Note:

- pouzite metody
- data, zejmean SOCOL (CCM, okrajove podminky, QBO-nudging)
- popis obrazku (horni vs. dolni strato)

+++
#### Temperature response to SC @TLS (wavelet)
@div[left-50]
<br>
![RI](assets/wavelet.png)
@divend
@div[right-50 fragment]
@ul
- @size[xx-large](solar signal is reduced in TLS to 44% in case of REF-C1-q)
- @size[xx-large](and 94% in case of REF-C1-q-clim for the period 1980–2009)
- @size[xx-large](ongoing discussion on mechanism of downward signal propagation)
- @size[xx-large](incorrect attribution leads to incorrect conclusions)
@ulend
@divend

Note:

- popis wavelet transformace (casove-frekvenci metoda=>nestacionarnost X FFT)
- global: prumer pres vsechny spektra, stat. vyznamnost
- precist zavery


---
### Role of parametrized orographic gravity waves in the lower stratosphere
![No cover](assets/motivation_fig.png)

Note: 

- GW vznikající působením síly zemské tíže v interakci s různými mechanickými rozruchy, např. při obtékání překážek
- jejich role roste s vyskou, posledni zjisteni vsak ukazuji, ze jsou dulezite i pro nizsi strato
- popis CMAM, rozliseni (obzvlaste pro CCMs)=> potreba paremetrizace oGWs (Scinoccca and McFarlane (2000))
- oGWD/(oGWD+nGWD+EPFD) 
- konzistentni skrze dalsi modely, rozdily vzhledem k pozorovani
- oblasti slabych zonalnich vetru ve strato=>podminky pro disipaci stac. orogr. vln


+++
#### Peak detection
![No cover](assets/methodology_fig.png)

Note:

- lehci identifikace lok. pusobeni orograf. vln+vetsi spolehlivost reanalyz
- identifikace nejvyznamejsi hotspotu @70 hPa
- detekce nejvyznamejsi peaku vzdalenych 20 nebo 30 dni **v zime**
- zprumerovani=>kompozity
- nejvetsi amplitude pro WestAmer
- nejcastejsi pro EastAsia

+++
#### Results: temperature response
![](assets/ta_anomalies_all_20days_zm_wabsolutevaluesandsignificance.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend

Note:

- stat. vyznamnost byla testovana vzhledem k 100k nahodnych vzorku=>odhad norm. rozdeleni=>vypocet p-hodnot
- spolecna negativni anomalie v dolni mezo, stat. vyznamna na hladine vyznamnosti p<0.01
- dale vyrazna pos. anomalie v dolni polarni strato pro komp. Himalaji


+++
#### Results: zonal wind response
![](assets/ua_anomalies_all_20days_zm_wabsolutevaluesandsignificance.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend

Note:

- odezva v teplote koresponduje se zonalnim vetrem
- zeslabeni PNJ, zesileni subtropickeho jetu


+++
#### Results: ozone response
![](assets/vmro3_percentages_all_20days_zm_wabsolutevaluesandsignificance.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend

Note: 

- stejne pozitivni jako teplota v dolni strato
- dynamicky induk. anomalie v teplote ma vliv na fotochemii ozonu, coz urychluje jeho destrukci



+++
#### Dynamical effects: residual circulation
![](assets/epfdiag_anomalies_all_20days_zm_4poster.png)
@snap[south-east]
@size[large](`$\uparrow\ldots \bar{w}^{*} $`)<br>
@size[large](`$\rightarrow\ldots \bar{v}^{*} $`)<br>
@size[large](shading `$\ldots \nabla \cdot \vec{F}$`)<br>
@size[large](contours `$\ldots$` oGWD)
@snapend

Note:

- stejny pattern pro vsechny kompozity v mezosfere (pos. anomalie v EPFD)
- zvysena disipace pro Himalaje
- downward control=>intenzifikace BDC
- podobne rysy jako v pripade SSW


+++
#### Localized response in ozone @70hPa
![](assets/vmro3@70hPa_percentages_all_20days_wsignificancefrom100000_tinypng.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend

Note:

- prestoze stat. nevyznamne anom. v zon. prumeru (maskovani), zejmena pro EA a WA
- pusobeni GW je zonalne asymetricke=>potreba 3D diagnostik (odkaz na LWA+Plumb)


+++
#### Discussion
@ul
- common features between Himalayas composite with SSWs
- position of imposed drag by oGWs may be critical for nonlocal interaction with PWs
  - compensation mechanism suggested by [Cohen et al (2014)](https://journals.ametsoc.org/doi/abs/10.1175/JAS-D-14-0021.1)
- importance of discussion of localized dynamical effects
- not straightforward causality between oGWs and SSWs
@ulend

Note:

- perturbace GW mimo surf zone zpusobi nelokalni interakci s PWs a zeslabeni vortex
- zintenzivneni vert. propagace PW a negativni anomalie EPFD
- dusledkem asym. povahy pusobeni GWs nutna diskuze a aplikace 3D diagnostik
- overeti kauzality pomoci mech. ci komplexnejsiho modelu




---
### Thesis conclusions

@ul
- benefits and caveats of (non)linear attribution techniques to study interactions in the atmosphere
- rigorous attribution avoiding potential aliasings => correct conclusions about coupling mechanisms
- importance of GW perturbation outside of the surf zone for vortex preconditioning \[[Albers & Birner, 2014](http:
//journals.ametsoc.org/doi/abs/10.1175/JAS-D-14-0026.1)\]
- ?single **unifying** (top-down) mechanism acting across different timescales \[[Kidston et al, 2015](http://www.nature.com/doifinder/10.1038/ngeo2424)\]
@ulend




