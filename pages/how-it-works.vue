<template>
  <div class="container">
    <section class="hero">
      <div class="media">
        <img
          src="https://cms.mixers.com/assets/5A2EFFD1-E688-4C71-AD4F-6F57364E0935?format=webp"
        >
      </div>
    </section>
    <main class="wrapper flex">
      <StructureSidebarDefault class="sidebar flex30">
        <SectionQuoteRequest
          :content="'To learn more about ' + appConfig.title"
        />
        <div class="related">
          <h3>Common Static Mixer Applications</h3>
          <ul>
<li>Thermal homogenization extrusion and injection molding</li>
<li>Color blending extrusion and injection molding</li>
<li>Wastewater neutralization</li>
<li>PH control</li>
<li>Starch cooker</li>
<li>Heat exchanger</li>
<li>Food mixing and blending</li>
<li>Reactive mixes such as epoxies and urethances</li>
<li>Plastic pellets </li>
          </ul>
        </div>
      </StructureSidebarDefault>
      <div class="flex70 bl-light contentSection mti">
        <div>
          <section id="howitworks" class="bb-light px-3">
            <h4>How It Works</h4>
            <h2>How to Select a Static Mixer</h2>

            <p>Static Mixers are easily sized using available formulas and pressure drop charts. Your initial selection can be made by following the guidelines listed below. To fine tune your selection contact our application engineering staff.</p>

<h3>(1) Determine the mixer type using the Motionless Table:</h3>
<table class="tblContent fullwidth">
										<tr>
											<th>Type
															of Flow
											</th>
											<th># of LPD
											</th>
											<th># of ISG
															Elements
											</th>
										</tr>
										<tr>
											<td>
												<center>
													<font size="2"><b>Turbulent</b></font></center>
											</td>
											<td>
												<center>
													<font size="2">2 - 6 </font></center>
											</td>
											<td>
												<center>
													<font size="2">4</font></center>
											</td>
										</tr>
										<tr>
											<td>
												<center>
													<font size="2"><b>Laminar</b></font></center>
											</td>
											<td> </td>
											<td> </td>
										</tr>
										<tr height="28">
											<td width="36%" height="28">
												<center>
													<font size="2"><b>Viscosity Ratio =  0.1 to
															1,000</b></font></center>
											</td>
											<td width="32%" height="28">
												<center>
													<font size="2">24</font></center>
											</td>
											<td width="32%" height="28">
												<center>
													<font size="2">10</font></center>
											</td>
										</tr>
										<tr height="28">
											<td width="36%" height="28">
												<center>
													<font size="2"><b>Viscosity Ratio = 1,000 to
															10,000</b></font></center>
											</td>
											<td width="32%" height="28">
												<center>
													<font size="2">36</font></center>
											</td>
											<td width="32%" height="28">
												<center>
													<font size="2">14</font></center>
											</td>
										</tr>
										<tr height="28">
											<td width="36%" height="28">
												<center>
													<font size="2"><b>Viscosity Ratio =  10,000 to
															100,000</b></font></center>
											</td>
											<td width="32%" height="28">
												<center>
													<font size="2">48</font></center>
											</td>
											<td width="32%" height="28">
												<center>
													<font size="2">20</font></center>
											</td>
										</tr>
									</table>
									<p style="font-size:.8rem;">*Viscosity Ratio  = &micro;p/&micro;m<br>
											(viscosity of primary stream p / viscosity of minor stream m)</p>


<h3>(2) Assume a mixer diameter</h3>

<h3>(3) Estimate Pressure Drop</h3>

