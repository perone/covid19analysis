**06/March** -- COVID-19 Time varying reproduction numbers estimation for Brazil
*****************************************************************************************************
These plots show the estimation of the instantaneous reproduction number for all
the states in Brazil. These reports uses the method described in the work 
`A New Framework and Software to Estimate Time-Varying Reproduction Numbers During Epidemics <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3816335/>`_. We used the serial interval parameters similar to the ones used
by `CMMID <https://cmmid.github.io/topics/covid19/>`_ with a :math:`\mu = 4.7 (3.7 - 6.0)`
and :math:`\sigma = 2.9 (1.9 - 4.9)`.

.. note:: This plot uses official data from government, reports until
          06/March. This method is sensitive to changes in COVID-19
          testing procedures and the level of effort used to detect cases.
          Therefore, changes in the testing efforts will introduce bias
          if the testing practices are not kept consistent. So please
          keep in mind these limitations, that are often not stated in
          many analysis around there. Imported cases weren't also
          considered in this analysis, neither the delay of the symptoms
          onset and reporting.

.. warning:: Remember that this is the instantaneous reproduction number, therefore when
             it is below 1.0 for one or two days, it doesn't mean everything is ok.
             This method is less sensitive to under-reporting but as long as the bias is
             constant. So please, read the plots with the limitations in mind.
             As an example, Portugal had an R(t) below 1.0 for almost 3 weeks
             before relaxing interventions, so keep in mind that it is not
             about being below 1.0 for a single day but for weeks.

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_all.csv">
    <img src="https://raster.shields.io/badge/Download_Data-all_states-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p>

Summary for the last instantaneous reproduction number estimate
===============================================================================
.. rubric:: Map for the accumulated cases

.. raw:: html

    <iframe src="_static/restim_cases_map.html" height="591px" width="100%" frameBorder="0"></iframe>

.. rubric:: Map for the last instantaneous reproduction number estimate

.. raw:: html

    <iframe src="_static/restim_map.html" height="591px" width="100%" frameBorder="0"></iframe>

.. rubric:: Map of states with mean reproduction number R(t) > 1.0

.. raw:: html

    <iframe src="_static/restim_badr_map.html" height="591px" width="100%" frameBorder="0"></iframe>

.. rubric:: Map for the accumulated deaths by COVID-19

.. raw:: html

    <iframe src="_static/restim_deaths_map.html" height="591px" width="100%" frameBorder="0"></iframe>

.. rubric:: Summary for the last instantaneous reproduction number estimate

Last update: **06/March**

.. image:: _static/br/r0_estim/estim_all.svg
    :width: 800

.. rubric:: Summary for recent median instantaneous reproduction number estimate

Last update: **06/March**

The median R(t) estimates are clipped in 2.0 to avoid issues with the colormap.

.. raw:: html

    <iframe src="_static/br/r0_estim/estim_timeline_all.html" height="650px" width="100%" frameBorder="0"></iframe>

.. rubric:: Summary table for the last instantaneous reproduction number estimate

.. raw:: html
    
    <style>
        table.greyGridTable {
          border: 2px solid #FFFFFF;
          width: 100%;
          text-align: center;
          border-collapse: collapse;
        }
        table.greyGridTable td, table.greyGridTable th {
          border: 1px solid #FFFFFF;
          padding: 3px 4px;
        }
        table.greyGridTable tbody td {
          font-size: 13px;
        }
        table.greyGridTable td:nth-child(even) {
          background: #EBEBEB;
        }
        table.greyGridTable thead {
          background: #FFFFFF;
          border-bottom: 4px solid #333333;
        }
        table.greyGridTable thead th {
          font-size: 15px;
          font-weight: bold;
          color: #333333;
          text-align: center;
          border-left: 2px solid #333333;
        }
        table.greyGridTable thead th:first-child {
          border-left: none;
        }

        table.greyGridTable tfoot {
          font-size: 14px;
          font-weight: bold;
          color: #333333;
          border-top: 4px solid #333333;
        }
        table.greyGridTable tfoot td {
          font-size: 14px;
        }
    </style>

    <table class="greyGridTable">
    <thead>
    <tr>
    <th>State</th> 
    <th>Mean Estimated R (CI 0.975)</th>
    </tr>
    </thead>
    <tbody>
    
    <tr>
        <td>DF</td>
        <td>1.28 (1.22 - 1.34)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>1.27 (1.21 - 1.33)</td>
    </tr>
    
    <tr>
        <td>PI</td>
        <td>1.21 (1.16 - 1.26)</td>
    </tr>
    
    <tr>
        <td>RO</td>
        <td>1.21 (1.14 - 1.27)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>1.17 (1.15 - 1.20)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>1.16 (1.11 - 1.22)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>1.10 (1.05 - 1.15)</td>
    </tr>
    
    <tr>
        <td>SC</td>
        <td>1.10 (1.06 - 1.13)</td>
    </tr>
    
    <tr>
        <td>MT</td>
        <td>1.09 (1.06 - 1.12)</td>
    </tr>
    
    <tr>
        <td>GO</td>
        <td>1.07 (1.04 - 1.12)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>1.07 (1.06 - 1.08)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>1.07 (1.02 - 1.12)</td>
    </tr>
    
    <tr>
        <td>AC</td>
        <td>1.07 (1.02 - 1.11)</td>
    </tr>
    
    <tr>
        <td>TO</td>
        <td>1.06 (1.01 - 1.12)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>1.06 (1.03 - 1.08)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>1.06 (1.04 - 1.07)</td>
    </tr>
    
    <tr>
        <td>AP</td>
        <td>1.05 (1.00 - 1.11)</td>
    </tr>
    
    <tr>
        <td>MS</td>
        <td>1.04 (1.01 - 1.07)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>1.03 (0.99 - 1.08)</td>
    </tr>
    
    <tr>
        <td>SE</td>
        <td>1.02 (0.97 - 1.09)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>1.02 (1.00 - 1.05)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>1.02 (0.99 - 1.04)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>0.96 (0.93 - 0.99)</td>
    </tr>
    
    <tr>
        <td>PA</td>
        <td>0.94 (0.91 - 0.96)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>0.90 (0.87 - 0.93)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>0.88 (0.83 - 0.93)</td>
    </tr>
    
    <tr>
        <td>RR</td>
        <td>0.88 (0.83 - 0.92)</td>
    </tr>
    
    </tbody>
    </table>

