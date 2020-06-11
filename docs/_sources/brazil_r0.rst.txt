**10/June** -- COVID-19 Time varying reproduction numbers estimation for Brazil
*****************************************************************************************************
These plots show the estimation of the instantaneous reproduction number for all
the states in Brazil. These reports uses the method described in the work 
`A New Framework and Software to Estimate Time-Varying Reproduction Numbers During Epidemics <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3816335/>`_. We used the serial interval parameters similar to the ones used
by `CMMID <https://cmmid.github.io/topics/covid19/>`_ with a :math:`\mu = 4.7 (3.7 - 6.0)`
and :math:`\sigma = 2.9 (1.9 - 4.9)`.

.. note:: This plot uses official data from government, reports until
          10/June. This method is sensitive to changes in COVID-19
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

Last update: **10/June**

.. image:: _static/br/r0_estim/estim_all.svg
    :width: 800

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
        <td>RO</td>
        <td>1.52 (1.35 - 1.73)</td>
    </tr>
    
    <tr>
        <td>DF</td>
        <td>1.34 (1.24 - 1.46)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>1.34 (1.23 - 1.46)</td>
    </tr>
    
    <tr>
        <td>GO</td>
        <td>1.34 (1.25 - 1.43)</td>
    </tr>
    
    <tr>
        <td>MT</td>
        <td>1.33 (1.22 - 1.44)</td>
    </tr>
    
    <tr>
        <td>RR</td>
        <td>1.26 (1.15 - 1.38)</td>
    </tr>
    
    <tr>
        <td>AC</td>
        <td>1.23 (1.14 - 1.33)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>1.21 (1.15 - 1.26)</td>
    </tr>
    
    <tr>
        <td>SE</td>
        <td>1.20 (1.12 - 1.29)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>1.19 (1.12 - 1.27)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>1.18 (1.11 - 1.26)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>1.17 (1.11 - 1.24)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>1.17 (1.11 - 1.21)</td>
    </tr>
    
    <tr>
        <td>PI</td>
        <td>1.17 (1.08 - 1.25)</td>
    </tr>
    
    <tr>
        <td>MS</td>
        <td>1.16 (1.06 - 1.27)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>1.15 (1.10 - 1.20)</td>
    </tr>
    
    <tr>
        <td>PA</td>
        <td>1.12 (1.06 - 1.18)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>1.10 (1.06 - 1.14)</td>
    </tr>
    
    <tr>
        <td>SC</td>
        <td>1.06 (1.01 - 1.11)</td>
    </tr>
    
    <tr>
        <td>AP</td>
        <td>1.03 (0.98 - 1.07)</td>
    </tr>
    
    <tr>
        <td>TO</td>
        <td>1.02 (0.97 - 1.07)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>1.02 (0.99 - 1.05)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>1.02 (0.99 - 1.04)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>0.94 (0.88 - 0.99)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>0.91 (0.82 - 0.98)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>0.90 (0.84 - 0.94)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>0.89 (0.85 - 0.93)</td>
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
        <td>10.18 (2.97 - 17.38)</td>
        <td>112</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Amapá</td>
        <td>9.36 (1.65 - 17.06)</td>
        <td>149</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Maranhão</td>
        <td>6.96 (4.16 - 9.77)</td>
        <td>436</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Sergipe</td>
        <td>4.96 (1.31 - 8.61)</td>
        <td>223</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Alagoas</td>
        <td>4.77 (1.98 - 7.56)</td>
        <td>303</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Pará</td>
        <td>4.53 (2.09 - 6.98)</td>
        <td>410</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Ceará</td>
        <td>3.95 (1.85 - 6.06)</td>
        <td>500</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Amazonas</td>
        <td>3.46 (1.06 - 5.87)</td>
        <td>504</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Rio Grande do Norte</td>
        <td>3.33 (1.58 - 5.09)</td>
        <td>664</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Rondônia</td>
        <td>3.25 (1.00 - 5.49)</td>
        <td>349</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Pernambuco</td>
        <td>3.01 (1.14 - 4.88)</td>
        <td>498</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Bahia</td>
        <td>2.35 (0.72 - 3.97)</td>
        <td>524</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Paraíba</td>
        <td>2.26 (0.61 - 3.91)</td>
        <td>536</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Piauí</td>
        <td>2.22 (0.36 - 4.09)</td>
        <td>311</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Espírito Santo</td>
        <td>1.93 (0.68 - 3.18)</td>
        <td>828</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Mato Grosso</td>
        <td>1.92 (0.42 - 3.43)</td>
        <td>658</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Goiás</td>
        <td>1.77 (0.60 - 2.93)</td>
        <td>774</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Distrito Federal</td>
        <td>1.64 (0.66 - 2.62)</td>
        <td>1749</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Rio de Janeiro</td>
        <td>1.45 (0.48 - 2.43)</td>
        <td>1009</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Acre</td>
        <td>1.29 (-1.21 - 3.80)</td>
        <td>108</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Tocantins</td>
        <td>1.22 (-0.77 - 3.20)</td>
        <td>165</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>São Paulo</td>
        <td>1.07 (0.61 - 1.53)</td>
        <td>3089</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Mato Grosso do Sul</td>
        <td>1.01 (0.04 - 1.98)</td>
        <td>622</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Rio Grande do Sul</td>
        <td>0.98 (0.00 - 1.95)</td>
        <td>686</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Minas Gerais</td>
        <td>0.75 (-0.01 - 1.51)</td>
        <td>808</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Santa Catarina</td>
        <td>0.67 (-0.18 - 1.52)</td>
        <td>620</td>
        <td>08-06-2020
    </tr>
    
    <tr>
        <td>Paraná</td>
        <td>0.16 (-0.21 - 0.54)</td>
        <td>675</td>
        <td>08-06-2020
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

