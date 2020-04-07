COVID-19 Analysis for Brazil
*******************************************************************************
This section contains analysis done for Brazil.

Brazil: country-wide analysis
===============================================================================

.. _DeathCountModelling:

Bayesian death count modelling
-------------------------------------------------------------------------------
It is known that there is a heavy under-reporting of cases in Brazil due to
lack of testing capacity (this was acknoledged by the government), therefore
using confirmed cases poses difficult challenges. I decided to focus this
analysis on the deaths, as they seem to be less impacted by the lack of the
testing capacity.

To model the death counts I used a `Negative Binomial` likelihood, the same
distribution used in the work `Estimating the number of infections and the impact
of nonpharmaceutical interventions on COVID-19 in 11 European countries <https://www.imperial.ac.uk/mrc-global-infectious-disease-analysis/covid-19/report-13-europe-npi-impact/>`_ by Imperial College London.

The negative binomal distribution is interesting because it is a discrete distribution
and can be used to model over-dispersion as Poisson assumes :math:`\mathrm{E}[x] = \mathrm{Var}[x]`,
therefore we can have more flexibility to model variance separately.

The priors of the model are described below:

.. math::

	\begin{array}{rcl}
    \text{alpha_mu} &\sim & \text{Normal}(\mathit{mu}=0.0,~\mathit{sigma}=10.0)\\\text{alpha} &\sim & \text{Normal}(\mathit{mu}=\text{alpha_mu},~\mathit{sigma}=10.0)\\\text{beta_mu} &\sim & \text{Normal}(\mathit{mu}=0.0,~\mathit{sigma}=10.0)\\\text{beta} &\sim & \text{Normal}(\mathit{mu}=\text{beta_mu},~\mathit{sigma}=10.0)\\\text{sigma} &\sim & \text{HalfCauchy}(\mathit{beta}=50.0)\\\text{y} &\sim & \text{NegativeBinomial}(\mathit{mu}=f(f(\text{alpha}),~f(f(f(\text{beta}),~\text{data_x}))),~\mathit{alpha}=\text{sigma})
    \end{array}

The model is an exponential model as it is a very good approximation due to the natural phenomena that
arises from the nature of viruses transmission dynamics. The model is:

.. math::

	f(t) = \alpha e^{\beta x}

Where :math:`\beta` is the growth coefficient and :math:`t` is the time index. The model in plate notation
is also shown below:

.. raw:: html

	<div style="width: 500pt; height: 298pt;"><svg width="674pt" height="298pt" viewBox="0.00 0.00 674.16 298.00" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" style="width: 100%; height: 100%;">
	<g id="graph0" class="graph" transform="scale(1 1) rotate(0) translate(4 294)">
	<title>%3</title>
	<polygon fill="white" stroke="transparent" points="-4,4 -4,-294 670.16,-294 670.16,4 -4,4"></polygon>
	<g id="clust1" class="cluster">
	<title>cluster21</title>
	<path fill="none" stroke="black" d="M20,-8C20,-8 190,-8 190,-8 196,-8 202,-14 202,-20 202,-20 202,-214 202,-214 202,-220 196,-226 190,-226 190,-226 20,-226 20,-226 14,-226 8,-220 8,-214 8,-214 8,-20 8,-20 8,-14 14,-8 20,-8"></path>
	<text text-anchor="middle" x="187" y="-14.8" font-family="Times,serif" font-size="14.00">21</text>
	</g>
	<!-- y -->
	<g id="node1" class="node">
	<title>y</title>
	<ellipse fill="lightgrey" stroke="black" cx="105" cy="-128" rx="88.64" ry="18"></ellipse>
	<text text-anchor="middle" x="105" y="-123.8" font-family="Times,serif" font-size="14.00">y ~ NegativeBinomial</text>
	</g>
	<!-- data_y -->
	<g id="node2" class="node">
	<title>data_y</title>
	<path fill="lightgrey" stroke="black" d="M140.32,-74C140.32,-74 69.68,-74 69.68,-74 63.68,-74 57.68,-68 57.68,-62 57.68,-62 57.68,-50 57.68,-50 57.68,-44 63.68,-38 69.68,-38 69.68,-38 140.32,-38 140.32,-38 146.32,-38 152.32,-44 152.32,-50 152.32,-50 152.32,-62 152.32,-62 152.32,-68 146.32,-74 140.32,-74"></path>
	<text text-anchor="middle" x="105" y="-51.8" font-family="Times,serif" font-size="14.00">data_y ~ Data</text>
	</g>
	<!-- y&#45;&gt;data_y -->
	<g id="edge1" class="edge">
	<title>y-&gt;data_y</title>
	<path fill="none" stroke="black" d="M105,-109.7C105,-101.98 105,-92.71 105,-84.11"></path>
	<polygon fill="black" stroke="black" points="108.5,-84.1 105,-74.1 101.5,-84.1 108.5,-84.1"></polygon>
	</g>
	<!-- data_x -->
	<g id="node3" class="node">
	<title>data_x</title>
	<path fill="lightgrey" stroke="black" d="M140.32,-218C140.32,-218 69.68,-218 69.68,-218 63.68,-218 57.68,-212 57.68,-206 57.68,-206 57.68,-194 57.68,-194 57.68,-188 63.68,-182 69.68,-182 69.68,-182 140.32,-182 140.32,-182 146.32,-182 152.32,-188 152.32,-194 152.32,-194 152.32,-206 152.32,-206 152.32,-212 146.32,-218 140.32,-218"></path>
	<text text-anchor="middle" x="105" y="-195.8" font-family="Times,serif" font-size="14.00">data_x ~ Data</text>
	</g>
	<!-- data_x&#45;&gt;y -->
	<g id="edge6" class="edge">
	<title>data_x-&gt;y</title>
	<path fill="none" stroke="black" d="M105,-181.7C105,-173.98 105,-164.71 105,-156.11"></path>
	<polygon fill="black" stroke="black" points="108.5,-156.1 105,-146.1 101.5,-156.1 108.5,-156.1"></polygon>
	</g>
	<!-- beta_mu -->
	<g id="node4" class="node">
	<title>beta_mu</title>
	<ellipse fill="none" stroke="black" cx="256" cy="-272" rx="76.56" ry="18"></ellipse>
	<text text-anchor="middle" x="256" y="-267.8" font-family="Times,serif" font-size="14.00">beta_mu ~ Normal</text>
	</g>
	<!-- beta -->
	<g id="node6" class="node">
	<title>beta</title>
	<ellipse fill="none" stroke="black" cx="271" cy="-200" rx="61.11" ry="18"></ellipse>
	<text text-anchor="middle" x="271" y="-195.8" font-family="Times,serif" font-size="14.00">beta ~ Normal</text>
	</g>
	<!-- beta_mu&#45;&gt;beta -->
	<g id="edge3" class="edge">
	<title>beta_mu-&gt;beta</title>
	<path fill="none" stroke="black" d="M259.71,-253.7C261.36,-245.98 263.35,-236.71 265.19,-228.11"></path>
	<polygon fill="black" stroke="black" points="268.66,-228.62 267.33,-218.1 261.82,-227.15 268.66,-228.62"></polygon>
	</g>
	<!-- alpha_mu -->
	<g id="node5" class="node">
	<title>alpha_mu</title>
	<ellipse fill="none" stroke="black" cx="432" cy="-272" rx="81.4" ry="18"></ellipse>
	<text text-anchor="middle" x="432" y="-267.8" font-family="Times,serif" font-size="14.00">alpha_mu ~ Normal</text>
	</g>
	<!-- alpha -->
	<g id="node7" class="node">
	<title>alpha</title>
	<ellipse fill="none" stroke="black" cx="416" cy="-200" rx="65.46" ry="18"></ellipse>
	<text text-anchor="middle" x="416" y="-195.8" font-family="Times,serif" font-size="14.00">alpha ~ Normal</text>
	</g>
	<!-- alpha_mu&#45;&gt;alpha -->
	<g id="edge2" class="edge">
	<title>alpha_mu-&gt;alpha</title>
	<path fill="none" stroke="black" d="M428.04,-253.7C426.28,-245.98 424.16,-236.71 422.2,-228.11"></path>
	<polygon fill="black" stroke="black" points="425.55,-227.07 419.91,-218.1 418.73,-228.63 425.55,-227.07"></polygon>
	</g>
	<!-- beta&#45;&gt;y -->
	<g id="edge4" class="edge">
	<title>beta-&gt;y</title>
	<path fill="none" stroke="black" d="M237.41,-184.83C212.58,-174.36 178.47,-159.98 151.09,-148.44"></path>
	<polygon fill="black" stroke="black" points="152.29,-145.14 141.72,-144.48 149.57,-151.59 152.29,-145.14"></polygon>
	</g>
	<!-- alpha&#45;&gt;y -->
	<g id="edge5" class="edge">
	<title>alpha-&gt;y</title>
	<path fill="none" stroke="black" d="M367.19,-187.92C358.47,-185.95 349.47,-183.91 341,-182 284.02,-169.14 219.28,-154.61 172.04,-144.02"></path>
	<polygon fill="black" stroke="black" points="172.76,-140.59 162.23,-141.82 171.23,-147.42 172.76,-140.59"></polygon>
	</g>
	<!-- sigma -->
	<g id="node8" class="node">
	<title>sigma</title>
	<ellipse fill="none" stroke="black" cx="583" cy="-200" rx="83.33" ry="18"></ellipse>
	<text text-anchor="middle" x="583" y="-195.8" font-family="Times,serif" font-size="14.00">sigma ~ HalfCauchy</text>
	</g>
	<!-- sigma&#45;&gt;y -->
	<g id="edge7" class="edge">
	<title>sigma-&gt;y</title>
	<path fill="none" stroke="black" d="M522.53,-187.55C511.71,-185.61 500.53,-183.69 490,-182 386.55,-165.43 266.95,-149.46 188.85,-139.46"></path>
	<polygon fill="black" stroke="black" points="188.95,-135.95 178.59,-138.15 188.07,-142.89 188.95,-135.95"></polygon>
	</g>
	</g>
	</svg></div>