.. rubric:: Summary for the Facebook COVID-like illness survey (last date)

.. image:: _static/br/facebook_survey/estim_all.svg
    :width: 800

.. note:: This is the summary for the Facebook COVID-like illness survey using
          the last survey date available for each state. Note that not all states
          have the same last date available, for more information please look
          at the plots for each state to see dynamics of these results and
          also the last available date.

.. rubric:: Summary table for the Facebook COVID-like illness (CLI) survey (last date)

.. raw:: html
    
    <table class="greyGridTable">
    <thead>
    <tr>
    <th>State</th> 
    <th>Weighted Percent of CLI responses (95% CI)</th>
    <th>Sample Size</th>
    <th>Survey Date</th>

    </tr>
    </thead>
    <tbody>
    
    <tr>
        <td>Acre</td>
        <td>7.52 (0.65 - 14.39)</td>
        <td>107</td>
        <td>23-06-2020
    </tr>
    
    <tr>
        <td>Roraima</td>
        <td>7.18 (1.20 - 13.15)</td>
        <td>111</td>
        <td>14-06-2020
    </tr>
    
    <tr>
        <td>AmapÃ¡</td>
        <td>6.79 (1.12 - 12.47)</td>
        <td>101</td>
        <td>15-01-2021
    </tr>
    
    <tr>
        <td>MaranhÃ£o</td>
        <td>4.04 (1.38 - 6.70)</td>
        <td>290</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>RondÃ´nia</td>
        <td>3.93 (0.27 - 7.59)</td>
        <td>167</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>ParaÃ­ba</td>
        <td>3.89 (1.09 - 6.68)</td>
        <td>278</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Rio Grande do Norte</td>
        <td>3.41 (0.94 - 5.89)</td>
        <td>334</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>PiauÃ­</td>
        <td>3.27 (0.32 - 6.23)</td>
        <td>189</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Alagoas</td>
        <td>3.20 (-0.05 - 6.45)</td>
        <td>176</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>ParÃ¡</td>
        <td>3.16 (1.03 - 5.28)</td>
        <td>354</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Rio Grande do Sul</td>
        <td>3.01 (1.91 - 4.11)</td>
        <td>1459</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Santa Catarina</td>
        <td>3.01 (1.53 - 4.48)</td>
        <td>791</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>CearÃ¡</td>
        <td>2.84 (1.10 - 4.57)</td>
        <td>526</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Amazonas</td>
        <td>2.76 (0.25 - 5.27)</td>
        <td>245</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Mato Grosso</td>
        <td>2.45 (0.40 - 4.50)</td>
        <td>348</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Distrito Federal</td>
        <td>2.39 (0.64 - 4.14)</td>
        <td>505</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Sergipe</td>
        <td>2.35 (-1.25 - 5.95)</td>
        <td>108</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Bahia</td>
        <td>2.33 (0.80 - 3.87)</td>
        <td>542</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>GoiÃ¡s</td>
        <td>2.32 (0.84 - 3.81)</td>
        <td>619</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Pernambuco</td>
        <td>2.22 (0.57 - 3.87)</td>
        <td>451</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>EspÃ­rito Santo</td>
        <td>1.97 (0.03 - 3.92)</td>
        <td>301</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>SÃ£o Paulo</td>
        <td>1.81 (1.31 - 2.31)</td>
        <td>4648</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>ParanÃ¡</td>
        <td>1.54 (0.67 - 2.42)</td>
        <td>1186</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Tocantins</td>
        <td>1.43 (-1.24 - 4.10)</td>
        <td>106</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Minas Gerais</td>
        <td>1.37 (0.58 - 2.15)</td>
        <td>1280</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Mato Grosso do Sul</td>
        <td>1.32 (-0.19 - 2.83)</td>
        <td>319</td>
        <td>04-03-2021
    </tr>
    
    <tr>
        <td>Rio de Janeiro</td>
        <td>1.10 (0.33 - 1.87)</td>
        <td>1287</td>
        <td>04-03-2021
    </tr>
    
    </tbody>
    </table>



