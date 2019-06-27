---
bibliography: 'bib.bib'
title: |
    Supporting Information for “Impact of parametrized orographic gravity
    waves in the lower stratosphere”
...

**Contents of this file**

1.  Figures S1 to S10

2.  Tables S1 to Sx

**Introduction**

For understanding the middle-atmospheric circulation, a useful
quantitative framework based on transformed Eulerian-mean (TEM)
equations has been developed and is still abundantly used despite its
limitations [@Haynes2005], e.g. small-amplitude wave disturbances and
zonally symmetric basic flows. The transformation leading to the TEM
equations was introduced by @andrews1976planetary
[@andrews1978generalized; @boyd1976noninteraction]. Using TEM equations
in spherical ($\varphi$), log-pressure[^1] coordinates, we document how
in the two-dimensional perspective wave forcing affects the mean flow
($\bar{u}$) as well as the meridional transport: $$\eqnum{S1}
\bar{u}_t + \bar{v}^{*}\left[(\rho_0 a \cos \varphi)^{-1}(\bar{u} \cos \varphi)_{\varphi} -f \right] +\bar{w}^{*}\bar{u}_z = (\rho_0 a \cos \varphi)^{-1} \nabla\cdot\vec{F}+R \equiv \mathcal{\bar{F}}
\label{eq:tem}$$ where $f$ is the Coriolis parameter[^2], $a$ is the
earth’s radius, $\rho_0$ is a standard reference density and $\bar{R}$
denotes the residual term representing sub-grid scale processes such as
GWD and numerical diffusion. The vector $\vec{F}$ is known as the
Eliassen-Palm (EP) flux: $$\begin{aligned}
\eqnum{S2}
    F^{(\varphi)} &=& \rho_0 a \cos \varphi \left(\bar{u}_z \overline{v^\prime \theta^\prime}/\bar{\theta}_z - \overline{v^\prime u^\prime}\right),\\
\eqnum{S3}
    F^{(z)} &=& \rho_0 a \cos \varphi \left\{\left[f - (\rho_0 a \cos \varphi)^{-1}(\bar{u} \cos \varphi)_{\varphi} \right]\overline{v^\prime \theta^\prime}/\bar{\theta}_z- \overline{w^\prime u^\prime}\right\}\end{aligned}$$

together used in the EP flux divergence (EPFD): $$\eqnum{S4}
\nabla\cdot\vec{F} = (a \cos\varphi)^{-1} \left(F^{(\varphi)} \cos\varphi\right)_{\varphi}+ F^{(z)}_{z}
\label{eq:epfd}$$ The residual mean meridional circulation representing
the Brewer-Dobson circulation (BDC) is defined by $$\begin{aligned}
\eqnum{S5}
    \bar{v}^{*} &=& \bar{v}- \rho_0^{-1} (\rho_0 \overline{v^\prime \theta^\prime}/\bar{\theta}_z )_z, \\
\eqnum{S6}
    \bar{w}^{*} &=& \bar{w}+ (a \cos \varphi)^{-1} (\cos\varphi \overline{v^\prime\theta^\prime}/\bar{\theta}_z)_\varphi\end{aligned}$$
Overbars and primes denote zonal mean and anomalies from the zonal mean,
respectively. The subscripts denote derivatives.

Another conservation equation exists named the generalized EP theorem by
@andrews1976planetary between the divergence of EP flux
$\nabla\cdot\vec{F}$ and the time derivative of zonal-mean wave activity
density known as wave transience $A_t$: $$\eqnum{S7}
A_t + \left(a \cos\varphi\right)^{-1}\nabla\cdot\vec{F} = S
\label{eq:fawa}$$ where $S$ represents nonconservative sink or source of
wave activity. Note that we show the relationship above with the
quasigeostrophic (QG) finite-amplitude wave activity (FAWA) derived by
@Nakamura2010. @NakamuraZhu2010 have introduced FAWA based on the areal
displacement of QG potential vorticity from zonal symmetry. 2D
representation of FAWA has recently been generalized
longitudinally [@Huang2015] representing *local* wave activity (LWA) to
diagnose eddy-mean flow interaction on the regional scale. By
combination of Eqs.\[eq:tem\] in the QG form and \[eq:fawa\] we obtain
$$\eqnum{S8}
\bar{u}_t - f\bar{v}^* = -A_t + S + R
\label{eq:tem2}$$ Hence for steady and conservative waves, the zonal
mean flow (when the residual term $R$ is neglected) neither the
meridional residual circulation is accelerated. This is an example of
the nonacceleration theorem firstly noted by @Charney1961.

![Climatological relative EPFD contribution to the overall drag
(EPFD+total GWD) in January averaged over the period 1980-2010. Black
dotted line represents JRA55. Black solid line represents MERRA2 and
blue solid line represents CMAM30.<span
data-label="fig:ratio_epfd_total_jan"></span>](./img/ratio_epfd_vs_total_january.pdf)

![Climatological average of particular CMAM30 tendencies in January
averaged over the period 1980-2010. $R$ was calculated from
eq.\[eq:tem\] as a difference between
$(\rho_0 a \cos \varphi)^{-1} \nabla\cdot\vec{F}$ labeled as
$(u_t)_{\mathrm{EPFD}}$ and the left side of the equation.
$(u_t)_{\mathrm{OWGD}}$ or $(u_t)_{\mathrm{NGWD}}$ origins from outputs
of CMAM30 parameterizations, respectively.<span
data-label="fig:tem"></span>](./img/CMAM_january_climatological_comparison_origGWD_vs_GWDfromTEM_new.pdf)

