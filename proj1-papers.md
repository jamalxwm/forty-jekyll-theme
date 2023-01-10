---
layout: post
title: Papers (BE)
description: A database, a server, an API, a Covid story
image: assets/images/papersbecover.png
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

<section id="one">
	<div class="inner">

<!-- Content -->
<div class="row">
	<div class="6u 12u$(small)">
		<div style="text-align: center">
			<h2><em>"The whole world is just one giant Covid waiting room."</em></h2>
			<h4>-Jamal Whorms-MonDésir</h4>
		</div>
		<h3>TL;DR</h3>
		<p>Papers (Backend) is an API built using Express and PostgreSQL the programatically allow for accessesing and updating a database of articles, comments, users, and topics.</p>
		<h3>Objectives</h3>
			<ul>
				<li>Build a database and API that serves data to specified endpoints using the MVC framework</li>
				<li>Employ best practices for SQL injection prevention</li>
				<li>Develop models for error handling and relaying status codes</li>
			</ul>
		<h3>Summary</h3>
		<p>Fresh off the back of a prolonged tour through callback hell and a stop through middleware midlands, our first solo sprint was to build an API for what would later become a fully-functioning Reddit-style web app in our frontend project. <br/><br/>This one week project entailed building a database with <strong>PostgreSQL</strong>, building a server and endpoints using <strong>Express.js</strong> and <strong>node-postgres</strong>, and extensive testing with <strong>Jest</strong> and <strong>Supertest</strong>. All from scratch. So no pressure there.<br/><br/> What a week to catch Covid!</p>
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
						<td><a href="https://papersjxwm.cyclic.app" target="_blank"><i class="fa-solid fa-globe"></i> Live site</a></td>	
					</tr>
                    <tr>
						<td><a href="https://github.com/jamalxwm/be-nc-news" target="_blank" class="icon fa-github"> Codebase</a></td>	
					</tr>
                    <tr>
						<td><a href="https://trello.com/b/Jca486kY/jamals-nc-news" target="_blank"><i class="fa-brands fa-trello"></i> Tickets</a></td>	
					</tr>
                    <thead>
					<tr style="display:flex;background-color:#fff;justify-content:center">
                        
						<th style="color:#242943">Tech Stack</th>
                        	
					</tr>
				</thead>
                    <tr style="text-align:center">
						<td>
                            <ul style="list-style-type:none">
                                <li><i class="fa-solid fa-database"></i> PostgreSQL</li>
                                <li>Express</li>
                                <li>Node.js</li>
								<li>Husky</li>
								<li>Jest</li>
								<li>Supertest</li>
                            </ul>
                        </td>	
					</tr>
                    <thead>
					<tr style="display:flex;background-color:#fff;justify-content:center">
                        
						<th style="color:#242943">By the numbers</th>
                        	
					</tr>
				</thead>
                    <tr style="text-align:center">
						<td><i class="icon fa-calendar"> 4 days to complete</i></td>	
					</tr>
                    <tr style="text-align:center">
						<td><i class="icon fa-bed"> 1 day in bed</i></td>	
					</tr>
					<tr style="text-align:center">
						<td><i class="fa-solid fa-wine-glass"></i> 1 well-deserved bottle of wine</td>	
					</tr>
				</tbody>
				
			</table>
		</div>
	</div>
</div>

	<h2>The build</h2>
	<p><span class="image left"><img src="{% link assets/images/besnacks.jpg %}" alt="" /></span>I long ago accepted that the whole world is one giant Covid waiting room but after fending off fate for over two, <em>'The Rona'</em> finally caught me. This wasn't a particularly convenient time for a pox on my house but, nonetheless, we move.<br/><br/>After some mindless staring into the black mirror looking for  where to get started, I managed to skeleton a working <strong>model</strong> and <strong>controller</strong> for the <a href="https://trello.com/c/SvoM2Ofe" target="_blank">first API call</a> without much fuss. I submitted it for pull request and awaited the feedback from underneath my duvet.<br/><br/>For being a predominantly visual learner, I found it remarkably easy to work with invisible databases. The next several tickets became a sort of lather, rinse, repeat excercise. And for the first time on the course, even the practice of writing tests became cogently clear now that I was working with salient data and tangible outputs.<br/><br/>I truly wish I could use this space to describe process of seeding the database, spinning up the server, and writing SQL queries but between the covidian haze and how quickly acquainted I got with everything, not much—bar the points below—has surfaced in my memory.</p>

<h2 id="elements">The Wins</h2>
	<div class="row">
	
	<div class="6u 12u$(small)">
		<h3>Querying the information schema</h3>
		<p>By day three, I was so comfortable with writing SQL queries that I was hungry for something more. I spotted an opportunity to advance my learning on <a href="https://trello.com/c/hM5JM7aQ" target="_blank">ticket #11</a>. Rather than hardcoding the topics into an array, the bare minimum needed to complete this ticket and prevent SQL injection, I figured out how to query the table's metadata via information schema for the topics list instead. Ultimately, this stood me well come frontend project where the topic values were different.</p>
	</div>
	<div class="6u 12u$(small)">
		<h3>Finishing on schedule</h3>
		<p>Despite being full of Covid and having to sit out day for rest, I managed to finish all the core tasks within the week.</p>
	</div>
</div>
	<h2 id="elements">The Challenges</h2>
	<div class="row">
	
	<div class="4u 12u$(medium)">
		<h3>Testing the tragic path</h3>
		<p>While writing tests had admittedly become easier, my tutor stressed testing more sad paths. "What if a user misspells 'inc'?" he stressed in one of his pull request comments. At this point I realised I won't always be writing code for end users who have the guiding hand of a UI and so I had to consider more of the ridiculous things that could go wrong and test for some truly tragic paths.</p>
	</div>
	<div class="4u 12u$(medium)">
		<h3>Missing a pair of eyes</h3>
		<p>As my first solo sprint, I came to truly embrace the value of pair programming after spending hours trying to resolve an object destructuring issue. An expected return value that was meant to be an array kept coming back as an object. After finally giving up and submitting the pull request anyway, the comments in the feedback pointed out exactly which line in which file was causing the issue.     </p>
	</div>
	<div class="4u$ 12u$(medium)">
		<h3>Getting to grips with <code>next</code></h3>
		<p>It's easy to miss that dev packages can do some clever things. As an overthinker, I struggled to comprehend the magic that is the <code>next</code> function in Express.js. "BUT HOW DOES IT KNOW WHAT TO DO?!" Eventually, I just had to accept that some people are just as good at overthinking as I am.</p>
	</div>
</div>
<h2 id="elements">What I'd change</h2>
		<h3>Better to async/await</h3>
		<p>Throughout most the project I stuck to what I know works, which is promise chains. Funny enough, even our tutors commented that most the cohort didn't venture into using async/await despite having a much cleaner syntax. Around the point that was diving into information schema I decided to give it a whirl and realised I had been scribing long promise chains needlessly. If theres's one thing I'd absolutely do differently its this</p>



</div>
</section>

</div>