**State**: Acre / AC
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_ac.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_ac-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_ac.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_ac.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_ac.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_ac.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Alagoas / AL
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_al.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_al-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_al.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_al.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_al.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_al.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Amazonas / AM
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_am.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_am-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_am.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_am.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_am.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_am.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Amapá / AP
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_ap.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_ap-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_ap.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_ap.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_ap.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_ap.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Bahia / BA
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_ba.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_ba-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_ba.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_ba.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_ba.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_ba.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Ceará / CE
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_ce.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_ce-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_ce.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_ce.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_ce.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_ce.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Distrito Federal / DF
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_df.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_df-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_df.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_df.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_df.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_df.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Espírito Santo / ES
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_es.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_es-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_es.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_es.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_es.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_es.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Goiás / GO
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_go.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_go-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_go.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_go.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_go.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_go.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Maranhão / MA
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_ma.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_ma-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_ma.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_ma.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_ma.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_ma.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Minas Gerais / MG
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_mg.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_mg-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_mg.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_mg.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_mg.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_mg.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Mato Grosso do Sul / MS
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_ms.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_ms-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_ms.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_ms.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_ms.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_ms.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Mato Grosso / MT
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_mt.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_mt-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_mt.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_mt.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_mt.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_mt.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Pará / PA
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_pa.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_pa-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_pa.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_pa.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_pa.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_pa.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Paraíba / PB
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_pb.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_pb-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_pb.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_pb.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_pb.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_pb.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Pernambuco / PE
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_pe.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_pe-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_pe.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_pe.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_pe.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_pe.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Piauí / PI
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_pi.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_pi-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_pi.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_pi.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_pi.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_pi.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Paraná / PR
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_pr.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_pr-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_pr.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_pr.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_pr.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_pr.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Rio de Janeiro / RJ
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_rj.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_rj-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_rj.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_rj.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_rj.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_rj.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Rio Grande do Norte / RN
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_rn.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_rn-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_rn.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_rn.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_rn.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_rn.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Rondônia / RO
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_ro.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_ro-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_ro.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_ro.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_ro.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_ro.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Roraima / RR
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_rr.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_rr-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_rr.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_rr.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_rr.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_rr.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Rio Grande do Sul / RS
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_rs.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_rs-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_rs.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_rs.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_rs.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_rs.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Santa Catarina / SC
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_sc.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_sc-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_sc.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_sc.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_sc.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_sc.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Sergipe / SE
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_se.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_se-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_se.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_se.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_se.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_se.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: São Paulo / SP
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_sp.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_sp-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_sp.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_sp.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_sp.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_sp.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.


**State**: Tocantins / TO
===============================================================================
.. rubric:: R(t) estimate, incidence and accumulated cases

.. raw:: html
    
    <p align="right">
    <a href="https://perone.github.io/covid19analysis/_static/br/r0_estim/r_state_to.csv">
    <img src="https://raster.shields.io/badge/Download_Data-State:_to-blue.png?style=for-the-badge&logo=codesandbox"/>
    </a></p><br/><br/>

.. image:: _static/br/r0_estim/state_to.png
  :width: 900

.. rubric:: Facebook mobility trend data for the state

.. image:: _static/br/trend_maps/relchange_to.png
  :width: 1000

.. note:: This plot uses official data from Facebook mobility data. This data is
          released with a Creative Commons Attribution International license.

.. rubric:: Mobility data for the state

.. image:: _static/br/r0_estim/mobility_state_to.png
  :width: 1000

.. rubric:: Facebook symptom survey for the state

.. image:: _static/br/facebook_survey/state_to.png
  :width: 1000

.. note:: This plot uses official data from Brazilian government as well as
          mobility data from Google Community Mobility Reports. The red markers
          on the x-axis are weekends or holidays. This plot also uses data from
          the Facebook Symptom survey data kindly hosted by University of Maryland.

