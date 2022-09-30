---
layout: post
title: Papers (FE)
description: A Reddit-style web app built with React
image: assets/images/pic11.jpg
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
			<h2><em>"Frontend problems are like a dot..."</em></h2>
			<h4>-Kev</h4>
		</div>
		<h3>TL;DR</h3>
		<p>Built on the foundations of Papers (Backend), Papers (frontend) is a Reddit-style web app built using React. It employs best practices for mobile first development, state management, optimistic rendering, and error handling. </p>
		<h3>Objectives</h3>
			<ul>
				<li>Plan and build responsive web app with React employing mobile first strategies</li>
				<li>Make use of optimistic rendering for patch and post requests </li>
				<li>Use hooks for state management and asynchronous functions</li>
                <li>Interpret and handle client and server side errors</li>
			</ul>
		<h3>Summary</h3>
		<p>Papers culminated our <a href="./proj1-papers.html" target="_blank">backend sprint</a> into a full-fledged functional web app built with React. While React is admittedly overkill for the needs of this project it's primary purpose was to familiarise us with building apps in React, optimistic rendering, handling frontend errors, and consolidate our learning of hooks, states, and components.<br/><br/>Although basic CSS styling was encouraged along the way, it was made clear this was only of secondary importance.<br/><br/>Through this sprint I also learned the importance of planning to keep things functioning smoothly. </p>
		</div>
	<div class="6u$ 12u$(small)">
		<div class="table-wrapper">
			<table>
				<thead>
					<tr>
						<th>Name</th>
						<th>Description</th>
						<th>Price</th>
					</tr>
				</thead>
				<tbody>
					<tr>
						<td>Item1</td>
						<td>Ante turpis integer aliquet porttitor.</td>
						<td>29.99</td>
					</tr>
					<tr>
						<td>Item2</td>
						<td>Vis ac commodo adipiscing arcu aliquet.</td>
						<td>19.99</td>
					</tr>
					<tr>
						<td>Item3</td>
						<td> Morbi faucibus arcu accumsan lorem.</td>
						<td>29.99</td>
					</tr>
					<tr>
						<td>Item4</td>
						<td>Vitae integer tempus condimentum.</td>
						<td>19.99</td>
					</tr>
					<tr>
						<td>Item5</td>
						<td>Ante turpis integer aliquet porttitor.</td>
						<td>29.99</td>
					</tr>
				</tbody>
				<tfoot>
					<tr>
						<td colspan="2"></td>
						<td>100.00</td>
					</tr>
				</tfoot>
			</table>
		</div>
	</div>
</div>

	<h2>The build</h2>
	<p><span class="image left"><img src="{% link assets/images/pic09.jpg %}" alt="" /></span>Initially I struggled with frontend. Working on the assumption frontend would be entirely about "making things look pretty" I found myself in for a rude awakening when dealing with the DOM. Even after learning how React negated the need for directly dealing with the DOM, I still awaited the point where frontend became less technical and more beautiful.<br/><br/>By week two of frontend module I accepted that was never going to be the case.<br/><br/>Having accepted that frontend would be harder than backend, I started this build entirely with MUI components to avoid losing my sanity in a maze of flexboxes. MUI's syntax wasn't intuitively simple as I'd hoped so I relied heavily on YouTube tutorials to push through this.<br/><br/>At the start of the project we drew plans for our components, paying special attention to props and states that would need to be passed around. This was not only for our own benefits in devlopment but we'd also need to submit this along with any helpdesk requests.<br/><br/>Naturally, as a first timer my plan was pretty botched which I discovered on my first helpdesk call where I found some of my states were held too low or too high. In fairness it's difficult to understand what any of this means until you get stuck in and break things and figure out what went wrong.<br/><br/>If you're not breaking things, you're probably not learning.<br/><br/>By the end of the week, I had a very ugly but working app and two outstanding tickets to complete after the bootcamp.<br/><br/>Once the pressure of project week had passed and I was free to revisit this sprint in my free time, I challnged myself to make some as beautiful as it was technical. Inspired by <a href="https://papers-blog-template.webflow.io/ready-made-pages/company-blog" target="_blank">this Webflow theme</a> I stripped back as many of the orignal MUI components as possible and set myself a goal of trying to rebuild this theme as best as I could from scratch. I'm happy to say I succeeded without getting lost in a flexbox maze! </p>

<h2 id="elements">The Wins</h2>
	<div class="row">
	
	<div class="6u 12u$(small)">
		<h3>Mastering CSS debugging</h3>
		<p>Having built websites before, I've experienced firsthand the frustrations of deubgging layout issues. Endlessly tinkering with margins, padding, flexing, positions to try to get things right and chalking things up to "mysteries of the web" when they go wrong. I was grateful for being introduced to Chrome's developer tools which made this so much easier. The web is no longer mysterious to me!</p>
	</div>
	<div class="6u 12u$(small)">
		<h3>Finishing...eventually</h3>
		<p>In total this project took 10 days to complete. Five days on the course and five days after. The upside of finishing in my own time also came without the benefit of having helpdesk available. As you'll read in the challenges section below, frontend issues are TOUGH. It's a testament to my resolve that I could complete this at all using only docs and what I'd learned from Northcoders.</p>
	</div>
</div>
	<h2 id="elements">The Challenges</h2>
	<div class="row">
	
	<div class="4u 12u$(medium)">
		<h3>Debugging React</h3>
		<p>On a helpdesk call on day three, my mentor and I scratched our head over why a function I had written wasn't working as expected. By all accounts, it should have worked. After an hour troubleshooting we landed back at function that, while syntactically different, was very similar to the code I started with. Nonethless it worked. When I asked why, he said "I don't know. React just didn't like that". He continued on to say "Backend problems are like a circle; most things that can go wrong are fenced within it. Frontend issues are like a dot; the problem could be anywhere."</p>
	</div>
	<div class="4u 12u$(medium)">
		<h3>Re-rendering non-deleted comments</h3>
		<p>For reasons I'm still unsure of, I haven't figured out how to re-render a deleted comment after its API call fails. That's to say I dont know how to revert its optimistic rendering. If you have any ideas, I'd love to hear them.</p>
	</div>
	<div class="4u$ 12u$(medium)">
		<h3>Routing via URL</h3>
		<p>After deploying this app, I found that React routers browser router wasn't behaving as it should. While the URL in the browser updates as expected, if you navigated directly to the same URL or even refreshed the page you'd be met with a 404 page. While I assumed this had to do with client side vs server side routing, I found my colleagues didn't have this issue despite having the exact same setup. To circumvent this I used a Hash Router instead.</p>
	</div>
</div>
<h2 id="elements">If I started over I'd...</h2>
<div class="row">
<div class="6u 12u$(small)">
		<h3>Explore other CSS libraries</h3>
		<p>MUI is brilliant at what it does and I'd love to use it again in the future. For the purposes of this project it's syntax was added an extra learning curve that cut into the actual development time. Instead, I may have opted for Tailwinds or Bootstrap.</p>
</div>
<div class="6u 12u$(small)">
		<h3>Lift some states to app</h3>
		<p>A few components like the ArticleGrid and CommentsList require a fetchUsers function that then maps the users relevant variables (e.g. ariticle authors and comment authors). In retrospect, these asynchronous functions slow down some page loads. Performance could be improved by setting this state at app level and passing it through props.</p>
</div>
</div>

</div>
</section>

</div>
