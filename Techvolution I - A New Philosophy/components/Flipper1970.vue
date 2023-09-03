<!-- 
resources used to get this nice carousel.
https://glidejs.com/docs/setup/
https://stackoverflow.com/questions/69457943/is-it-possible-to-use-glidejs-inside-a-vue-component
https://stackblitz.com/edit/vue3-glidejs?file=src%2Fcomponents%2FCarousel.vue
-->

<!-- 
 Internet Age, 1970
 This is a carousel to display several factoids about how many societal problems started in 1969, because we entered a new age, but didn't evolve into new (technological) species.
  -->

  <template>
   <div>
     <div class="glide">
       <div class="glide__track" data-glide-el="track">
         <ul class="glide__slides">
           <li class="glide__slide">
             <img src="/assets/problem-solving-philosophy.png">
             <i>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</i>
           </li>
           <li class="glide__slide">
             <img src="https://lp-cms-production.imgix.net/2020-11/GettyRF_598163608.jpg?auto=format&fit=crop&sharp=10&vib=20&ixlib=react-8.6.4&w=850&q=20&dpr=5">
             <i>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</i>
           </li>
           <li class="glide__slide">
             <img src="https://coastalcroatia.com/wp-content/uploads/2017/07/makarska-e1527695960897.jpg">
             <i>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</i>
           </li>
         </ul>
       </div>
       <div class="glide__arrows" data-glide-el="controls">
         <button class="glide__arrow glide__arrow--left; button-flipper" data-glide-dir="<" style="margin-right: 10px">Prev</button>
         <button class="glide__arrow glide__arrow--right; button-flipper" data-glide-dir=">">Next</button>
       </div>
     </div>
   </div>
   In the game of chutes and ladders, we thus keep hitting chute.
 </template>
 
 <script>
 import Glide from '@glidejs/glide'
 
 export default {
   mounted() {
     new Glide('.glide').mount()
   },
 }
 </script>
 
 <style scoped>
 @import '@glidejs/glide/dist/css/glide.core.min.css';
 </style>
 
 <!-- 
  sources
  https://tradingeconomics.com/
  https://www.pewresearch.org 
  https://ourworldindata.org/


  ===

  Useable and coded slides.


  INTERNET AGE TECHNOLOGY
  We love using this stuff.

  <li class="glide__slide">
    <b>Share of people using the internet</b>
    <iframe src="https://ourworldindata.org/grapher/share-of-individuals-using-the-internet" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
    <i>Share of people using the internet.<a href="https://ourworldindata.org/grapher/share-of-individuals-using-the-internets">Our World in Data.</a></i>
  </li>

<li class="glide__slide">
    <b>Historical cost of computer memory and storage</b>
    <iframe src="https://ourworldindata.org/grapher/historical-cost-of-computer-memory-and-storage" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
    <i>Historical cost of computer memory and storage.<a href="https://ourworldindata.org/grapher/historical-cost-of-computer-memory-and-storage">Our World in Data.</a></i>
</li>

<li class="glide__slide">
    <b>Moore's law: The number of transistors per microprocessor</b>
    <iframe src="https://ourworldindata.org/grapher/transistors-per-microprocessor" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
    <i>Moore's law: The number of transistors per microprocessor.<a href="https://ourworldindata.org/grapher/historical-cost-of-computer-memory-and-storage">Our World in Data.</a></i>
</li>

<li class="glide__slide">
    <b>Adoption of communication technologies, World</b>
    <iframe src="https://ourworldindata.org/grapher/ict-adoption" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
    <i>Adoption of communication technologies, World.<a href="https://ourworldindata.org/grapher/ict-adoption">Our World in Data.</a></i>
</li>