![Zonal mean of temperature anomalies (shading; units: K) and absolute
(contour levels: $200,220,240,260,\mathbf{273.15}\,\mathrm{K}$)
composite average at lag=0 representing the Himalayas (left panel), East
Asian (middle panel) and West America (right panel). Green horizontal
and vertical lines represent regions of a particular GW hotspot. Black
dashed line corresponds to tropopause pressure level of respective
composite. Hatching \\\\\\\\and $////$ represents p-values $<0.05$ and
$<0.01$, respectively.<span
data-label="fig:zmta_lag0"></span>](./img/ta_anomalies_all_20days_zm_wsignificance_DJFonly.pdf)

![Zonal wind anomalies (shading; units: m/s) composite average at
$70\,\mathrm{hPa}$ at lag=0 representing the Himalayas (left panel),
East Asia (middle panel) and West America (right panel). Green boxes
represent regions of a particular GW hotspot. Black contour levels
correspond to DJF climatology.<span
data-label="fig:ua70_lag0"></span>](./img/ua@7000Pa_anomalies_allwclim_20days_wsignificancefrom10000_PlateCarree_DJFonly.pdf)

![Meridional gradient of tendency of eastward wind due to OGWD (shading;
units: $10^{-12}\,s^{-2}$) composite average at $70\,\mathrm{hPa}$ both
at lag=0 representing the Himalayas (upper panel), East Asia (middle
panel) and West America (lower panel). Green boxes represent regions of
a particular GW hotspot. Hatching \\\\\\\\and $////$ represents p-values
$<0.05$ and $<0.01$, respectively. Black contour levels correspond to
DJF climatology.<span
data-label="fig:daccelogwdy_70hpa_lag0"></span>](./img/daccelogwdy@7000Pa_anomalies_allwclim_20days_wsignificancefrom10000_PlateCarree_DJFonly.pdf)

![Ertel’s potential vorticity anomalies (shading; units:
$10^{-6}\,\mathrm{K}\cdot\mathrm{m}^2\cdot\mathrm{kg}^{-1}\cdot\mathrm{s}^{-1}$)
composite average at $70\,\mathrm{hPa}$ both at lag=0 representing the
Himalayas (left panel), East Asia (middle panel) and West America (right
panel). Green boxes represent regions of a particular GW hotspot.
Hatching \\\\\\\\and $////$ represents p-values $<0.05$ and $<0.01$,
respectively. Black contour levels correspond to DJF climatology.<span
data-label="fig:pv_70hpa_lag0"></span>](./img/vorpot@7000Pa_anomalies_all_20days_wsignificancefrom10000_PlateCarree_DJFonly.pdf)

![Tendency of Ertel’s potential vorticity anomalies (shading; units:
$10^{-6}\,\mathrm{K}\cdot\mathrm{m}^2\cdot\mathrm{kg}^{-1}\cdot\mathrm{s}^{-1}$)
composite average at $70\,\mathrm{hPa}$ both at lag=0 representing the
Himalayas (left panel), East Asia (middle panel) and West America (right
panel). Green boxes represent regions of a particular GW hotspot.
Hatching \\\\\\\\and $////$ represents p-values $<0.05$ and $<0.01$,
respectively. Black contour levels correspond to DJF climatology.<span
data-label="fig:dvorpotdt_70hpa_lag0"></span>](./img/dvorpotdt@7000Pa_anomalies_allwclim_20days_wsignificancefrom10000_PlateCarree_DJFonly.pdf)

![Vertical gradient of potential temperature (shading; units:
$10^{-3}\,\mathrm{K}/\mathrm{Pa}$) composite average at
$70\,\mathrm{hPa}$ both at lag=0 representing the Himalayas (left
panel), East Asia (middle panel) and West America (right panel). Green
boxes represent regions of a particular GW hotspot. Hatching \\\\\\\\and
$////$ represents p-values $<0.05$ and $<0.01$, respectively. Black
contour levels correspond to DJF climatology.<span
data-label="fig:dtpotdp_70hpa_lag0"></span>](./img/dtpotdp@7000Pa_anomalies_allwclim_20days_wsignificancefrom10000_PlateCarree_DJFonly.pdf)

![Tendency of vertical gradient of potential temperature (shading;
units: $10^{-10}\,\mathrm{K}/\mathrm{Pa}/\mathrm{s}$) composite average
at $70\,\mathrm{hPa}$ both at lag=0 representing the Himalayas (left
panel), East Asia (middle panel) and West America (right panel). Green
boxes represent regions of a particular GW hotspot. Hatching \\\\\\\\and
$////$ represents p-values $<0.05$ and $<0.01$, respectively. Black
contour levels correspond to DJF climatology.<span
data-label="fig:ddtpotdpdt_70hpa_lag0"></span>](./img/ddtpotdpdt@7000Pa_anomalies_allwclim_20days_wsignificancefrom10000_PlateCarree_DJFonly.pdf)

  ----------- --------------- --------------- ------------------
                **Himalayas**   **East Asia**   **West America**
    **Month**                                 
            9             NaN               1                NaN
           10             NaN               7                  1
           11             NaN              11                  6
       **12**           **5**           **9**              **9**
        **1**          **16**          **15**             **11**
        **2**          **16**          **13**              **5**
            3               7              11                  3
            4               1               6                  1
            5             NaN               1                NaN
  ----------- --------------- --------------- ------------------

  : Number of detected events per month for particular hotspot. DJF
  values are emphasized.

[^1]: $z= -H \ln (p/p_s)$ where $p_s$ is a standard reference pressure
    (usually $\approx 10^3\,\mathrm{hPa}$) and $H$ is a mean scale
    height (usually $\approx 7\,\mathrm{km}$) [@andrewsjr].

[^2]: It equals to $2\Omega \sin \varphi$ where
    $\Omega\doteq7.292\cdot10^{-5}\,\mathrm{s^{-1}}$ is the earth’s
    rotation rate.
