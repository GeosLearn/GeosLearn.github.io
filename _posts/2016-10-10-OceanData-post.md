---
title: Ocean data query
featured: images/pic1.jpg
layout: post
---

Access to quality data is essential to understand marine processes. Over the last 20 years, **Ocean Data portals** have emerged and are routinely used by Scientific organizations, Research agencies and the Industry to better understand the _complexity of the Ocean_ and its _interactions with Climate and Life_. These portals facilitate seamless access to marine data/services and promote the exchange and dissemination of marine data and services.

Ocean scientists routinely perform data _crunching_ to understand a particular system and need to **access and query** extensive lists of data.
Understanding how these data are stored, their origin and how to quickly retrieve particular information from them are what this module is all about!

<section>
  <header>
    <span class="byline"><font color = "#000000">Preamble</font></span>
  </header>
  <p>The information that is stored, processed, and exchanged, is at the heart of <strong>modern marine science</strong>. We will consider the Web's information systems that serve as entry points to information of all sorts. The most widespread examples of this kind of system are search engines like Google, which provides an index to billions of documents on the Web, and in a way allows us to think of the Web as a gigantic database. </p>

  <p>The Web's information systems, just like centralised data management systems, are mediators between individuals with little desire to trouble themselves with programming details, and physical objects like discs or USB keys. In this module, we will be looking at data systems that can <strong>manage information, understand it and make it available to marine scientists</strong>.</p>

  <header>
    <span class="byline"><font color = "#000000">Lecture resources</font></span>
  </header>
  <div class="col-md-6">
    <a href="http://earth.nullschool.net/about.html">earth</a> a visualization of global weather conditions forecast by supercomputers
        updated every three hours!
    <iframe id="weatherMap" style="width:100%; height:500px" src="https://earth.nullschool.net/#current/ocean/surface/currents/overlay=sea_surface_temp/orthographic=-226.48,-28.33,807"
    frameborder="0" scrolling="no" allowfullscreen></iframe>
  </div>
  <p>Wave height measures taken every day by a buoy offshore Sydney are <strong>data</strong>. A graph showing the evolution of the significant wave height over time, at a given place, is <strong>information</strong>. The fact that the number of extreme storms hitting Australian's coast increases as a result of climate change is <strong>knowledge</strong>. These three notions are very closely linked.
  <br/>
  <br/>
  Roughly speaking, here is how you should use them:
  <br/>
  - A piece of <strong>data</strong> provides a basic description, typically numerical for our purposes, of a given reality. <br/>
  - Drawing on the collected data, <strong>information</strong> is obtained by organising and structuring data so as to derive meaning.<br/>
  - By understanding the meaning of information, we obtain <strong>knowledge</strong>.<br/>
  </p>
  <div class="col-md-6">
  <iframe style="width:100%; height:400px" src="https://www.youtube.com/embed/7yTpv70gkGE?rel=0" frameborder="0" allowfullscreen></iframe>
  </div>
  <p>
  One of the great challenges for Ocean Data users is to understand where and how to find technologies that make it possible to evaluate, validate, verify, and rank information to help them in their jobs. This involves understanding how the ocean data providers are organised, the main standards, vocabularies and formats which are used by the community as well as the best approach for accessing and querying these information routinely.</p>
  <strong>Materials from the lecture:</strong>
  <table style="width:80%">
    <tr>
      <th><strong><a href="http://geoslearn.github.io/OceanData/#" target="_blank">HTML version</a></strong> (for Chrome or Safari)</th>
      <th><strong><a href="https://cloudstor.aarnet.edu.au/plus/index.php/s/FkfAC6DWiA6K5Xs" target="_blank">PDF version</a></strong></th>
    </tr>
  </table>
  <header>
    <span class="byline"><font color = "#000000">For the labs</font></span>
  </header>
  <p>
  We will use <strong><a href="http://jupyter.org" target="_blank">Jupyter</a></strong>,  a web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. To access the module materials we will download via Kitematic a  <strong><a href="https://www.docker.com/what-docker" target="_blank">Docker</a></strong> container called <strong>oceandata</strong>. Please follow the documentation provided <strong><a href="{{ site.prefix }}/LabDeploy.html">here</a></strong> on how to install the materials on your local computer or directly from the school computer labs.<br/>
  <br/>
  A series of examples based on <strong>ipython notebooks</strong> is proposed to give you an introduction to marine data querying. There are several advantages of using python as a general data analysis language and the notebook environment is a versatile tool that is designed to be intractive, user-friendly, open-source and sharable. While there are many libraries available to perform data analysis in Python, here's a few to get you started:
  <br/>
  + <strong><a href="www.numpy.org/" target="_blank">NumPy</a></strong>  is fundamental for scientific computing with Python. It supports large, multi-dimensional arrays and matrices and includes an assortment of high-level mathematical functions to operate on these arrays.<br/>
  + <strong><a href="http://www.sympygamma.com" target="_blank">SciPy</a></strong>  works with NumPy arrays and provides efficient routines for numerical integration and optimization.<br/>
  + <strong><a href="http://pandas.pydata.org" target="_blank">Pandas</a></strong>, also built on top of NumPy, offers data structures and operations for manipulating numerical tables and time series.<br/>
  + <strong><a href="www.numpy.org/" target="_blank">Matplotlib</a></strong> is a 2D plotting library that can generate such data visualizations as histograms, power spectra, bar charts, and scatterplots with just a few lines of code.<br/>
  + Built on NumPy, SciPy, and Matplotlib, <strong><a href="http://scikit-learn.org/stable/" target="_blank">Scikit-learn</a></strong> is a machine learning library that implements classification, regression, and clustering algorithms including support vector machines, logistic regression, naive Bayes, random forests, and gradient boosting. <br/>
  For a longer list of Python libraries useful for data science applications follow this <a href="https://github.com/rasbt/pattern_classification/blob/master/resources/python_data_libraries.md" target="_blank">link</a>.<br/>
  <br/>
  When the <strong>oceandata</strong> container has been installed via Kitematic and a volume has been attached to the container, you will be ready to start opening the ipython notebooks. The following notebooks are available:<br/>
  + Using <strong><a href="http://matplotlib.org/basemap" target="_blank">Basemap</a></strong> library to map Global Ocean Salinity from NASA via THREDDS data server. <br/>
  + Analysing off-shore sydney wave buoy data from Australian <strong><a href="http://www.imos.org.au" target="_blank">Integrated Marine Observing System</a></strong> (IMOS) and historical <strong><a href="http://polar.ncep.noaa.gov/waves/wavewatch/" target="_blank">NOAA WW3</a></strong> model predictions for different locations. <br/>
  + Extract Ocean Radar dataset for Turquoise Bay from <strong><a href="http://www.imos.org.au" target="_blank">IMOS</a></strong> and plot them on a map.<br/>
  + Access via THREDDS protocol NetCDF forecast prediction dataset for Chesapeake bay (US) from <strong><a href="http://fvcom.smast.umassd.edu/research_projects/NECOFS/model_system.html" target="_blank">FVCOM</a></strong> model, visualise it and extract relevant information. <br/>
  </p>
  <header>
    <span class="byline"><font color = "#000000">Examples of ocean data providers</font></span>
  </header>
  <p><strong><a href="https://portal.aodn.org.au" target="_blank">Australian marine and climate science data</a></strong></p>
  <div class="col-md-6">
    <iframe style="width:100%; height:500px" src="https://portal.aodn.org.au" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>  
  </div>
  <p><strong><a href="https://earthdata.nasa.gov/" target="_blank">Ocean data from NASA</a></strong></p>
  <div class="col-md-6">
    <iframe style="width:100%; height:480px" src="https://earthdata.nasa.gov/discipline/ocean" frameborder="0" scrolling="yes" allowfullscreen>
    </iframe>  
  </div>
</section>
