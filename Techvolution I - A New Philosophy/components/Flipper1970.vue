<!-- 
resources used to get this nice carousel.
https://glidejs.com/docs/setup/
https://stackoverflow.com/questions/69457943/is-it-possible-to-use-glidejs-inside-a-vue-component
https://stackblitz.com/edit/vue3-glidejs?file=src%2Fcomponents%2FCarousel.vue
-->

<!-- 
 Internet Age, 1970
 This is a carousel to display several factoids about how today societal problems started in 1969, because we entered a new age, but didn't evolve into new (technological) species.
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

  
  Graphs/Datapoints:
  - Vehicle Miles Travelled
    - total VMT <https://afdc.energy.gov/data/10315>
    - 
  - Trust in Government
    - Public Trust in Government: 1958-2022 <https://www.pewresearch.org/politics/2022/06/06/public-trust-in-government-1958-2022/>
  
    - Political party cooperation
    - The Rise of Partisanship <https://journals.plos.org/plosone/article/figure?id=10.1371/journal.pone.0123507.g002> 
    - The Rise of Partisanship video <https://www.youtube.com/watch?v=tEczkhfLwqM>
  
    - Carbon Emissions
      Trends in Global Emissions <https://www.epa.gov/ghgemissions/global-greenhouse-gas-emissions-data#:~:text=Global%20carbon%20emissions%20from%20fossil,increase%20from%201970%20to%202011.>
  
  - Planet Temperature
  
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

  - Economic
    United States Corporate Profits <https://tradingeconomics.com/united-states/corporate-profits>


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