<li class="glide__slide">
    <b>Literate and illiterate world population, World</b>
    <iframe src="https://ourworldindata.org/grapher/literate-and-illiterate-world-population" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
    <i>Literate and illiterate world population, World.<a href="https://ourworldindata.org/grapher/literate-and-illiterate-world-population">Our World in Data.</a></i>
  </li>

  
  POLITICS
  Why is amazing new tech dividing us?

  <li class="glide__slide">
    <b>Public Trust in Government: 1958-2022</b>
    <img src="\img\flipper1970\chart-20081038.png">
    <i>Since the 1970s, trust in government has been consistently higher among members of the party that controls the White House than among the opposition party.  <a href="https://www.pewresearch.org/politics/2022/06/06/public-trust-in-government-1958-2022/">Pew Research</a></i>
  </li>
  
  <li class="glide__slide">
    <b>The Rise of Partisanship</b>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/tEczkhfLwqM?si=ux1aJDdLnOscdmT6" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    <i>The Rise of Partisanship and Super-Cooperators in the U.S. House of Representatives.<a href="https://journals.plos.org/plosone/article/figure?id=10.1371/journal.pone.0123507">Plos One</a></i>
  </li>


 ECONOMICS
 Where are the gains?

  <li class="glide__slide">
    <b>United States Imports</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=tbimtot&v=202308081251V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/imports'>tradingeconomics.com</a>
    <i>United States Imports.<a href="https://tradingeconomics.com/united-states/imports">Trading Economics</a></i>
  </li>

  <li class="glide__slide">
    <b>United States Exports</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=tbextot&v=202308301329V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/exports'>tradingeconomics.com</a>
    <i>United States Exports.<a href="https://tradingeconomics.com/united-states/exports">Trading Economics</a></i>
  </li>

  <li class="glide__slide">
    <b>United States Balance of Trade.</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=ustbtot&v=202308121125V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/balance-of-trade'>tradingeconomics.com</a>
    <i>United States Balance of Trade.<a href="https://tradingeconomics.com/united-states/balance-of-trade">Trading Economics</a></i>
  </li>


 LIVING COST
 People are using new tech but not harvesting more resources

  <li class="glide__slide">
    <b>Annual Vehicle Miles Traveled in the United States</b>
     <iframe style="width: 900px; height: 667.062px;" src="https://afdc.energy.gov/data/widgets/10315" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>
    <i>Increase in the vehicle miles travelled.<a href="https://afdc.energy.gov/data/10315">U.S. Dept. of Energy.</a></i>
  </li>



  <li class="glide__slide">
    <b>United States Nonfarm Labour Productivity</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=unitedstapro&v=202308040644V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/productivity'>tradingeconomics.com</a>
    <i>United States Nonfarm Labour Productivity.<a href="https://tradingeconomics.com/united-states/productivity">Trading Economics.</a></i>
  </li>
  
  <li class="glide__slide">
    <b>United States Nonfarm Labour Productivity</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=unitedstawaggro&v=202309021143V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600' frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/wage-growth'>tradingeconomics.com</a>
  </li>

  <li class="glide__slide">
    <b>United States Total Vehicle Sales</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=unitedstatotvehsal&v=202309021120V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/total-vehicle-sales'>tradingeconomics.com</a>
    <i>United States Total Vehicle Sales.<a href="https://tradingeconomics.com/united-states/total-vehicle-sales">Trading Economics</a></i>
  </li>

<li class="glide__slide">
  <b>United States Personal Savings Rate</b>
  <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=unitedstapersav&v=202309021014V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/personal-savings'>tradingeconomics.com</a>
