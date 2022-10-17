---
layout: post
title: Projectify
description: A React app thats finds listening their perfect nights out
image: assets/images/projectifybanner.png
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<section id="one">
	<div class="inner">

<!-- Content -->
<div class="row">
	<div class="6u 12u$(small)">
		<h3>TL;DR</h3>
		<p>Projectify is a React app that matches Spotify listeners to their most recommended events using their listening history</p>
		<h3>Summary</h3>
		<p>After leaving Northcoders, I was excited to start building something that was mine all mine. Something fun, useful, and that solved real world problems. I didn’t know what it would be but I knew I wanted to use the Spotify API. <br/><br/>

See, I am a HUGE audiophile. I love finding hidden gems, reacquainting with forgotten sounds, and discovering new genres. Every December, my Spotify Unwrapped graciously lets me know I’ve streamed to 5+ months worth of music in the past year.
<br/><br/>
Naturally, I had a bunch of ideas I was keen to explore but a fresh winning idea came to me at graduation when Leonie, my teammate on <a href="./proj3-hallpass.html">Hallpass App</a>, snuck away early to go to Warehouse Project. 
<br/><br/>
For the uninitiated, Warehouse Project (WHP for short) is an annual 4-month long festival that brings the best DJs and musical acts from around the globe to Manchester. Each summer, the lineup announcement leaves fans counting their pennies in a desperate scramble to figure out which nights to attend and which ones to miss. Leonie and I both know the feeling all too well.
<br/><br/>
If it wasn’t for the £40+ ticket price per night we’d happily buy them all! But until our profitable careers in software engineering takes off we’re building Projectify. Our nifty web app scans the user’s Spotify listening history to gather lots of different datapoints about their musical preferences. We then spin that data through a few different algorithm to rank which WHP sessions are most suitable for that listener. </p>
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
						<td><a href="https://projectify.live" target="_blank"><i class="fa-solid fa-globe"></i> Live site</a></td>	
					</tr>
                    <tr>
						<td><a href="https://github.com/jamalxwm/projectify" target="_blank" class="icon fa-github"> Codebase</a></td>	
					</tr>
                  
                    <thead>
					<tr style="display:flex;background-color:#fff;justify-content:center">
                        
						<th style="color:#242943">Tech Stack</th>
                        	
					</tr>
				</thead>
                    <tr style="text-align:center">
						<td>
                            <ul style="list-style-type:none">
                                
                                <li>React</li>
                                <li>Firebase</li>
                                <li>Spotify API</li>
								<li>Cheerio</li>
								<li>Material UI</li>
								<li>...more to come</li>
                            </ul>
                        </td>	
					</tr>  
				</tbody>
				
			</table>
		</div>
	</div>
</div>

	<h2>The build</h2>
	<p>This is still a work in progress, so here’s where we’re up to so far. <br/><br/>

We stuck with React and Firebase as our foundation stack for their familiarity and thus speed. Could we have explored Svelte, Vue, or Mongo DB? Sure, but we wanted to produce something quickly and we know that working with the Spotify data will ultimately be our biggest challenge. Being comfortable with React and Firebase already means that we can concentrate all our learning on perfecting the algorithms and data modelling we’ll need. <br/><br/>

Initially we considered hardcoding the musical acts into the Firestore but because WHP sees hundreds of artists each season, Leonie took it on herself to build a web scraper using Cheerio! We’re 90% of the way there and resolved most issues like removing the vertical bar (which WHP uses as spacers), separating two DJs who appear back to back (usually denoted as ‘DJ A B2B DJ B’), and scrapping the word “Live” (which honestly most fans can’t explain in reference to DJ sets). We’re still working out how to replace the html &lt;br/&gt; tags with spaces which are unintentionally joining some acts together in a single string.<br/><br/>

Once we figure that last bit out we it will open so many opportunities to using historical data in building out our algorithms.
I’ll update this page as and when there’s more information to share </p>

</div>
</section>

</div>