<ol>
  <li>Compute the Reynolds Number:<br>
												<br>
												<table border="0" cellpadding="2" cellspacing="0">
													<tr>
														<td rowspan="2">NRe &nbsp;=</td>
														<td>
															<center>
																<font size="2"><u>6.31w</u></font></center>
														</td>
														<td rowspan="2">=</td>
														<td>
															<center>
																<font size="2"><u>3,161 Q * sg</u></font></center>
														</td>
													</tr>
													<tr>
														<td>
															<center>
																<font size="2">&micro;D</font></center>
														</td>
														<td>
															<center>
																<font size="2">&micro;D</font></center>
														</td>
													</tr>
												</table>
												<p><b>NRe</b> = Reynolds number dimensionless<br>
													<b>D</b> = Inside diameter of mixer housing, inches<br>
													<b>Q</b> = Volumetric flow rate, gallons/minute<br>
													<b>w</b> = Mass flow rate, pounds/hour<br>
													<b>sg</b> = Specific gravity<br>
													<b>&micro;</b> = Absolute viscosity, centipoise
												</p>
  </li>
  <li>If NRe &lt; 500 the flow is laminar. Use either <a href="https://cdn.mixers.com/images/static-figure1.jpg" target="_blank">Fig.1</a> for LPD or <a href="https://cdn.mixers.com/images/static-figure3.jpg" target="_blank">Fig.3</a> for ISG mixers to estimate the pressure drop per element. If NRe &gt; 500, the flow is turbulent. The pressure drop per element is estimated from <a href="https://cdn.mixers.com/images/static-figure2.jpg" target="_blank">Fig.2</a> for LPD or <a href="https://cdn.mixers.com/images/static-figure4.jpg" target="_blank">Fig.4</a> for ISG mixers.</li>
  <li>Multipy the pressure drop per element by the total number of elements to obtain the estimated pressure drop through the mixer.</li>
  <li>The estimated pressure drop must be corrected for physical properties as follows:
												<ul>
													<li>For turbulent flow, multiply the estimated pressure drop by the specific gravity and the correction factor K from the table below to obtain the actual pressure drop.

                            <table class="tblContent">
                              <tr height="25">
                                <th>
                                  <center>
                                    <font><b>Viscosity, cps.</b></font></center>
                                </th>
                                <th>
                                  <center>
                                    <font><b>K</b></font></center>
                                </th>
                              </tr>
                              <tr height="25">
                                <td>
                                  <center>
                                    <font size="2">10</font></center>
                                </td>
                                <td>
                                  <center>
                                    <font size="2">1.1</font></center>
                                </td>
                              </tr>
                              <tr height="25">
                                <td>
                                  <center>
                                    <font size="2">100</font></center>
                                </td>
                                <td>
                                  <center>
                                    <font size="2">1.3</font></center>
                                </td>
                              </tr>
                              <tr height="25">
                                <td>
                                  <center>
                                    <font size="2">1000</font></center>
                                </td>
                                <td>
                                  <center>
                                    <font size="2">1.5</font></center>
                                </td>
                              </tr>
                              <tr height="25">
                                <td>
                                  <center>
                                    <font size="2">5000</font></center>
                                </td>
                                <td>
                                  <center>
                                    <font size="2">1.6</font></center>
                                </td>
                              </tr>
                            </table>
                        </li>

                        <li>For laminar flow, the pressure drop is proportional to the viscosity. Since <a href="https://cdn.mixers.com/images/static-figure1.jpg" target="_blank">Fig.1</a> and <a href="https://cdn.mixers.com/images/static-figure3.jpg" target="_blank">Fig.3</a> are based on a fluid having a viscosity of 10,000 cps, the actual pressure drop is calculated as follows:

                            <table>
                              <tr>
                                <td rowspan="2">Actual Pressure Drop = </td>
                                <td style="text-align:center;"><u>viscosity in cps</u></td>
                                <td rowspan="2">x est. pressure drop</td>
                              </tr>
                              <tr>
                                <td style="text-align:center;">10,000</td>
                              </tr>
                            </table>
                        </li>
                      </ul>
  </li>
  <li>To determine LLPD pressure drop, multiply LPD pressure drop by 0.46 (if turbulent). In laminar flow, the LPD and LLPD have similar pressure drop.
  </li>
  <li>If actual pressure drop exceeds the allowable value, repeat above steps using a larger mixer diameter.
  </li>
</ol>

          </section>
        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
import appConfig from '~/app.config';

useSeoMeta({
  title: 'Static Mixers for Process Industry Applications',
  description: 'Static and motionless - no moving parts inline continuous mixers for food, chemical, petrochemical, wastewater applications',
  ogImage: 'https://cms.mixers.com/assets/A54D4CFE-789F-4197-8E12-DA556F850C89?height=700&format=webp'
})
</script>

<style scoped>
.hero {
  background: #000;
  height: 300px;
  position: relative;
}

.sticky {
  position: sticky;
  top: 0rem;
  transform: translateY(0rem);
  align-self: flex-start;
}

.sidebar nav {
  background: #fff;
  padding: 2rem 0rem 2rem 2rem;
}

.sidebar nav ul {
  list-style: none;
  box-sizing: border-box;
}

.sidebar nav ul li a {
  padding: 1rem 3rem;
  display: block;
  text-align: right;
  border-bottom: 1px solid var(--light-gray);
  color: #465b6d;
  text-decoration: none;
}

.contentSection {
  box-sizing: border-box;
  background: #fff;
  margin-top: -10rem;
}

section {
  box-sizing: border-box;
  padding-top: 3rem;
  padding-bottom: 3rem;
}

.hero h1 {
  font-size: 3.2rem;
  line-height: 4rem;
  color: #fff;
  text-shadow: 5px 5px 0px rgba(0, 0, 0, 0.2);
}

.hero .media {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  overflow: hidden;
}

.hero .media img {
  object-fit: cover;
  width: 100%;
  height: 100%;
  object-position: center;
}

div.related {
  margin-top: 3rem;
  position: relative;
  width: 80%;
  float: right;
  padding-right: 3rem;
  text-align: right;
}

div.related ul {
  list-style: none;
}

div.related ul li {
  font-size: 1rem;
  margin-bottom: 1rem;
  line-height: 1.5rem;
}

table.tblContent th {
	background:#cae2fa;
	padding:5px 15px;
	border-bottom:1px solid #a0bfde;
}

table.tblContent td {
	padding:5px 15px;
	border-bottom:1px solid #a0bfde;

}

.contentSection ol li {
  margin-bottom:3rem;
}

@media screen and (max-width: 768px) {

.hero {
  display:none;
}

.contentSection {
  margin-top:0rem;
}

main.flex {
  flex-direction: column-reverse;
}

div.related {
  text-align:left;
  margin-bottom:2rem;
}

div.related ul {
  list-style:disc;
}

}

</style>