</li>

  <li class="glide__slide">
    <b>United States Balance of Trade</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=ustbtot&v=202308121125V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/balance-of-trade'>tradingeconomics.com</a>
  </li>

  <li class="glide__slide">
    <b>Canada Households Credit Market Debt to Disposable Income</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=canadahdti&v=202307131624V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/canada/households-debt-to-income'>tradingeconomics.com</a>
  </li>

  <li class="glide__slide">
    <b>Obesity in adults, 1975 to 2016</b>
 <iframe src="https://ourworldindata.org/grapher/share-of-adults-defined-as-obese?tab=chart&country=~USA" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
  <i>United States Balance of Trade.<a href="https://tradingeconomics.com/united-states/balance-of-trade">Our World in Data.</a></i>
  </li>

  <li class="glide__slide">
  <b>Marriages per 1,000 people</b>
    <iframe src="https://ourworldindata.org/grapher/marriage-rate-per-1000-inhabitants?time=earliest..2018&country=~USA" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
  <i>Marriages per 1,000 people.<a href="https://ourworldindata.org/grapher/marriage-rate-per-1000-inhabitants?time=earliest..2018&country=~USA">Our World in Data.</a></i></li>

  <li class="glide__slide">
  <b>The Productivity–Pay Gap</b>
    <iframe width="100%" height="460" src="https://www.epi.org?p=235212&view=embed&embed_template=charts_v2013_08_21&embed_date=20230828&onp=91701&utm_source=epi_press&utm_medium=chart_embed&utm_campaign=charts_v2" frameborder="0"></iframe>
  <i>The Productivity–Pay Gap.<a href="https://www.epi.org/productivity-pay-gap/">Our World in Data.</a></i></li>
  



    <li class="glide__slide">
  <b>U.S. House Prices Are Rising Exponentially Faster Than Income</b>
     <div class="infogram-embed" data-id="11fe5b89-1261-4031-aa72-6ff6b87b0435" data-type="interactive" data-title="1965 to 2021"></div><script>!function(e,n,i,s){var d="InfogramEmbeds";var o=e.getElementsByTagName(n)[0];if(window[d]&&window[d].initialized)window[d].process&&window[d].process();else if(!e.getElementById(i)){var r=e.createElement(n);r.async=1,r.id=i,r.src=s,o.parentNode.insertBefore(r,o)}}(document,"script","infogram-async","https://infogram.com/js/dist/embed-loader-min.js");</script>
  <i>U.S. House Prices Are Rising Exponentially Faster Than Income.<a href="https://www.realestatewitch.com/house-price-to-income-ratio-2021/">Our World in Data.</a></i></li>


  PROCREATION
  Like any species, because we're not harvesting more resources, we aren't procreating

  <li class="glide__slide">
  <b>Fertility rate: children per woman</b>
   <iframe src="https://ourworldindata.org/grapher/children-per-woman-UN?tab=chart&country=~USA" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
  <i>Fertility rate: children per woman.<a href="https://ourworldindata.org/grapher/children-per-woman-un?tab=chart&country=~USA">Our World in Data.</a></i></li>

  <li class="glide__slide">
    <b>Changing profile of stay-at-home parents</b>
    <img src="\img\flipper1970\c-g01-eng.png">
    <i>Increase in the vehicle miles travelled.<a href="https://www150.statcan.gc.ca/n1/pub/11-630-x/11-630-x2016007-eng.htm">Statscan.</a></i>
  </li>


  RED TAPE
  How new technology is being (mis)used.

  <li class="glide__slide">
    <b>United States Doctors</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=usphys&v=202304061134V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/medical-doctors'>tradingeconomics.com</a>
  </li>
  
  <li class="glide__slide">
    <b>United States Nurses</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=usnurs&v=202304061134V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/nurses'>tradingeconomics.com</a>
  </li>

  <li class="glide__slide">
    <b>United States Hospital Beds</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=usbeds&v=202304061134V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/hospital-beds'>tradingeconomics.com</a>
  </li>

  <li class="glide__slide">
    <b>US Healthcare Expenditure</b>
    <iframe src="https://ourworldindata.org/grapher/us-healthcare-expenditure" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
    <i>United States Total Vehicle Sales.<a href="https://ourworldindata.org/financing-healthcare">Our World in Data.</a></i>
  </li>

  <li class="glide__slide">
    <b>US Healthcare Expenditure</b>
    <https://www.sentencingproject.org/reports/mass-incarceration-trends/>
    <i>United States Total Vehicle Sales.<a href="https://ourworldindata.org/financing-healthcare">Our World in Data.</a></i>
  </li>

 <li class="glide__slide">
    <b>U.S. State and Federal Prison Population, 1925-2021</b>
    <img src="\img\flipper1970\figure-1-1-950x624.png">
    <i>U.S. State and Federal Prison Population, 1925-2021.<a href="https://www.sentencingproject.org/reports/mass-incarceration-trends/">Sentencing Project.</a></i>
  </li>
  

  ENVIRONTMENTAL
  Hyper industrialization is eating the environment all species are supposed to harvest resources from

 <li class="glide__slide">
    <b> Trends in Global Emissions</b>
    <img src="\img\flipper1970\fossil_fuels_1.png">
    <i>Trends in Global Emissions.<a href="https://www.epa.gov/ghgemissions/global-greenhouse-gas-emissions-data#:~:text=Global%20carbon%20emissions%20from%20fossil,increase%20from%201970%20to%202011.">U.S. Dept. of Energy.</a></i>
  </li>

  <li class="glide__slide">
    <b>World CO2 Emissionss</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=wld.en.atm.co2e.kt&v=202304061134V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/world/co2-emissions'>tradingeconomics.com</a>
  </li>

  <li class="glide__slide">
    <b>United States Average Temperature</b>
    <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=usatemp&v=202304061134V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/temperature'>tradingeconomics.com</a>
  </li>
 

  <li class="glide__slide">
    <b>Living Planet Index</b>
     <iframe src="https://ourworldindata.org/grapher/global-living-planet-index" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>
     <i>Living Planet Index.<a href="https://ourworldindata.org/grapher/global-living-planet-index">Our World in Data.</a></i>
  </li>


  DEBT
  So inefficient today that we must keep borrowing from tomorrow.

 <li class="glide__slide">
    <b>National debt of the United States</b>
    <img src="\img\flipper1970\Debt_to_GDP.webp.png">
    <i>National debt of the United States.<a href="https://en.wikipedia.org/wiki/National_debt_of_the_United_States.">Wikipedia.</a></i>
  </li>

  <li class="glide__slide">
    <b>United States Gross Federal Debt to GDP</b>
      <iframe src='https://d3fy651gv2fhd3.cloudfront.net/embed/?s=usadebt2gdp&projection=te&v=202304061134V20230410&w=850&h=400&d1=19230927&h=300&w=600' height='300' width='600'  frameborder='0' scrolling='no'></iframe><br />source: <a href='https://tradingeconomics.com/united-states/government-debt-to-gdp'>tradingeconomics.com</a>
    <i>Increase in the vehicle miles travelled.<a href="https://tradingeconomics.com/united-states/government-debt-to-gdp">Trading Economics.</a></i>
  </li>

  <li class="glide__slide">
    <b>Consumer Debt</b>
    <img src="\img\flipper1970\Personal_savings_rate_&_revolving_credit.webp.png">
    <i>Personal Savings Rate and Revolving Credit.<a href="https://en.wikipedia.org/wiki/Consumer_debt#.">Wikipedia.</a></i>
    <i>A Brief History of Consumer Culture.<a href="https://thereader.mitpress.mit.edu/a-brief-history-of-consumer-culture/.">MIT.</a></i>
  </li>

  <li class="glide__slide">
    <b>Consumer and Government Debt as a % of GDP</b>
    <img src="\img\flipper1970\Consumer_and_Government_Debt_as_a_%_of_GDP.png">
    <i>Consumer and Government Debt as a % of GDP.<a href="https://en.wikipedia.org/wiki/File:Consumer_and_Government_Debt_as_a_%25_of_GDP.png">Wikipedia.</a></i>
  </li>



  ==================================================


  

  Various data points. Not fully anaylzed for useability.
  
  Graphs/Datapoints:
  - Vehicle Miles Travelled
    - total VMT <https://afdc.energy.gov/data/10315>
  
    - Carbon Emissions
      Trends in Global Emissions <>
  
  
  - Government Debt
   - National debt of the United States <https://en.wikipedia.org/wiki/National_debt_of_the_United_States>
   - United States Gross Federal Debt to GDP  <https://tradingeconomics.com/united-states/government-debt-to-gdp>
   - Consumer Debt
   - A Brief History of Consumer Culture <https://thereader.mitpress.mit.edu/a-brief-history-of-consumer-culture/>
   - Personal Savings Rate and Revolving Credit <https://en.wikipedia.org/wiki/Consumer_debt#/media/File:Personal_savings_rate_&_revolving_credit.webp>
   - Consumer and Government Debt as a % of GDP <https://en.wikipedia.org/wiki/File:Consumer_and_Government_Debt_as_a_%25_of_GDP.png>
  - Worker Productivity
     - Changing profile of stay-at-home parents <https://www150.statcan.gc.ca/n1/pub/11-630-x/11-630-x2016007-eng.htm>
     - After Decades of Decline, A Rise in Stay-at-Home Mothers <https://www.pewresearch.org/social-trends/2014/04/08/after-decades-of-decline-a-rise-in-stay-at-home-mothers/>
     - United States Nonfarm Labour Productivity <https://tradingeconomics.com/united-states/productivity>
  
  - Wage growth.
    - United States Wages and Salaries Growth <https://tradingeconomics.com/united-states/wage-growth>

  - USA Imports
    - United States Imports   <https://tradingeconomics.com/united-states/imports>
  
  - USA Exports
    United States Imports Exports <https://tradingeconomics.com/united-states/exports>

  - Balance of Trade
    United States Balance of Trade <https://tradingeconomics.com/united-states/balance-of-trade>

  - United States Total Vehicle Sales
      United States Total Vehicle Sales <https://tradingeconomics.com/united-states/total-vehicle-sales>

  - United States Manufacturing Production
      United States Manufacturing Production <https://tradingeconomics.com/united-states/manufacturing-production>

  - Small business perception
      Canada CFIB Business Barometer <https://tradingeconomics.com/canada/small-business-sentiment>

  - United States Personal Savings Rate
      United States Personal Savings Rate <https://tradingeconomics.com/united-states/personal-savings>

  - Credit Market Debt to Disposable Income
    Canada Households Credit Market Debt to Disposable Income <https://tradingeconomics.com/canada/households-debt-to-income>


  - Consumer Spending
    United States Consumer Spending  <https://tradingeconomics.com/united-states/consumer-spending>
    Canada Consumer Spending  <https://tradingeconomics.com/canada/consumer-spending>

  - Consumer Confidence
      United States Michigan Consumer Sentiment <https://tradingeconomics.com/united-states/consumer-confidence>

  - Medical Stats
      United States Medical Doctors <https://tradingeconomics.com/united-states/medical-doctors>
      United States Nurses <https://tradingeconomics.com/united-states/nurses>
      United States Hospital Beds <https://tradingeconomics.com/united-states/hospital-beds>

  - Environment
    World CO2 Emissions <https://tradingeconomics.com/world/co2-emissions>
    United States CO2 Emissions <https://tradingeconomics.com/united-states/co2-emissions>
    China CO2 Emissions <https://tradingeconomics.com/china/co2-emissions>
    United States Average Temperature <https://tradingeconomics.com/united-states/temperature>
    A fair way of carbon emissions <https://blog.datawrapper.de/four-ways-compare-emissions/>

  - Economic
    United States Corporate Profits <https://tradingeconomics.com/united-states/corporate-profits>
    Industrial Revolution GDP growth "Camels in the Amazon" <https://ourworldindata.org/grapher/gdp-world-regions-stacked-area>
  - Real wages, not risen since 1970. <https://fred.stlouisfed.org/series/LES1252881600Q>

  - Geography
    Suburbanization rates... 
   
  - Obesity in adults, 1975 to 2016
  <iframe src="https://ourworldindata.org/grapher/share-of-adults-defined-as-obese?tab=chart&country=~USA" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

  - Biodiveristy
  <iframe src="https://ourworldindata.org/grapher/global-living-planet-index" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

  - Annual working hours per worker
  <iframe src="https://ourworldindata.org/grapher/annual-working-hours-per-worker?time=1913..latest" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

  - Productivity: output per hour worked
  <iframe src="https://ourworldindata.org/grapher/labor-productivity-per-hour-PennWorldTable?tab=chart&time=1950..2017&country=AUS~BEL~BRA~KHM~CHL~CHN~DEU~IND~ZAF~KOR~TWN~GBR~USA~CHE" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

  - Growth of global exports
