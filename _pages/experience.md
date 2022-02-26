---
layout: page
permalink: /experience/
title: Experience
# description: Experience
nav: true
baseurl: 
order: 2
jobs:
  - company: Intuit Inc., Bengaluru, India
    position: Software Engineer 2
    duration: July, 2020 &mdash; Present
    summary: Write about your core competencies in one or two sentences describing your position. If you held the position for a long time, it could be a longer section, including a couple bullet points
    logo: /assets/img/intuit-logo.png

  # Director of Digital Stratgy
  - company: Blinkit (formerly Grofers), Gurugram, India
    position: Software Engineer (Intern)
    duration: Jan, 2020 &mdash; May, 2020
    summary:  <ul class="resume-item-copy"><li>Identifying fraudulent users who claim false refunds by doing an Image validation using the Amazon Rekognition Service</li><li>Automation of customer query resolutions using auto resolution based on the configured rules.</li></ul>
    logo: /assets/img/blinkit-logo.png

  # Communications Coordinator
  - company: Dell EMC, Bengaluru, India
    position: Software Development Intern
    duration: Jun, 2008  &mdash; May, 2010
    summary: <ul class="resume-item-copy"><li>Designed and developed Desktop control application though face feature detection (Won at Juggad-a-thon 2019) and automated prototyping tool.</li><li> Implemented the framework in python and used libraries like openCV, dlib, pyautogui, speech_recognition, tkinter.</li></ul>
    logo: /assets/img/dell-logo.jpeg

  - company: Middlesex University, London, UK
    position: Research Intern (Machine Learning)
    duration: Jun, 2018  &mdash; July, 2018
    summary: Worked with the Research Group vis4sense on the project SenseMap, using Machine Learning Algorithms under Dr. Kai Xu.
    logo: /assets/img/mdx-logo-1.png
---


<section class="page">
	<div class="entry">
		<!-- begin Experience -->
		<section class="content-section">
			{% for job in page.jobs %}
			<div
				class="resume-item"
				itemscope
				itemprop="worksFor"
				itemtype="http://schema.org/Organization"
			>
        <div class="row">
          <img class="logo col-sm-0.5" src="{{job.logo}}" />
          <h3 class="resume-item-title col-sm-11.5" itemprop="name"><b>{{ job.company }}</b></h3>
        </div>
				<h4 class="resume-item-details" itemprop="description">
					<i>{{ job.position }} &bull; {{ job.duration }}</i>
				</h4>
				<p class="resume-item-copy">{{ job.summary }}</p>
			</div>
			<!-- end of resume-item -->
			{% endfor %}
		</section>
		<!-- end Experience -->
	</div>
</section>
