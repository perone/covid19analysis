**01/September** -- COVID-19 Time varying reproduction numbers estimation for Brazil
*****************************************************************************************************
These plots show the estimation of the instantaneous reproduction number for all
the states in Brazil. These reports uses the method described in the work 
`A New Framework and Software to Estimate Time-Varying Reproduction Numbers During Epidemics <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3816335/>`_. We used the serial interval parameters similar to the ones used
by `CMMID <https://cmmid.github.io/topics/covid19/>`_ with a :math:`\mu = 4.7 (3.7 - 6.0)`
and :math:`\sigma = 2.9 (1.9 - 4.9)`.

.. note:: This plot uses official data from government, reports until
          01/September. This method is sensitive to changes in COVID-19
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

Last update: **01/September**

.. image:: _static/br/r0_estim/estim_all.svg
    :width: 800

.. rubric:: Summary for recent median instantaneous reproduction number estimate

Last update: **01/September**

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
        <td>SC</td>
        <td>3.00 (2.03 - 3.82)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>1.21 (1.17 - 1.25)</td>
    </tr>
    
    <tr>
        <td>AP</td>
        <td>1.14 (1.08 - 1.20)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>1.06 (1.02 - 1.11)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>1.05 (1.00 - 1.11)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>1.05 (1.03 - 1.07)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>1.02 (0.99 - 1.07)</td>
    </tr>
    
    <tr>
        <td>MT</td>
        <td>0.98 (0.95 - 1.01)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>0.97 (0.92 - 1.03)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>0.97 (0.95 - 0.98)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>0.96 (0.94 - 0.99)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>0.95 (0.91 - 0.99)</td>
    </tr>
    
    <tr>
        <td>TO</td>
        <td>0.94 (0.91 - 0.97)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>0.93 (0.90 - 0.97)</td>
    </tr>
    
    <tr>
        <td>RO</td>
        <td>0.93 (0.89 - 0.97)</td>
    </tr>
    
    <tr>
        <td>MS</td>
        <td>0.92 (0.89 - 0.94)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>0.91 (0.90 - 0.93)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>0.91 (0.84 - 0.98)</td>
    </tr>
    
    <tr>
        <td>AC</td>
        <td>0.91 (0.84 - 0.97)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>0.91 (0.88 - 0.93)</td>
    </tr>
    
    <tr>
        <td>PA</td>
        <td>0.90 (0.86 - 0.93)</td>
    </tr>
    
    <tr>
        <td>PI</td>
        <td>0.89 (0.86 - 0.92)</td>
    </tr>
    
    <tr>
        <td>RR</td>
        <td>0.89 (0.83 - 0.95)</td>
    </tr>
    
    <tr>
        <td>GO</td>
        <td>0.88 (0.86 - 0.91)</td>
    </tr>
    
    <tr>
        <td>SE</td>
        <td>0.83 (0.78 - 0.88)</td>
    </tr>
    
    <tr>
        <td>DF</td>
        <td>0.78 (0.76 - 0.81)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>0.76 (0.71 - 0.81)</td>
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
        <td>9.67 (1.97 - 17.37)</td>
        <td>107</td>
        <td>23-06-2020
    </tr>
    
    <tr>
        <td>Roraima</td>
        <td>7.17 (1.20 - 13.15)</td>
        <td>111</td>
        <td>14-06-2020
    </tr>
    
    <tr>
        <td>Tocantins</td>
        <td>6.16 (0.89 - 11.44)</td>
        <td>106</td>
        <td>12-08-2020
    </tr>
    
    <tr>
        <td>Piauí</td>
        <td>4.69 (0.23 - 9.14)</td>
        <td>114</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Amapá</td>
        <td>4.56 (-0.21 - 9.32)</td>
        <td>103</td>
        <td>29-07-2020
    </tr>
    
    <tr>
        <td>Sergipe</td>
        <td>3.78 (-0.37 - 7.93)</td>
        <td>102</td>
        <td>26-08-2020
    </tr>
    
    <tr>
        <td>Goiás</td>
        <td>3.73 (1.62 - 5.85)</td>
        <td>441</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Pará</td>
        <td>3.36 (0.62 - 6.10)</td>
        <td>225</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Ceará</td>
        <td>3.27 (0.71 - 5.83)</td>
        <td>254</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Rondônia</td>
        <td>2.66 (-1.03 - 6.34)</td>
        <td>101</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Amazonas</td>
        <td>2.51 (-0.42 - 5.44)</td>
        <td>156</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Mato Grosso do Sul</td>
        <td>1.75 (-0.19 - 3.70)</td>
        <td>251</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Rio de Janeiro</td>
        <td>1.67 (0.48 - 2.87)</td>
        <td>656</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Espírito Santo</td>
        <td>1.64 (-0.20 - 3.48)</td>
        <td>297</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Distrito Federal</td>
        <td>1.49 (-0.18 - 3.17)</td>
        <td>373</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Mato Grosso</td>
        <td>1.43 (-0.46 - 3.32)</td>
        <td>212</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Santa Catarina</td>
        <td>1.12 (-0.09 - 2.33)</td>
        <td>443</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Rio Grande do Norte</td>
        <td>1.03 (-0.49 - 2.55)</td>
        <td>222</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>São Paulo</td>
        <td>0.98 (0.47 - 1.49)</td>
        <td>2118</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Pernambuco</td>
        <td>0.83 (-0.45 - 2.11)</td>
        <td>293</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Rio Grande do Sul</td>
        <td>0.80 (-0.12 - 1.71)</td>
        <td>531</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Paraíba</td>
        <td>0.66 (-0.73 - 2.04)</td>
        <td>176</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Paraná</td>
        <td>0.61 (-0.25 - 1.47)</td>
        <td>469</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Alagoas</td>
        <td>0.51 (-1.03 - 2.04)</td>
        <td>112</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Maranhão</td>
        <td>0.46 (-0.80 - 1.73)</td>
        <td>159</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Minas Gerais</td>
        <td>0.37 (-0.24 - 0.99)</td>
        <td>577</td>
        <td>31-08-2020
    </tr>
    
    <tr>
        <td>Bahia</td>
        <td>0.14 (-0.36 - 0.64)</td>
        <td>321</td>
        <td>31-08-2020
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

