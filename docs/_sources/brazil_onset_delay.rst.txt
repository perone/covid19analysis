**04/May** -- Symptom onset to confirmation delay estimation for states in Brazil
*****************************************************************************************************
Since the generation time of a virus is very difficult to estimate, most studies rely on
the serial interval which is estimated from the interval between clinical onsets. Given
that most analysis use the serial interval, it is paramount to have an estimate of the 
precise onset dates of the symptoms. This work tries to provide a early estimation of 
this delay for each state in Brazil.

These plots show the estimation of the delay interval between the symptom onset date and
confirmation date for confirmed COVID-19 patients. In the plot with two panels, you will see
in the left a plot with green dots, where the darker the dot is the more patients had the
same delay interval. On the right panel of this plot we have the empirical histogram
distribution of the delays with a KDE approximation and the median showed as a dashed
black line. Below this plot you have the posterior estimation for the mean of a Gamma
distribution and with 94% credibility (HPD).

Some important points:

* I only used data from states where we have more than 30 data points in the SIVED system,
  I'm planing to extend to small data regimes but that will require the implementation
  of evaluations for different distributions;
* I'm modelling the data with a Gamma distribution and Half Normal priors with
  :math:`\sigma = 8.0` both for the :math:`\sigma` and :math:`\mu` parametrization
  of the Gamma distribution;
* SIVED data doesn't include all testing done for all states and all cities;
* The delay interval is defined as the time (in days) between the symptom onset
  and the date where the results of the test was available;
* I'm not modelling the temporal changes of this delay, so the estimate distribution
  will end up with larger uncertainty due to this to cover up for these changes;

.. note:: This plot uses official data from SIVED system in Brazil, the maximum of the 
          notification date for this data was 04/May.
          Thanks to `Marcelo Oliveira <https://twitter.com/Capyvara>`_ and to
          `Raphael Saldanha <https://twitter.com/rfsaldanhario>`_ for the help with
          the SIVED dataset.

Summary for the last instantaneous reproduction number estimate
===============================================================================
.. rubric:: Summary for the last estimates

Last date on SIVED dataset: **04/May**

.. image:: _static/br/delays/delay_all.svg
    :width: 700

.. rubric:: Summary table for the last estimates

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
    <th>Mean estimated of Gamma dist. (94% HPD credibility)</th>
    </tr>
    </thead>
    <tbody>
    
    <tr>
        <td>GO</td>
        <td>9.37 (8.54 - 10.21)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>11.17 (10.51 - 11.88)</td>
    </tr>
    
    <tr>
        <td>PA</td>
        <td>10.60 (9.91 - 11.29)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>11.22 (10.85 - 11.57)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>7.57 (6.96 - 8.20)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>9.52 (8.95 - 10.08)</td>
    </tr>
    
    <tr>
        <td>SC</td>
        <td>9.89 (9.24 - 10.59)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>9.88 (9.49 - 10.27)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>9.11 (8.61 - 9.62)</td>
    </tr>
    
    <tr>
        <td>MT</td>
        <td>10.16 (9.16 - 11.20)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>9.34 (8.38 - 10.35)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>10.95 (10.78 - 11.12)</td>
    </tr>
    
    <tr>
        <td>PI</td>
        <td>8.49 (7.51 - 9.49)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>8.20 (6.75 - 9.68)</td>
    </tr>
    
    <tr>
        <td>MS</td>
        <td>7.61 (6.64 - 8.62)</td>
    </tr>
    
    <tr>
        <td>DF</td>
        <td>7.68 (6.28 - 9.26)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>9.99 (8.65 - 11.29)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>8.72 (7.89 - 9.58)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>8.56 (7.31 - 9.78)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>11.03 (10.56 - 11.51)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>10.69 (10.34 - 11.05)</td>
    </tr>
    
    <tr>
        <td>SE</td>
        <td>7.10 (5.72 - 8.64)</td>
    </tr>
    
    </tbody>
    </table>


**State**: Alagoas / AL
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_AL_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_AL_posterior.png
  :width: 700


**State**: Amazonas / AM
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_AM_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_AM_posterior.png
  :width: 700


**State**: Bahia / BA
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_BA_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_BA_posterior.png
  :width: 700


**State**: Ceará / CE
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_CE_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_CE_posterior.png
  :width: 700


**State**: Distrito Federal / DF
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_DF_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_DF_posterior.png
  :width: 700


**State**: Espírito Santo / ES
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_ES_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_ES_posterior.png
  :width: 700


**State**: Goiás / GO
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_GO_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_GO_posterior.png
  :width: 700


**State**: Maranhão / MA
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_MA_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_MA_posterior.png
  :width: 700


**State**: Minas Gerais / MG
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_MG_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_MG_posterior.png
  :width: 700


**State**: Mato Grosso do Sul / MS
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_MS_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_MS_posterior.png
  :width: 700


**State**: Mato Grosso / MT
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_MT_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_MT_posterior.png
  :width: 700


**State**: Pará / PA
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_PA_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_PA_posterior.png
  :width: 700


**State**: Paraíba / PB
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_PB_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_PB_posterior.png
  :width: 700


**State**: Pernambuco / PE
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_PE_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_PE_posterior.png
  :width: 700


**State**: Piauí / PI
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_PI_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_PI_posterior.png
  :width: 700


**State**: Paraná / PR
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_PR_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_PR_posterior.png
  :width: 700


**State**: Rio de Janeiro / RJ
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_RJ_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_RJ_posterior.png
  :width: 700


**State**: Rio Grande do Norte / RN
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_RN_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_RN_posterior.png
  :width: 700


**State**: Rio Grande do Sul / RS
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_RS_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_RS_posterior.png
  :width: 700


**State**: Santa Catarina / SC
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_SC_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_SC_posterior.png
  :width: 700


**State**: Sergipe / SE
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_SE_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_SE_posterior.png
  :width: 700


**State**: São Paulo / SP
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/delays/state_SP_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/delays/state_SP_posterior.png
  :width: 700