Sampling the posterior of these models without doing reparametrization can be complicated due to the shape of it as
shown below:

.. image:: _static/br/posterior.png
  :width: 700

However, due to the lack of time, I'm still sampling this posterior. I use the MCMC Hamiltonian
Monte Carlo (`A Conceptual Introduction to Hamiltonian Monte Carlo <https://arxiv.org/pdf/1701.02434>`_) with
at least 4 chains (68k samples, including the tuning steps).

.. warning:: This model doesn't model the effect of interventions, at some point in time it will
             cease to be calibrated due to the effect of non-pharmaceutical interventions made
             by the government.

.. note:: This model uses data from the `official government website <https://covid.saude.gov.br/>`_.


**07/April** -- Death count analysis and forecast
-------------------------------------------------------------------------------
.. rubric:: Forecast from the model

.. image:: _static/br/br_deaths_07apr.png
  :width: 750

.. rubric:: Growth coefficient estimation

.. image:: _static/br/br_deaths_07apr_coeff.png
  :width: 750

.. rubric:: Sampling diagnostics

.. image:: _static/br/br_deaths_07apr_traceplot.png
  :width: 750

.. image:: _static/br/br_deaths_07apr_diag.png
  :width: 750


.. seealso:: This model uses the modelling approach described at :ref:`DeathCountModelling`.

State: Rio Grande do Sul (RS)
===============================================================================
These are focused analysis on the state of Rio Grande do Sul/Brazil.

**07/April** -- Mapping transmission through time
-------------------------------------------------------------------------------
This is a short animation showing the cities with reported infections in 
Rio Grande do Sul (RS)/Brazil for the date range of **March 10th** until
**April 6th**.

.. raw:: html

	<video controls width="740">
    <source src="_static/br/rsmap.mp4"
            type="video/mp4">
    	Sorry, your browser doesn't support embedded videos.
	</video>

.. note:: This animation used data from `Brasil.io <http://www.brasil.io/>`_, which is collected from
          the `TI Saude RS <http://ti.saude.rs.gov.br/covid19/>`_.