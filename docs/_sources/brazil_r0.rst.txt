**11/April** -- COVID-19 Time varying reproduction numbers estimation for Brazil
*******************************************************************************
These plots show the estimation of the instantaneous reproduction number for all
the states in Brazil. These reports uses the method described in the work 
`A New Framework and Software to Estimate Time-Varying Reproduction Numbers During Epidemics <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3816335/>`_. We used the serial interval parameters similar to the ones used
by `CMMID <https://cmmid.github.io/topics/covid19/>`_ with a :math:`\mu = 4.7 (3.7 - 6.0)`
and :math:`\sigma = 2.9 (1.9 - 4.9)` with a log-normal distribution.

.. note:: This plot uses official data from government, reports until
          Apr 11th 2020. This method is sensitive to changes in COVID-19
          testing procedures and the level of effort used to detect cases.
          Therefore, changes in the testing efforts will introduce bias
          if the testing practices are not kept consistent. So please
          keep in mind these limitations, that are often not stated in
          many analysis around there.

Summary for the last instantaneous reproduction number estimate
===============================================================================
.. rubric:: Summary for the last instantaneous reproduction number estimate

Last update: **11/April**

.. image:: _static/br/r0_estim/estim_all.svg
    :width: 700

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
        <td>AP</td>
        <td>2.85 (1.78 - 4.67)</td>
    </tr>
    
    <tr>
        <td>PE</td>
        <td>2.63 (1.81 - 3.79)</td>
    </tr>
    
    <tr>
        <td>PB</td>
        <td>2.25 (1.52 - 3.12)</td>
    </tr>
    
    <tr>
        <td>RO</td>
        <td>2.22 (1.27 - 3.55)</td>
    </tr>
    
    <tr>
        <td>MA</td>
        <td>1.94 (1.52 - 2.51)</td>
    </tr>
    
    <tr>
        <td>SC</td>
        <td>1.93 (1.50 - 2.36)</td>
    </tr>
    
    <tr>
        <td>AC</td>
        <td>1.76 (1.13 - 2.54)</td>
    </tr>
    
    <tr>
        <td>AL</td>
        <td>1.73 (1.10 - 2.52)</td>
    </tr>
    
    <tr>
        <td>AM</td>
        <td>1.70 (1.36 - 2.18)</td>
    </tr>
    
    <tr>
        <td>ES</td>
        <td>1.65 (1.37 - 1.96)</td>
    </tr>
    
    <tr>
        <td>PI</td>
        <td>1.60 (0.95 - 2.46)</td>
    </tr>
    
    <tr>
        <td>RR</td>
        <td>1.55 (1.10 - 2.09)</td>
    </tr>
    
    <tr>
        <td>PA</td>
        <td>1.52 (1.21 - 1.90)</td>
    </tr>
    
    <tr>
        <td>GO</td>
        <td>1.50 (1.15 - 1.94)</td>
    </tr>
    
    <tr>
        <td>RJ</td>
        <td>1.46 (1.25 - 1.70)</td>
    </tr>
    
    <tr>
        <td>CE</td>
        <td>1.33 (1.15 - 1.57)</td>
    </tr>
    
    <tr>
        <td>BA</td>
        <td>1.26 (1.09 - 1.45)</td>
    </tr>
    
    <tr>
        <td>MS</td>
        <td>1.26 (0.89 - 1.69)</td>
    </tr>
    
    <tr>
        <td>MT</td>
        <td>1.25 (0.94 - 1.62)</td>
    </tr>
    
    <tr>
        <td>MG</td>
        <td>1.22 (1.08 - 1.38)</td>
    </tr>
    
    <tr>
        <td>SP</td>
        <td>1.20 (1.10 - 1.30)</td>
    </tr>
    
    <tr>
        <td>TO</td>
        <td>1.19 (0.58 - 2.04)</td>
    </tr>
    
    <tr>
        <td>SE</td>
        <td>1.11 (0.64 - 1.72)</td>
    </tr>
    
    <tr>
        <td>RS</td>
        <td>1.01 (0.87 - 1.15)</td>
    </tr>
    
    <tr>
        <td>PR</td>
        <td>0.98 (0.84 - 1.13)</td>
    </tr>
    
    <tr>
        <td>DF</td>
        <td>0.77 (0.64 - 0.91)</td>
    </tr>
    
    <tr>
        <td>RN</td>
        <td>0.53 (0.41 - 0.68)</td>
    </tr>
    
    </tbody>
    </table>


