---
title: Badlands workshop
featured: images/pic4.jpg
layout: post
---

This workshop aims to introduce those interested in landscape evolution and source to sink problems to a new open-source code: **[Badlands](https://github.com/badlands-model/pyBadlands/wiki)**. Note that you do not have to be a seasoned modeller to participate.
Geomorphologists, tectonicists and sedimentologists interested in testing conceptual models based on field observations are welcome!

<section>
<p>
When you use Badlands, please cite the following papers and/or code release citable <b>DOI</b>:<br/>
- <b>Salles, T. & Hardiman, L.</b>: Badlands: An open-source, flexible and parallel framework to study landscape dynamics, Computers & Geosciences, 91, 77-89, <strong><a href="http://dx.doi.org/10.1016/j.cageo.2016.03.011" target="_blank">doi:10.1016/j.cageo.2016.03.011</a></strong>, 2016.<br/>
- <b>Salles, T.</b>: Badlands: A parallel basin and landscape dynamics model, SoftwareX, <strong><a href="http://dx.doi.org/10.1016/j.softx.2016.08.005" target="_blank">doi:10.1016/j.softx.2016.08.005</a></strong>, 2016.<br/>
- <b>Salles, T. & Howson, I.</b>: Release 1: badlands-model/pyBadlands, Zenodo, <strong><a href="http://doi.org/10.5281/zenodo.160412" target="_blank">doi:10.5281/zenodo.160412</a></strong>, 2016.
</p>
  <header>
    <span class="byline"><font color = "#000000">Background on Badlands</font></span>
  </header>

  <p>The model's development started in 2015 and is part of the suite of tools from the <strong><a href="http://www.geosci.usyd.edu.au/research/re_hub.shtml" target="_blank">ARC Basin Genesis Hub</a></strong>. <strong>Basin and Landscape Dynamics</strong> (a.k.a <strong><a href="https://github.com/badlands-model/pyBadlands/wiki" target="_blank">Badlands</a></strong>) is a landscape evolution model, built to simulate topography development at various space and time scales.<br/>
  <br/>

  The model is capable of simulating hillslope processes (<strong>linear</strong> & <strong>non-linear</strong> diffusion), fluvial incision (<i>modified</i> <strong>Stream Power Law</strong>, <strong>Transport Capacity Law</strong> both for sediment erosion/transport/deposition), spatially and temporally varying geodynamic (horizontal + vertical displacements) and climatic forces which can be used to simulate changes in base level, as well as effects of climate changes or sea-level fluctuations. The model uses <strong><a href="https://github.com/awickert/gFlex" target="_blank">gFlex</a></strong> package which is designed to solve elastic plate flexure for applications to Earth's lithosphere.
  </p>

  <p>
  The model is designed around the following features:<br/><br/>
  + The finite volume approach from <strong><a href="http://www.sciencedirect.com/science/article/pii/S0098300400001345" target="_blank">Tucker et al. (2001)</a></strong>   based on the dual Delaunay-Voronoi framework is used to solve the continuity equation explicitly,<br/>
  + Node ordering is perform efficiently based on the work from <strong><a href="http://www.sciencedirect.com/science/article/pii/S0169555X12004618" target="_blank">Braun & Willett (2013)</a></strong>, <br/>
  + 3D surface deformations using the node refinement technique proposed by <strong><a href="http://onlinelibrary.wiley.com/doi/10.1002/2014GC005490/abstract;jsessionid=48A885F79A40B1E3E76AFC1BEAA2B238.f03t03" target="_blank">Thieulot et al. ( 2014)</a></strong>, <br/>
  + Orographic precipitation using <strong><a href="http://journals.ametsoc.org/doi/abs/10.1175/1520-0469(2004)061%3C1377%3AALTOOP%3E2.0.CO%3B2" target="_blank">Smith & Barstad (2004)</a></strong> linear model to compute topographic induced rain field, <br/>
  + Varying erodibility layers (both horizontally and vertically) to simulate impact of changing sediment characteristics on landscape evolution, <br/>
  + A set of functions for pre & post-processing of Badlands inputs and outputs is available in a <strong><a href="https://github.com/badlands-model/pyBadlands-Companion" target="_blank">GitHub Companion repository</a></strong>.
  </p>
</section>

<section>
  <header>
    <span class="byline"><font color = "#000000">Community driven</font></span>
  </header>
  <p>This program is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.<br/>
  This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
  <br/>
  You should have received a copy of the GNU Lesser General Public License along with this program. If not, see <strong><a href="http://www.gnu.org/licenses/lgpl-3.0.en.html" target="_blank">http://www.gnu.org/licenses/lgpl-3.0.en.html</a></strong>.</p>
</section>

<section>
  <header>
    <span class="byline"><font color = "#000000">Requirements</font></span>
  </header>
  <p>You will need to download the <strong><a href="http://www.docker.com/products/overview" target="_blank">Docker application</a></strong>
    by clicking on the link and choosing the right one for your operating system.
  </p>
  <div style="text-align: center;">
    <img src="{{ site.prefix }}/assets/images/docker.png" alt="download the Docker app" style="width:100%; height:100%" align="middle">
  </div>
  <p> You will also need  <strong><a href="http://www.paraview.org/download/" target="_blank">Paraview</a></strong> data analysis and visualization application.
  </p>
  <!-- <div class="col-md-6">
    <iframe style="width:100%; height:480px" src="http://www.paraview.org/" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>
  </div> -->
</section>

<section>
  <header>
    <span class="byline"><font color = "#000000">Resources</font></span>
  </header>
  <p>We will use <strong><a href="http://jupyter.org" target="_blank">Jupyter</a></strong>,  a web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. To access the workshop materials we will download via Kitematic a  <strong><a href="https://www.docker.com/what-docker" target="_blank">Docker</a></strong> container called <strong><a href="https://hub.docker.com/r/badlandsmodel/pybadlands-demo/" target="_blank">pybadlands-demo</a></strong>. Please follow the documentation provided <strong><a href="{{ site.prefix }}/LabDeploy.html">here</a></strong> on how to install the materials on your local computer or directly from the School's computer labs.<br/>
  </p>

  <p>
    Some notes on how to use <b>Badlands</b> via <b>Docker</b>, setup initial models and run examples is available through the following links:</p>
    <table style="width:80%">
      <tr>
        <th><strong><a href="http://geoslearn.github.io/BadlandsWorkshop/#" target="_blank">HTML version</a></strong> (for Chrome or Safari)</th>
        <th><strong><a href="https://cloudstor.aarnet.edu.au/plus/index.php/s/ZAVmdaaupVKuZHA" target="_blank">PDF version</a></strong></th>
      </tr>
    </table>
    <p>
    For pre- & post-processing it is also recommended to use the <strong><a href="https://github.com/badlands-model/pyBadlands-Companion
" target="_blank">Companion</a></strong> which is already shipped in the Docker container.<br/>
Most of the information regarding how to use the tool are provided in <strong><a href="https://github.com/badlands-model/pyBadlands/wiki" target="_blank"> Badlands wiki</a></strong>.
</p>

<p>
<strong><a href="https://github.com/badlands-model/pyBadlands/wiki/XML-input" target="_blank">Complete input file options</a></strong></p>

<p>
<strong><a href="https://github.com/badlands-model/pyBadlands/wiki/PreProcessing" target="_blank">Pre-processing options</a></strong></p>

<p>
<strong><a href="https://github.com/badlands-model/pyBadlands/wiki/PostProcessing" target="_blank">Post-processing options</a></strong></p>


</section>


<section>
  <header>
    <span class="byline"><font color = "#000000">Hands-on examples</font></span>
  </header>
  <p>
  A compilation of notebooks with examples are available for the workshop:<br/>
  + delta evolution under sea-level fluctuation
  <strong><a href="http://nbviewer.jupyter.org/github/badlands-model/pyBadlands/blob/master/Examples/delta/delta.ipynb" target="_blank">nbviewer</a></strong><br/>
  + impact of climate on mountain dynamic
  <strong><a href="http://nbviewer.jupyter.org/github/badlands-model/pyBadlands/blob/master/Examples/mountain/mountain.ipynb" target="_blank">nbviewer</a></strong><br/>
  + basin filling associated to a strike-slip fault system
  <strong><a href="http://nbviewer.jupyter.org/github/badlands-model/pyBadlands/blob/master/Examples/strikeslip/strike-slip.ipynb" target="_blank">nbviewer</a></strong> <br/>
  + infilling of a crater-type topography
  <strong><a href="http://nbviewer.jupyter.org/github/badlands-model/pyBadlands/blob/master/Examples/crater/crater.ipynb" target="_blank">nbviewer</a></strong> <br/>
  + flexural response due to loading and unloading under variable elastic thickness <strong><a href="http://nbviewer.jupyter.org/github/badlands-model/pyBadlands/blob/master/Examples/flexure/flexure.ipynb" target="_blank">nbviewer</a></strong> <br/>
  + quick setup of real topography/bathymetry model using etopo1
  <strong><a href="http://nbviewer.jupyter.org/github/badlands-model/pyBadlands/blob/master/Examples/etopo/etopo.ipynb" target="_blank">nbviewer</a></strong>
  </p>
  <div style="text-align: center;">
    <img src="{{ site.prefix }}/assets/images/example.png" alt="series of examples" style="width:90%; height:100%" align="middle">
  </div>
</section>

<section>
  <header>
    <span class="byline"><font color = "#000000">Some questions?</font></span>
  </header>
  <p>If you come across a bug or if you need some help compiling or using the code you can: <br/><br/>
  + go through our mailing list <strong><a href="http://mailman.sydney.edu.au/pipermail/badlands/" target="_blank">archive</a></strong>.<br/>
  + subscribe to our <strong><a href="http://mailman.sydney.edu.au/mailman/listinfo/badlands" target="_blank">mailing list</a></strong>.<br/>
  + or <strong><a href="mailto:badlands@mailman.sydney.edu.au" target="_blank">drop us a line</a></strong>.
</p>
</section>