<iframe src="https://ourworldindata.org/grapher/world-trade-exports-constant-prices" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Share of people using the internet
<iframe src="https://ourworldindata.org/grapher/share-of-individuals-using-the-internet" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Literacy rates
<iframe src="https://ourworldindata.org/grapher/literate-and-illiterate-world-population" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Historical cost of computer memory and storage
<iframe src="https://ourworldindata.org/grapher/historical-cost-of-computer-memory-and-storage" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Moore's law: The number of transistors per microprocessor
<iframe src="https://ourworldindata.org/grapher/transistors-per-microprocessor" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Price changes in consumer goods and services in the United States
<iframe src="https://ourworldindata.org/grapher/price-changes-consumer-goods-services-united-states" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Marriages per 1,000 people
<iframe src="https://ourworldindata.org/grapher/marriage-rate-per-1000-inhabitants?time=earliest..2018&country=~USA" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

Productivity: output per hour worked
<iframe src="https://ourworldindata.org/grapher/labor-productivity-per-hour-PennWorldTable?tab=chart&time=1950..2017&country=AUS~BEL~BRA~KHM~CHL~CHN~DEU~IND~ZAF~KOR~TWN~GBR~USA~CHE" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Invention patents granted annually in the United States since 1790
<iframe src="https://ourworldindata.org/grapher/annual-patents-invention-united-states-1790" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Trust in government in the United States
<iframe src="https://ourworldindata.org/grapher/public-trust-in-government" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