**State**: Acre / AC
===============================================================================

.. image:: _static/br/r0_estim/state_ac.png
  :width: 700


**State**: Alagoas / AL
===============================================================================

.. image:: _static/br/r0_estim/state_al.png
  :width: 700


**State**: Amazonas / AM
===============================================================================

.. image:: _static/br/r0_estim/state_am.png
  :width: 700


**State**: Amapá / AP
===============================================================================

.. image:: _static/br/r0_estim/state_ap.png
  :width: 700


**State**: Bahia / BA
===============================================================================

.. image:: _static/br/r0_estim/state_ba.png
  :width: 700


**State**: Ceará / CE
===============================================================================

.. image:: _static/br/r0_estim/state_ce.png
  :width: 700


**State**: Distrito Federal / DF
===============================================================================

.. image:: _static/br/r0_estim/state_df.png
  :width: 700


**State**: Espírito Santo / ES
===============================================================================

.. image:: _static/br/r0_estim/state_es.png
  :width: 700


**State**: Goiás / GO
===============================================================================

.. image:: _static/br/r0_estim/state_go.png
  :width: 700


**State**: Maranhão / MA
===============================================================================

.. image:: _static/br/r0_estim/state_ma.png
  :width: 700


**State**: Minas Gerais / MG
===============================================================================

.. image:: _static/br/r0_estim/state_mg.png
  :width: 700


**State**: Mato Grosso do Sul / MS
===============================================================================

.. image:: _static/br/r0_estim/state_ms.png
  :width: 700


**State**: Mato Grosso / MT
===============================================================================

.. image:: _static/br/r0_estim/state_mt.png
  :width: 700


**State**: Pará / PA
===============================================================================

.. image:: _static/br/r0_estim/state_pa.png
  :width: 700


**State**: Paraíba / PB
===============================================================================

.. image:: _static/br/r0_estim/state_pb.png
  :width: 700


**State**: Pernambuco / PE
===============================================================================

.. image:: _static/br/r0_estim/state_pe.png
  :width: 700


**State**: Piauí / PI
===============================================================================

.. image:: _static/br/r0_estim/state_pi.png
  :width: 700


**State**: Paraná / PR
===============================================================================

.. image:: _static/br/r0_estim/state_pr.png
  :width: 700


**State**: Rio de Janeiro / RJ
===============================================================================

.. image:: _static/br/r0_estim/state_rj.png
  :width: 700


**State**: Rio Grande do Norte / RN
===============================================================================

.. image:: _static/br/r0_estim/state_rn.png
  :width: 700


**State**: Rondônia / RO
===============================================================================

.. image:: _static/br/r0_estim/state_ro.png
  :width: 700


**State**: Roraima / RR
===============================================================================

.. image:: _static/br/r0_estim/state_rr.png
  :width: 700


**State**: Rio Grande do Sul / RS
===============================================================================

.. image:: _static/br/r0_estim/state_rs.png
  :width: 700


**State**: Santa Catarina / SC
===============================================================================

.. image:: _static/br/r0_estim/state_sc.png
  :width: 700


**State**: Sergipe / SE
===============================================================================

.. image:: _static/br/r0_estim/state_se.png
  :width: 700


**State**: São Paulo / SP
===============================================================================

.. image:: _static/br/r0_estim/state_sp.png
  :width: 700


**State**: Tocantins / TO
===============================================================================

.. image:: _static/br/r0_estim/state_to.png
  :width: 700

