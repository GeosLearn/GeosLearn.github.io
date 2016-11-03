---
title: Coastal evolution modeling
featured: images/pic2.png
layout: post
---

<head>
   <link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.5/leaflet.css" />
   <script src="http://cdn.leafletjs.com/leaflet-0.5/leaflet.js"></script>
</head>

In this module, we will build upon the theory that were developed during the first parts of your UoS using simple numerical models. In particular we will look at medium to long-term coastal process evolution models. The aim is to give you some understanding on how to set up and use numerical models for coastal projects as well as elaborate on the differences between these models.

**Landsat satellites images of the Nauset-Monomoy barrier beach system between from 1984 to 2013 (USGS-NASA).**
<div class="col-md-6">
  <iframe style="width:100%; height:350px" src="/assets/images/coasts.mp4" frameborder="0" scrolling="yes" allowfullscreen>
  </iframe>  
</div>

As an example, we will simulate the impact of storms on 2D beach profiles, explore the sensitivities of crenulated bay to different wave conditions and use models of longshore transport.

<section>
  <header>
    <span class="byline"><font color = "#000000">Preamble</font></span>
  </header>
  <p>Our understanding of coastal evolution is often based on <strong>physical</strong> and <strong>numerical</strong> hydrodynamic models which are used to simulate the main processes taking place in coastal regions.
  <br/>
  <strong>Physical models</strong> refer to the use of laboratory models at an appropriate scale ( micro, small, medium and large scale models) for investigating the relevant process.
  <br/>
  <strong>Numerical models</strong> refer to the use of computer codes (commercial, open source, home-made software).
  <br/>
  <br/>
  Hydrodynamic modeling forms the basis for many other modeling studies, whether sediment transport, morphology, waves, water quality and/or ecological changes are being investigated.
  In this module, a general overview is given and describes some examples of physical and numerical modeling approach used to study coastal processes.
  </p>
  <header>
    <span class="byline"><font color = "#000000">Lecture resources</font></span>
    <h1><font color = "#000000"><strong>Physical Models</strong></font></h1>
  </header>
  <div class="col-md-6">
    <iframe style="width:100%; height:400px" src="https://www.youtube.com/embed/IOkgGIWNixk?rel=0" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>  
  </div>
  <p>Physical models and laboratory experiments remain part and parcel of the research methodology because of their many strong points, such as:
  <br/>
  + <strong>Observability</strong>: experiments to investigate mechanisms that are difficult to observe in nature,<br/>
  + <strong>Measurability</strong>: experiments to isolate phenomena that are difficult to measure in nature,<br/>
  + <strong>Repeatability</strong>: repeated experiments, to investigate the range of inherent uncertainty of phenomena,<br/>
  + <strong>Input control</strong>: experiments with various realistic input time series, to assess the predictive capability of numerical models,<br/>
  + <strong>Process control</strong>: experiments for simple situations, in order to validate the results of theoretical behaviour analyses,<br/>
  + <strong>Robustness</strong>: modeling of processes that cannot be modelled numerically, because (unlike numerical models) physical models are basically similar to prototype (especially in facilities that model processes at full scale).
  </p>
  <div class="col-md-6">
    <iframe style="width:100%; height:400px" src="https://www.youtube.com/embed/RvtBMojxWUQ?rel=0" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>  
  </div>
  <p>
  Facilities of various sizes (from large to micro scale) are available for physical modeling of coastal processes. The size of the facility for use depends on the scale and scope of the phenomenon to be modelled.
  </p>
  <strong>Materials for physical modeling:</strong>
  <table style="width:80%">
    <tr>
      <th><strong><a href="http://geoslearn.github.io/physicalModel/#" target="_blank">HTML version</a></strong> (for Chrome or Safari)</th>
      <th><strong><a href="https://cloudstor.aarnet.edu.au/plus/index.php/s/KEz6Kt72sxvZNzc" target="_blank">PDF version</a></strong></th>
    </tr>
  </table>

  <header>
    <h1><font color = "#000000"><strong>Numerical Models</strong></font></h1>
  </header>
  <p>
  The rapid development of computing technology has furnished a large number of models to be employed in coastal hydrodynamic problems.
  <br/>
  The numerical technique can be based on the finite element method, finite difference method, boundary element method, finite volume method and Eulerian-Lagrangian method. The time-stepping algorithm can be implicit, semi-implicit, explicit, or characteristic-based.
  <br/>
  The modeling can be simplified into different spatial dimensions, i.e., a one-dimensional (1D) model, two-dimensional (2D) depth-integrated model, 2D lateral-integrated model, 2D layered model and 3D model.
  </p>
  <div class="col-md-6">
    <iframe style="width:100%; height:400px" src="https://www.youtube.com/embed/CCmTY0PKGDs?rel=0" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>  
  </div>
  <p>
  An analysis of coastal hydraulics and water quality often demands the application of heuristics and empirical experience, and is accomplished through some simplifications and modeling techniques according to the experience of specialists. However, the accuracy of the prediction is to a great extent dependent on open boundary conditions, model parameters, and the numerical scheme. The adoption of a proper numerical model for a practical coastal problem is a highly specialized task. These predictive tools inevitably involve certain assumptions and/or limitations, and need to be applied with caution by experienced scientists who possess a comprehensive understanding of the problem domain.
  </p>
  <strong>Materials for numerical modeling:</strong>
  <table style="width:80%">
    <tr>
      <th><strong><a href="http://geoslearn.github.io/numericalModel/#" target="_blank">HTML version</a></strong> (for Chrome or Safari)</th>
      <th><strong><a href="https://cloudstor.aarnet.edu.au/plus/index.php/s/pefBV4Xx3pEU2QD" target="_blank">PDF version</a></strong></th>
    </tr>
  </table>

  <header>
    <span class="byline"><font color = "#000000">For the labs</font></span>
  </header>
  <p>We will use <strong><a href="http://jupyter.org" target="_blank">Jupyter</a></strong>,  a web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. To access the module materials we will download via Kitematic a  <strong><a href="https://www.docker.com/what-docker" target="_blank">Docker</a></strong> container called <strong>coastevol</strong>. Please follow the documentation provided <strong><a href="{{ site.prefix }}/LabDeploy.html">here</a></strong> on how to install the materials on your local computer or directly from the school computer labs.<br/>
  When the <strong>coastevol</strong> container has been installed via Kitematic and a volume has been attached to the container, you will be ready to start opening the ipython notebooks.
  The labs will focus on 2 different numerical models. <br/>
  <br/>
  <strong>One-line model</strong><br/>
  First we will look at the <strong><a href="https://cove-model.github.io/Website/" target="_blank">COastal Vector Evolution</a></strong> model (COVE) - a vector-based one-line coastal evolution model presented and used in a <strong><a href="http://onlinelibrary.wiley.com/doi/10.1002/2015JF003704/abstract" target="_blank">paper</a></strong> by Hurst et al. (2015). <br/>
  The model's highlights include:<br/>
  + Application at spatial scales of kms to tens of kms, over decadal to millennial timescales.<br/>
  + Coastal change is driven by gradients in wave-generated alongshore sediment transport. <br/>
  + Alongshore sediment transport driven by the height and angle of breaking waves.<br/>
  + Retreat of cliffs governed by beach interaction (protection vs tools).</p>  