Productivity Soars, Wages Stagnate
<a href="https://www.statista.com/chart/23410/inequality-in-productivity-and-compensation/" title="Infographic: Productivity Soars, Wages Stagnate | Statista"><img src="https://cdn.statcdn.com/Infographic/images/normal/23410.jpeg" alt="Infographic: Productivity Soars, Wages Stagnate | Statista" width="100%" height="auto" style="width: 100%; height: auto !important; max-width:960px;-ms-interpolation-mode: bicubic;"/></a> You will find more infographics at <a href="https://www.statista.com/chartoftheday/">Statista</a>

- Adoption of communication technologies, World
<iframe src="https://ourworldindata.org/grapher/ict-adoption" loading="lazy" style="width: 100%; height: 600px; border: 0px none;"></iframe>

- Mass incarcination rate
<https://www.sentencingproject.org/reports/mass-incarceration-trends/>

- Consumer price index
https://tradingeconomics.com/united-states/consumer-price-index-cpi#:~:text=Consumer%20Price%20Index%20CPI%20in,points%20in%20February%20of%201950.

- growth in productivity vs. compensation  - economic
https://www.epi.org/productivity-pay-gap/



population of lawyers
meat consumption
children per women
https://ourworldindata.org/grapher/children-per-woman-un?tab=chart&country=~USA

medien house cost and household income
https://www.realestatewitch.com/house-price-to-income-ratio-2021/
https://www.longtermtrends.net/home-price-median-annual-income-ratio/
https://dqydj.com/historical-home-affordability/



  - Percentage of Boomers with Grandkids
  - Public Sector Wages.
  - Loss of Manufacturing.
  - Rise of China.
  - Bowling Alone.
  - Marriage Rates.
  - Spinsters.
  - Increased paperwork, ex. doctors.
  - Time to construction/permits.
  - Chips offshoring.
  - Consultants.
  - Engineers.

 -->