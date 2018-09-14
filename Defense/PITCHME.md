
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


---?image=assets/gray2010_layers.png&transition=none&size=auto 90%
---?image=assets/gray2010_topdown.png&transition=none&size=auto 90%
---?image=assets/gray2010.png&size=auto 90%

+++
### Thesis targets
@ul
- (non)linear assessment of 11-yr SC in the middle atmosphere
- aliasing of 11-yr SC in the tropical lower stratosphere (TLS)
- role of parametrized oGWs 
@ulend


---?image=assets/motivation_fig1.png&transition=none&size=auto 90%
---?image=assets/motivation_fig2.png&transition=none&size=auto 90%
---?image=assets/motivation_fig3.png&transition=none&size=auto 90%
---?image=assets/motivation_fig4.png&transition=none&size=auto 90%
---?image=assets/motivation_fig5.png&transition=none&size=auto 90%

---
### The 11-year solar cycle in current reanalyses: a (non)linear attribution study of the middle atmosphere
![ACP cover](assets/nnet_fig.png)

+++
#### Attribution of SC using multiple techniques
<br>
@div[left-50]
@ul
- multiple linear regression (MLR)
- support vector regression (SVR)
- multiple layer perceptron (MLP)
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



---?image=assets/te_merra_relimpact_all_final2.png&size=90% auto

@snap[north-west]
@css[headline1](Relative impact of SC in strat. temperature (MERRA))
@snapend

+++

@div[left-50 fragment]
Relative impact (MLR)
![RI](assets/te_merra_relimpact_mlr2.png)
@divend

@div[right-50 fragment]
Regression coefficients
![coefs](assets/te_merra_coefs.png)
@divend

+++
#### Summary of (non)linear attribution
@div[left-50 fragment]
![RI](assets/te_merra_relimpact_mlr2.png)
@divend

@div[right-50]
@ul
- results by MLR confirmed MLP & SVR
- MLP & SVR required rigorous cross-validation (~computing time)
- MLP & SVR explains more variance of MA time-series
@ulend
@divend


+++
#### Monthly response
Revision of mechanism by [Kodera & Kuroda (2002)](https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2002JD002224)
![](assets/teue_merra_coefs_monthly.png)


+++
#### Monthly response
##### Elliassen-palm flux diagnostics

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
- @size[xx-large](not reproduced by GCMs (<a href="https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1029/2009JD012542" target="_blank">Schmidt et al, 2010</a>; <a href="https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/qj.2530" target="_blank">Mitchell et al, 2015</a>) or CCMs (<a href="https://www.atmos-chem-phys.net/18/11323/2018/acp-18-11323-2018.html" target="_blank">Maycock et al, 2018</a>)
@ulend
@divend



---
### On the aliasing of the solar cycle in the lower-stratospheric tropical temperature
![JGR cover](assets/aliasing.png)
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

---
### Role of parametrized orographic gravity waves in the lower stratosphere
![No cover](assets/motivation_fig.png)

+++
#### Peak detection
![No cover](assets/methodology_fig.png)

+++
#### Results: temperature response
![](assets/ta_anomalies_all_20days_zm_wabsolutevaluesandsignificance.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend


+++
#### Results: zonal wind response
![](assets/ua_anomalies_all_20days_zm_wabsolutevaluesandsignificance.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend


+++
#### Results: ozone response
![](assets/vmro3_percentages_all_20days_zm_wabsolutevaluesandsignificance.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend

+++
#### Dynamical effects: residual circulation
![](assets/epfdiag_anomalies_all_20days_zm_4poster.png)
@snap[south-east]
@size[large](`$\uparrow\ldots \bar{w}^{*} $`)<br>
@size[large](`$\rightarrow\ldots \bar{v}^{*} $`)<br>
@size[large](shading `$\ldots \nabla \cdot \vec{F}$`)<br>
@size[large](contours `$\ldots$` GWD)
@snapend

+++
#### Localized response in ozone
![](assets/epfdiag_anomalies_all_20days_zm_4poster.png)
@snap[south-east]
@size[large](\\\\\\\\`$\ldots$` p values of <0.05)<br>
@size[large](////`$\ldots$` p values of <0.01)
@snapend

+++
#### Discussion
@ul
- common features between Himalayas composite with SSWs
- position of imposed drag by oGWs may be critical for nonlocal interaction with PWs
  - compensation mechanism suggested by [Cohen et al (2014)](https://journals.ametsoc.org/doi/abs/10.1175/JAS-D-14-0021.1)
- importannce of discussion of localized dynamical effects
- not straightforward causality between oGWs and SSWs
@ulend


---
### Thesis conclusions

@ul
-
@ulend