<div class="col-md-6" id="map" style="width:100%; height:400px"></div>
<script>
  var map = L.map('map').setView([37.4848, -122.459], 13);
  L.tileLayer('http://{s}.tile.stamen.com/terrain/{z}/{x}/{y}.jpg', {
        maxZoom: 18,
        attribution: 'Map tiles by <a href="http://stamen.com">Stamen Design</a>, under <a href="http://creativecommons.org/licenses/by/3.0">CC BY 3.0</a>. Data by <a href="http://openstreetmap.org">OpenStreetMap</a>, under <a href="http://creativecommons.org/licenses/by-sa/3.0">CC BY SA</a>.'
    }).addTo(map);
    var marker_1 = L.marker([37.462777, -122.47788]);
    marker_1.bindPopup("Crenulate bay example: Half Moon Bay (CA)");
    map.addLayer(marker_1)
</script>
  <p>  <br/> Following the ideas proposed in Hurst et al. (2015), you will investigate the evolution of crenulate bays and explore coastal behavior and sensitivity under different climatic conditions.<br/>
  <br/>
  <strong>Nearshore wave propagation model</strong><br/>
  Then we will use <strong><a href="http://oss.deltares.nl/web/xbeach/" target="_blank">XBeach</a></strong> model.
  XBeach solves coupled 2D horizontal equations for wave propagation, flow, sediment transport and bottom changes, for varying (spectral) wave and flow boundary conditions. It is a public-domain model that has been developed with major funding from the US Army Corps of Engineers, Rijkswaterstaat and the EU, supported by a consortium of UNESCO-IHE, Deltares, Delft University of Technology and the University of Miami. <br/>
   XBeach can be used as stand-alone model for small-scale (project-scale) coastal applications, but could also be integrated within more complex coupling frameworks. For example, it could be driven by boundary conditions provided by wind, wave or surge models and its main outputs (time-varying bathymetry and possibly discharges over breached barrier island sections) could be then transferred back.  <br/>
   </p>
   <div class="col-md-6">
     <iframe style="width:100%; height:400px" src="https://www.youtube.com/embed/UgK2OfaNqfM?rel=0" frameborder="0" scrolling="yes" allowfullscreen>
     </iframe>  
   </div>
   <p>
   Because the model takes into account the variation in wave height in time (long known to surfers) it resolves the special long wave motions created by this variation. This so-called <strong>surf beat</strong> is responsible for most of the swash waves that actually hit the dune front or overtop it. <br/> Using this functionality we will explore 2D profiles evolution and XBeach outputs for different initial conditions.
  </p>
  <header>
    <span class="byline"><font color = "#000000">Coastal models repository</font></span>
  </header>
  <p><strong>- <a href="https://csdms.colorado.edu/wiki/Main_Page" target="_blank">Community Surface Dynamics Modeling System</a></strong> (CSDMS)</p>
  <p><strong>- <a href="http://www.coastalhazards.org" target="_blank">Coastal Hazards Research Collaboratory</a></strong> (CHARCOL)</p>
  <div class="col-md-6">
    <iframe style="width:100%; height:500px" src="https://csdms.colorado.edu/wiki/Main_Page" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>  
  </div>
  <br/>
  <div class="col-md-6">
    <iframe style="width:100%; height:500px" src="http://www.coastalhazards.org/index.html" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>  
  </div>
</section>
