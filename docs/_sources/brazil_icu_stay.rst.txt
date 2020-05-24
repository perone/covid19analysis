**18/May** -- ICU length of stay (LOS) estimation for states in Brazil
*****************************************************************************************************
The length of stay (LOS) of confirmed COVID-19 patients in ICUs is an important quantity
to estimate, as it shows how long a patient will be allocating resources such
as health workers, equipment, ICU beds, etc.

These plots show the estimation of the ICU stay length for each state in Brazil.
In the plot with two panels, you will see in the left a plot with green dots, where
the darker the dot is the more patients had the same stay interval. On the right
panel of this plot we have the empirical histogram distribution of the stays with the
mean showed as a dashed black line. Below this plot
you have the posterior estimation for the mean and std. dev. of a Gamma distribution
and with 90% credibility (HPD).

Some important points:

* There is no distinction of non-survivor vs survivor, this analysis includes both
  cohorts;
* I only used data from states where we have more than 30 data points in the SIVEP system,
  I'm planing to extend to small data regimes but that will require the implementation
  of evaluations for different distributions;
* I'm modelling the data with a Gamma distribution and Exponential priors with
  :math:`\lambda = 0.5` both for the :math:`\sigma` and :math:`\mu` parametrization
  of the Gamma distribution;
* SIVEP data doesn't include all testing done for all states and all cities;
* The stay interval is defined as the time (in days) between the date of entrance in the
  ICU (DT_ENTUTI) and the date when the patient exited the ICU (DT_SAIDUTI);
  I'm not modelling the temporal changes of this delay, so the estimate distribution
  will end up with larger uncertainty due to this to cover up for these changes;

.. note:: This plot uses official data from SIVEP system in Brazil, the maximum of the 
          notification date for this data was 18/May.

Summary for the ICU stay estimates
===============================================================================
.. rubric:: Summary for the Gamma mean estimates

Last date on SIVEP dataset: **18/May**

.. image:: _static/br/time_icu/delay_mu_all.svg
    :width: 800

.. rubric:: Summary for the Gamma std. dev. estimates

Last date on SIVEP dataset: **18/May**

.. image:: _static/br/time_icu/delay_sd_all.svg
    :width: 800

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
    <th>Mean estimated of Gamma dist. (90% HPD credibility)</th>
    <th>Std. Dev. estimated of Gamma dist. (90% HPD credibility)</th>
    </tr>
    </thead>
    <tbody>
    
    <tr>
        <td>PA</td>
        <td>6.70 (5.49 - 7.94)</td>
        <td>6.72 (5.30 - 8.10)</td>
    </tr>
    
    <tr>
        <td>SC</td>
        <td>9.38 (7.24 - 11.41)</td>
        <td>10.54 (8.06 - 12.99)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>9.97 (8.74 - 11.24)</td>
        <td>10.70 (9.16 - 12.17)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>7.07 (5.86 - 8.25)</td>
        <td>8.45 (6.86 - 9.96)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>5.56 (4.92 - 6.20)</td>
        <td>8.47 (7.43 - 9.50)</td>
    </tr>
    
    <tr>
        <td>DF</td>
        <td>8.27 (6.69 - 9.93)</td>
        <td>8.73 (6.81 - 10.54)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>10.42 (9.15 - 11.68)</td>
        <td>11.15 (9.62 - 12.68)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>7.33 (7.02 - 7.65)</td>
        <td>9.19 (8.75 - 9.63)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>5.89 (5.15 - 6.60)</td>
        <td>8.39 (7.30 - 9.51)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>7.35 (6.71 - 8.01)</td>
        <td>9.03 (8.11 - 9.88)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>4.61 (3.69 - 5.51)</td>
        <td>6.12 (4.81 - 7.41)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>5.71 (4.06 - 7.26)</td>
        <td>6.25 (4.40 - 8.12)</td>
    </tr>
    
    <tr>
        <td>GO</td>
        <td>6.95 (5.35 - 8.45)</td>
        <td>8.21 (6.27 - 10.19)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>3.26 (2.09 - 4.44)</td>
        <td>5.87 (3.70 - 7.97)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>7.06 (6.07 - 8.07)</td>
        <td>6.90 (5.74 - 8.00)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>6.67 (5.17 - 8.10)</td>
        <td>7.88 (5.98 - 9.70)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>4.27 (2.87 - 5.67)</td>
        <td>5.83 (3.83 - 7.79)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>3.52 (2.09 - 4.84)</td>
        <td>5.90 (3.48 - 8.10)</td>
    </tr>
    
    </tbody>
    </table>


**State**: Alagoas / AL
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_AL_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_AL_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_AL_posterior_sd.png
  :width: 700



**State**: Amazonas / AM
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_AM_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_AM_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_AM_posterior_sd.png
  :width: 700



**State**: Bahia / BA
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_BA_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_BA_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_BA_posterior_sd.png
  :width: 700



**State**: Ceará / CE
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_CE_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_CE_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_CE_posterior_sd.png
  :width: 700



**State**: Distrito Federal / DF
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_DF_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_DF_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_DF_posterior_sd.png
  :width: 700



**State**: Espírito Santo / ES
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_ES_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_ES_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_ES_posterior_sd.png
  :width: 700



**State**: Goiás / GO
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_GO_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_GO_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_GO_posterior_sd.png
  :width: 700



**State**: Maranhão / MA
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_MA_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_MA_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_MA_posterior_sd.png
  :width: 700



**State**: Minas Gerais / MG
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_MG_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_MG_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_MG_posterior_sd.png
  :width: 700



**State**: Pará / PA
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_PA_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_PA_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_PA_posterior_sd.png
  :width: 700



**State**: Paraíba / PB
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_PB_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_PB_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_PB_posterior_sd.png
  :width: 700



**State**: Pernambuco / PE
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_PE_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_PE_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_PE_posterior_sd.png
  :width: 700



**State**: Paraná / PR
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_PR_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_PR_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_PR_posterior_sd.png
  :width: 700



**State**: Rio de Janeiro / RJ
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_RJ_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_RJ_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_RJ_posterior_sd.png
  :width: 700



**State**: Rio Grande do Norte / RN
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_RN_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_RN_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_RN_posterior_sd.png
  :width: 700



**State**: Rio Grande do Sul / RS
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_RS_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_RS_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_RS_posterior_sd.png
  :width: 700



**State**: Santa Catarina / SC
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_SC_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_SC_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_SC_posterior_sd.png
  :width: 700



**State**: São Paulo / SP
=======================================================================================
.. rubric:: Scatter plot of symptom onset vs confirmation and empirical distribution

.. image:: _static/br/time_icu/state_SP_delay.png
  :width: 1200

.. rubric:: Posterior distribution for the mean of the Gamma distribution

.. image:: _static/br/time_icu/state_SP_posterior_mu.png
  :width: 700

.. rubric:: Posterior distribution for the std. dev. of the Gamma distribution

.. image:: _static/br/time_icu/state_SP_posterior_sd.png
  :width: 700


