---
layout: postalt
title: Hallpass App
description: A marketplace for tutors built with React Native
image: assets/images/hallpasscover.jpg
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<iframe width="100%" height="315" src="https://www.youtube.com/embed/_nZw0vASIPk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<section id="one">
	<div class="inner">

<!-- Content -->
<div class="row">
	<div class="6u 12u$(small)">
		<div style="text-align: center">
			<h2><em>"It's not about what you know. It's about what you know you can Google."</em></h2>
			<h4>-Leonie Phelps</h4>
		</div>
		<h3>TL;DR</h3>
		<p>Hallpass App is a mobile app connecting learners looking for personalised tuition in a specialist skill with available local and virtual tutors. It was built by a team of four using React Native and Firebase as part of a Northcoders final project.  </p>
        <h3>Project objectives</h3>
			<ul>
				<li>Build an MVP using two technologies not learned on the course</li>
				<li>Continue using agile methodologies for planning and development </li>
                <li>Learn faster and break things as Northcoders' support will be limited </li>
			</ul>
		
	</div>
	<div class="6u$ 12u$(small)">
		<div class="table-wrapper">
			<table>
				<thead>
					<tr style="display:flex;background-color:#fff;justify-content:center;align-item:center">
                        
						<th style="color:#242943">Links</th>
                        	
					</tr>
				</thead>
				<tbody style="text-align:center">
					<tr>
						<td><a href="https://youtu.be/_nZw0vASIPk" target="_blank" class="icon fa-youtube"> Product Demo</a></td>	
					</tr>
                    <tr>
						<td><a href="https://github.com/jamalxwm/hallpass-app" target="_blank" class="icon fa-github"> Codebase</a></td>	
					</tr>
                    <thead>
					<tr style="display:flex;background-color:#fff;justify-content:center">
                        
						<th style="color:#242943">Tech Stack</th>
                        	
					</tr>
				</thead>
                    <tr style="text-align:center">
						<td>
                            <ul style="list-style-type:none">
                                <li><i class="fa-brands fa-react"></i> React Native</li>
                                <li><i class="fa-regular fa-laptop-mobile"></i> Expo</li>
                                <li><i class="fa-solid fa-database"></i> Firebase</li>
                                <li><i class="fa-solid fa-database"></i> Google Cloud Trigger Functions</li>
                                <li><i class="fa-solid fa-map"></i> Google Maps API</li>
                                <li><i class="fa-solid fa-camera-web"></i> Whereby API</li>
                            </ul>
                        </td>	
					</tr>
                    <thead>
					<tr style="display:flex;background-color:#fff;justify-content:center">
                        
						<th style="color:#242943">By the numbers</th>
                        	
					</tr>
				</thead>
                    <tr style="text-align:center">
						<td><i class="icon fa-calendar"> 10 days to complete</i></td>	
					</tr>
                    <tr style="text-align:center">
						<td><i class="icon fa-coffee"> 106 cups of coffee</i></td>	
					</tr>
					<tr style="text-align:center">
						<td><i class="icon fa-moon"> 8 late nights</i></td>	
					</tr>
                    <tr style="text-align:center">
						<td><i class="fa-solid fa-people-group"></i> 1 dreamy team</td>	
					</tr>
                    <tr style="text-align:center">
						<td><i class="fa-solid fa-person-harassing"></i> 0 arguments</td>	
					</tr>
				</tbody>
				
			</table>
		</div>
</div>
        <h3>Summary</h3>
		<p>After 10 arduous week of ceaseless coding,  sleeping, repeating—punctuated only by healthy doses of crying and seeking dopamine from the northcoders snack bowl and/or the bottom of an after work pint glass—we survived to meet the dreaded final project weeks. <br/><br/>

        Dreaded because, now, everything relied solely on the imperceptible competence and bravado in ourselves and our yet-to-be-defined team members. What we chose to build and how we’d build it was entirely up to us to decide. Because the imperative was to use technologies not taught on the bootcamp, it was made clear at the start that the level of support helpdesk calls could offer would vary according to the responder’s own experience. Almost without exception, we’d be left entirely at the whim of developer docs and YouTube tutorials (as capable developers are wont to do).
        <br/><br/>
        By sheer luck I landed myself in a dream team with three very coolheaded and skilful engineers. There’d be no vainglorious ego clashes in pursuit of our decided build, Hallpass, an ‘Uber for tutors’.
        <br/><br/>
        Our solution was as simple as it was beautiful. A marketplace matching capable tutors with those wanting to learn or advance a new skill. While finding a local tutor for academic subjects may be somewhat easy (depending on your location), where does one look for personalised tuition in a niche or advanced skill? Hallpass solves the former by allowing users to find local tutors available in-person and achieves the latter by allowing tutees to learn virtually via video call from directly within the React Native app.  
        <br/><br/>
        To further our philosophy of “learn anything anywhere”,  a proposed feature added a library of borrowable equipment to make learning any new skill accessible and affordable without the usual upfront sunk costs.
        <br/><br/>
        Referencing the ubiquitous terms & conditions of any educational or employment contract, our mentor stressed that Northcoders owns the IP to whatever we produce and emphasised that “this may be too good for a final project”.</p>

	<h3>The build</h3>
	<p><span class="image left"><img src="{% link assets/images/hallpassteam.jpg %}" alt="the hallpass team" /></span>Despite filling three weeks in our schedule the reality was that we’d have only 10 days to build our MVP. Bookending the start of that week and half was a bank holiday, and one day each, for pitch development, practice resolving issues git conflict, more agile engingeering, prep and spiking. The final two days were spent recording and watching our product demos.  
<br/><br/>
Spiking took much longer than expected as some technologies specifically sendbird for handling video calls, were less than compatible with our Expo managed workflow. 
<br/><br/>
We quickly found ourselves revisiting any proposed packages that required access to native modules and found building a truly functional in-app chat and video calling feature, to the standard we would’ve liked, would be a time consuming task. On this we made trade offs using Whereby’s API inside an iframe and a simulated in-app chat.
<br/><br/>
Firebase became a two day long sticking point as many of the tutorials we found demonstrated syntax for Firebase 8 which we had to figure out how to refactor for Firebase 9. Luckily we found Google’s documentation to be superbly clear. 
<br/><br/>
While working through this Firebase saga, A true defining moment arose when I ecstatically jumped out of the corner office we commandeered shouting that I’d finally got a NEW error. Seemingly a hallmark of progress. 
<br/><br/>
Two separate NC mentors independently suggested NoSQL for our solution which we eventually came to rethink when we realised a relational database would’ve been much more efficient in building our equipment library feature.
<br/><br/>
As we continued to pair program throughout the project working on individual tickets we never encountered any major git conflicts. The one conflict that did emerge was solved with a quick and easy rebase. 
<br/><br/>
By our final build day, we were comfortably left with styling as our only major task. As we stood back in awe of what we’d accomplished we all wondered how we managed all this in just 10 days. To which Leonie emphatically announced “it’s not what you know. It’s what you know you can Google”. 
<br/><br/>
Truer words were never spoken. 
</p>



</div>
</div>
</section>

</div>
