**08/August** -- COVID-19 Time varying reproduction numbers estimation for Brazil
*****************************************************************************************************
These plots show the estimation of the instantaneous reproduction number for all
the states in Brazil. These reports uses the method described in the work 
`A New Framework and Software to Estimate Time-Varying Reproduction Numbers During Epidemics <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3816335/>`_. We used the serial interval parameters similar to the ones used
by `CMMID <https://cmmid.github.io/topics/covid19/>`_ with a :math:`\mu = 4.7 (3.7 - 6.0)`
and :math:`\sigma = 2.9 (1.9 - 4.9)`.

.. note:: This plot uses official data from government, reports until
          08/August. This method is sensitive to changes in COVID-19
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

Last update: **08/August**

.. image:: _static/br/r0_estim/estim_all.svg
    :width: 800

.. rubric:: Summary for recent median instantaneous reproduction number estimate

Last update: **08/August**

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
        <td>PA</td>
        <td>1.26 (1.19 - 1.34)</td>
    </tr>
    
    <tr>
        <td>TO</td>
        <td>1.19 (1.14 - 1.23)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>1.13 (1.10 - 1.16)</td>
    </tr>
    
    <tr>
        <td>AP</td>
        <td>1.09 (1.03 - 1.15)</td>
    </tr>
    
    <tr>
        <td>GO</td>
        <td>1.09 (1.06 - 1.12)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>1.07 (1.04 - 1.10)</td>
    </tr>
    
    <tr>
        <td>PI</td>
        <td>1.07 (1.04 - 1.10)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>1.04 (1.01 - 1.08)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>1.04 (1.03 - 1.06)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>1.03 (1.01 - 1.05)</td>
    </tr>
    
    <tr>
        <td>MS</td>
        <td>1.02 (0.99 - 1.05)</td>
    </tr>
    
    <tr>
        <td>AC</td>
        <td>1.02 (0.95 - 1.11)</td>
    </tr>
    
    <tr>
        <td>DF</td>
        <td>1.02 (1.00 - 1.04)</td>
    </tr>
    
    <tr>
        <td>MT</td>
        <td>1.02 (0.99 - 1.04)</td>
    </tr>
    
    <tr>
        <td>RO</td>
        <td>1.01 (0.97 - 1.05)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>1.00 (0.98 - 1.02)</td>
    </tr>
    
    <tr>
        <td>SC</td>
        <td>0.98 (0.95 - 1.01)</td>
    </tr>
    
    <tr>
        <td>RR</td>
        <td>0.96 (0.92 - 1.00)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>0.94 (0.91 - 0.99)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>0.92 (0.89 - 0.95)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>0.92 (0.87 - 0.97)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>0.88 (0.84 - 0.91)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>0.87 (0.82 - 0.91)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>0.84 (0.82 - 0.86)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>0.82 (0.79 - 0.85)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>0.82 (0.78 - 0.87)</td>
    </tr>
    
    <tr>
        <td>SE</td>
        <td>0.71 (0.65 - 0.77)</td>
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
        <td>Roraima</td>
        <td>8.96 (2.43 - 15.50)</td>
        <td>113</td>
        <td>14-06-2020
    </tr>
    
    <tr>
        <td>Rondônia</td>
        <td>6.39 (1.89 - 10.89)</td>
        <td>177</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Tocantins</td>
        <td>6.09 (0.75 - 11.43)</td>
        <td>126</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Goiás</td>
        <td>5.37 (2.71 - 8.03)</td>
        <td>623</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Amazonas</td>
        <td>5.12 (1.53 - 8.71)</td>
        <td>237</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Maranhão</td>
        <td>4.89 (1.53 - 8.24)</td>
        <td>231</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Rio Grande do Norte</td>
        <td>4.80 (2.07 - 7.53)</td>
        <td>296</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Pará</td>
        <td>4.66 (1.79 - 7.53)</td>
        <td>283</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Amapá</td>
        <td>4.39 (-0.19 - 8.96)</td>
        <td>107</td>
        <td>29-07-2020
    </tr>
    
    <tr>
        <td>Ceará</td>
        <td>4.28 (1.71 - 6.86)</td>
        <td>353</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Sergipe</td>
        <td>3.96 (0.15 - 7.77)</td>
        <td>140</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Mato Grosso</td>
        <td>3.60 (1.32 - 5.88)</td>
        <td>378</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Acre</td>
        <td>3.41 (-1.25 - 8.06)</td>
        <td>101</td>
        <td>06-07-2020
    </tr>
    
    <tr>
        <td>Mato Grosso do Sul</td>
        <td>2.91 (0.82 - 5.00)</td>
        <td>386</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Paraíba</td>
        <td>2.70 (0.21 - 5.19)</td>
        <td>260</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Pernambuco</td>
        <td>2.30 (0.48 - 4.12)</td>
        <td>362</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Alagoas</td>
        <td>2.22 (-0.29 - 4.73)</td>
        <td>168</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Espírito Santo</td>
        <td>1.64 (0.11 - 3.17)</td>
        <td>395</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Distrito Federal</td>
        <td>1.59 (0.57 - 2.60)</td>
        <td>1309</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Rio Grande do Sul</td>
        <td>1.56 (0.45 - 2.67)</td>
        <td>704</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>São Paulo</td>
        <td>1.54 (0.96 - 2.12)</td>
        <td>2503</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Rio de Janeiro</td>
        <td>1.45 (0.41 - 2.50)</td>
        <td>712</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Santa Catarina</td>
        <td>1.42 (0.29 - 2.56)</td>
        <td>654</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Minas Gerais</td>
        <td>1.33 (0.28 - 2.37)</td>
        <td>700</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Bahia</td>
        <td>1.22 (-0.05 - 2.49)</td>
        <td>424</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Piauí</td>
        <td>1.07 (-0.61 - 2.76)</td>
        <td>185</td>
        <td>07-08-2020
    </tr>
    
    <tr>
        <td>Paraná</td>
        <td>0.89 (-0.02 - 1.80)</td>
        <td>609</td>
        <td>07-08-2020
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

