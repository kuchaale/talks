
### Coupling processes of various timescales in the middle atmosphere
<br><br>
**Mgr. Aleš Kuchař** 
<br>@size[x-large](supervised by doc. RNDr. Petr Pišoft, Ph.D.)

@size[small](2018-09-17)


---
#### Thesis highlights
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
#### Thesis targets
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
#### The 11-year solar cycle in current reanalyses: a (non)linear attribution study of the middle atmosphere
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
                 &\text{k-variable held constant}
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
### Monthly response
Revision of mechanism by Kodera & Kuroda (2002)
![](assets/teue_merra_coefs_monthly.png)


+++
### Monthly response
#### Elliassen-palm flux diagnostics

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
### Monthly response
<br>
@div[left-40]
![RI](assets/epfd_monthly.png)
@divend
@div[right-60 fragment]
@ul
- enhanced downwelling in polar latitudes and upwelling in the equatorial region
- possible aliasing with internal variability or volc. signal
- not reproduced by GCMs (Schmidt et al, 2010; Mitchell et al, 2015b) or CCMs (Maycock et al, 2018)
@ulend
@divend



---
### On the aliasing of the solar cycle in the lower-stratospheric tropical temperature
![JGR cover](assets/aliasing.png)
+++
#### Tropical temperature response to SC (MLR)
@div[left-50]
![RI](assets/profile.png)
@divend
@div[right-50 fragment]
@ul
- concerns about the origin of the lower peak (Marsh & Garcia, 2007; Chiodo et al, 2014) observed and simulated by CCMs
- confirmed aliasing of SC with major volc. eruptions using:
  - statistical techniques: MLR and wavelet analysis
  - sensitivity simulations with CCM SOCOLv3
- possibility of decadal variation from SST interannual variability
@ulend
@divend

+++
#### Tropical temperature response to SC (wavelet)
@div[left-50]
![RI](assets/wavelet.png)
@divend
@div[right-50 fragment]
@ul
- possibility of decadal variation from SST interannual variability
- solar signal is reduced in TLS (@50 hPa) to 44% in case of REF-C1-q
- and 94% in case of REF-C1-q-clim for the period 1980–2009
- ongoing discussion on mechanism of downward signal propagation
- incorrect attribution leads to incorrect conclusions
@ulend
@divend

---
#### Role of parametrized orographic gravity waves in the lower stratosphere
![No cover](assets/motivation_fig.png)

---
#### Thesis conclusions

@ul
-
@ulend




