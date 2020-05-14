**13/May** -- COVID-19 Time varying reproduction numbers estimation for Portugal
*****************************************************************************************
These plots show the estimation of the instantaneous reproduction number for all
the regions in continental Portugal. These reports uses the method described in the work 
`A New Framework and Software to Estimate Time-Varying Reproduction Numbers During Epidemics <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3816335/>`_. We used the serial interval parameters similar to the ones used
by `CMMID <https://cmmid.github.io/topics/covid19/>`_ with a :math:`\mu = 4.7 (3.7 - 6.0)`
and :math:`\sigma = 2.9 (1.9 - 4.9)`.

.. note:: This plot uses official data Data Science for Social Good Portugal, reports until
          13/May. This method is sensitive to changes in COVID-19
          testing procedures and the level of effort used to detect cases.
          Therefore, changes in the testing efforts will introduce bias
          if the testing practices are not kept consistent. So please
          keep in mind these limitations, that are often not stated in
          many analysis around there. Imported cases weren't also
          considered in this analysis, neither the delay of the symptoms
          onset and reporting. I tried many times to enter in contact
          with DGS to understand why sometimes *accumulated cases* decrease
          from ony day to another, but they never answered, therefore I do
          linear interpolation when I have negative incidence.

Summary for the last instantaneous reproduction number estimate
===============================================================================
.. rubric:: Map for the accumulated cases

.. raw:: html

    <iframe src="_static/restim_cases_map_pt_continental.html" height="750px" width="100%" frameBorder="0"></iframe>

.. rubric:: Map for the last instantaneous reproduction number estimate

.. raw:: html

    <iframe src="_static/restim_map_pt_continental.html" height="750px" width="100%" frameBorder="0"></iframe>

.. rubric:: Map of states with mean reproduction number R(t) > 1.0

.. raw:: html

    <iframe src="_static/restim_badr_map_pt_continental.html" height="750px" width="100%" frameBorder="0"></iframe>

.. rubric:: Map for the accumulated deaths by COVID-19

.. raw:: html

    <iframe src="_static/restim_deaths_map_pt_continental.html" height="750px" width="100%" frameBorder="0"></iframe>

.. rubric:: Summary for the last instantaneous reproduction number estimate

Last update: **13/May**

.. image:: _static/pt/r0_estim/estim_all.svg
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
    <th>Region</th>
    <th>Mean Estimated R (CI 0.975)</th>
    </tr>
    </thead>
    <tbody>
    
    <tr>
        <td>alentejo</td>
        <td>1.14 (0.68 - 1.73)</td>
    </tr>
    
    <tr>
        <td>norte</td>
        <td>0.97 (0.89 - 1.05)</td>
    </tr>
    
    <tr>
        <td>rlvt</td>
        <td>0.95 (0.87 - 1.04)</td>
    </tr>
    
    <tr>
        <td>algarve</td>
        <td>0.77 (0.38 - 1.30)</td>
    </tr>
    
    <tr>
        <td>centro</td>
        <td>0.62 (0.49 - 0.78)</td>
    </tr>
    
    </tbody>
    </table>


**Region**: Alentejo
===============================================================================

.. image:: _static/pt/r0_estim/state_alentejo.png
  :width: 900


**Region**: Algarve
===============================================================================

.. image:: _static/pt/r0_estim/state_algarve.png
  :width: 900


**Region**: Centro
===============================================================================

.. image:: _static/pt/r0_estim/state_centro.png
  :width: 900


**Region**: Norte
===============================================================================

.. image:: _static/pt/r0_estim/state_norte.png
  :width: 900


**Region**: Rlvt
===============================================================================

.. image:: _static/pt/r0_estim/state_rlvt.png
  :width: 900

