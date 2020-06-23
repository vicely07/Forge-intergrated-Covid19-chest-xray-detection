# Pega-intergrated-Covid19-chest-xray-detection
CovidScan.ai is developed to be a secured AI app intergrated with Pega platform with the purpose to assist radiologists with fast and accurate pneumonia dectection amid this COVID-19 pandemic. 

**Installation guide:**

1. Import Pega_Package.zip in Pega V8.2 environment and make sure below operators are imported

* ClinicOp
* MedOp

2. Make URL update in Meshup part of SA.html file.Change data-pega-url and script source as below



    <!-- ********************** Begin Pega content ********************** -->
  <script src ='http://localhost:8080/prweb/PRServlet?pyActivity=pzIncludeMashupScripts'></script>
  <div data-pega-gadgetname ='PegaGadget'
  data-pega-action ='createNewWork'
  data-pega-action-param-classname ='DMOrg-CT-Work-TreatCovid'
  data-pega-action-param-flowname ='pyStartCase'
  data-pega-isdeferloaded ='false'
  data-pega-applicationname ='CT'
  data-pega-threadname ='STANDARD'
  data-pega-resizetype ='stretch'
  data-pega-url ='http://localhost:8080/prweb/PRServlet' 
  data-pega-action-param-parameters ='{"pzSkinName":"CT","UserIdentifier":"MedOp","Password":"rules"}' ></div>

  <!-- ********************** End Pega content ********************** -->


#################################################################################

3. Deploy SA.html and CT.html on apache server.



