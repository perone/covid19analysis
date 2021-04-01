**01/April** -- COVID-19 Time varying reproduction numbers estimation for Brazil
*****************************************************************************************************
These plots show the estimation of the instantaneous reproduction number for all
the states in Brazil. These reports uses the method described in the work 
`A New Framework and Software to Estimate Time-Varying Reproduction Numbers During Epidemics <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3816335/>`_. We used the serial interval parameters similar to the ones used
by `CMMID <https://cmmid.github.io/topics/covid19/>`_ with a :math:`\mu = 4.7 (3.7 - 6.0)`
and :math:`\sigma = 2.9 (1.9 - 4.9)`.

.. note:: This plot uses official data from government, reports until
          01/April. This method is sensitive to changes in COVID-19
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

Last update: **01/April**

.. image:: _static/br/r0_estim/estim_all.svg
    :width: 800

.. rubric:: Summary for recent median instantaneous reproduction number estimate

Last update: **01/April**

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
        <td>MS</td>
        <td>1.17 (1.12 - 1.21)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>1.12 (1.11 - 1.14)</td>
    </tr>
    
    <tr>
        <td>PI</td>
        <td>1.12 (1.08 - 1.16)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>1.09 (1.07 - 1.12)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>1.06 (1.04 - 1.09)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>1.04 (1.01 - 1.07)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>1.01 (0.99 - 1.03)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>1.01 (0.99 - 1.04)</td>
    </tr>
    
    <tr>
        <td>AP</td>
        <td>1.00 (0.96 - 1.03)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>0.99 (0.97 - 1.02)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>0.99 (0.94 - 1.03)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>0.99 (0.97 - 1.00)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>0.98 (0.93 - 1.03)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>0.97 (0.94 - 1.01)</td>
    </tr>
    
    <tr>
        <td>PA</td>
        <td>0.97 (0.95 - 1.00)</td>
    </tr>
    
    <tr>
        <td>SE</td>
        <td>0.97 (0.93 - 1.01)</td>
    </tr>
    
    <tr>
        <td>MT</td>
        <td>0.97 (0.95 - 0.99)</td>
    </tr>
    
    <tr>
        <td>DF</td>
        <td>0.95 (0.94 - 0.97)</td>
    </tr>
    
    <tr>
        <td>RO</td>
        <td>0.95 (0.92 - 0.98)</td>
    </tr>
    
    <tr>
        <td>TO</td>
        <td>0.94 (0.90 - 0.97)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>0.94 (0.89 - 0.98)</td>
    </tr>
    
    <tr>
        <td>AC</td>
        <td>0.90 (0.86 - 0.94)</td>
    </tr>
    
    <tr>
        <td>RR</td>
        <td>0.89 (0.82 - 0.96)</td>
    </tr>
    
    <tr>
        <td>GO</td>
        <td>0.88 (0.85 - 0.90)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>0.87 (0.85 - 0.90)</td>
    </tr>
    
    <tr>
        <td>SC</td>
        <td>0.79 (0.76 - 0.82)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>0.71 (0.69 - 0.74)</td>
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
        <td>ParÃ¡</td>
        <td>6.19 (3.47 - 8.90)</td>
        <td>397</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>PiauÃ­</td>
        <td>4.36 (0.84 - 7.89)</td>
        <td>175</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>RondÃ´nia</td>
        <td>4.35 (0.54 - 8.15)</td>
        <td>158</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>CearÃ¡</td>
        <td>3.93 (1.88 - 5.98)</td>
        <td>471</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>MaranhÃ£o</td>
        <td>3.59 (1.08 - 6.10)</td>
        <td>302</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Tocantins</td>
        <td>3.39 (-0.42 - 7.20)</td>
        <td>110</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Amazonas</td>
        <td>2.73 (-0.03 - 5.50)</td>
        <td>213</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Alagoas</td>
        <td>2.59 (-0.71 - 5.89)</td>
        <td>145</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Mato Grosso</td>
        <td>2.57 (0.62 - 4.52)</td>
        <td>381</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>GoiÃ¡s</td>
        <td>2.47 (0.97 - 3.97)</td>
        <td>612</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Mato Grosso do Sul</td>
        <td>2.42 (0.24 - 4.60)</td>
        <td>371</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Sergipe</td>
        <td>2.30 (-0.99 - 5.59)</td>
        <td>128</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>ParanÃ¡</td>
        <td>2.05 (1.06 - 3.04)</td>
        <td>1172</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Rio de Janeiro</td>
        <td>1.94 (1.02 - 2.85)</td>
        <td>1416</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Distrito Federal</td>
        <td>1.54 (0.12 - 2.96)</td>
        <td>534</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>SÃ£o Paulo</td>
        <td>1.32 (0.93 - 1.70)</td>
        <td>5211</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Rio Grande do Norte</td>
        <td>1.19 (-0.30 - 2.67)</td>
        <td>287</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>ParaÃ­ba</td>
        <td>1.18 (-0.41 - 2.78)</td>
        <td>278</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Rio Grande do Sul</td>
        <td>1.13 (0.40 - 1.86)</td>
        <td>1192</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Minas Gerais</td>
        <td>1.11 (0.42 - 1.80)</td>
        <td>1440</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Pernambuco</td>
        <td>1.08 (-0.07 - 2.23)</td>
        <td>441</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Bahia</td>
        <td>0.86 (-0.13 - 1.84)</td>
        <td>491</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>Santa Catarina</td>
        <td>0.79 (-0.03 - 1.61)</td>
        <td>689</td>
        <td>30-03-2021
    </tr>
    
    <tr>
        <td>EspÃ­rito Santo</td>
        <td>0.53 (-0.25 - 1.30)</td>
        <td>483</td>
        <td>30-03-2021
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

