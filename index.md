---
layout: default
title: Home
---

<section id="about" class="section">
    <div class="container">
        <h2>About the Project</h2>
        <div class="about-content">
            <p>
                The Hawaiian Drosophila Genomes Project is dedicated to advancing our understanding 
                of Hawaiian fruit fly evolution through comprehensive genomic research. Hawaii's 
                unique island ecosystem has given rise to one of the most spectacular examples of 
                adaptive radiation, with over 1,000 endemic Drosophila species.
            </p>
            <p>
                Our project aims to sequence, assemble, and analyze the genomes of these remarkable 
                species to understand the genetic basis of their adaptive traits and evolutionary 
                history. This research provides insights into speciation, adaptation, and the role 
                of genomic architecture in evolutionary processes.
            </p>
            <div class="highlights">
                <div class="highlight-box">
                    <h3>Research Goals</h3>
                    <ul>
                        <li>Generate high-quality genome assemblies</li>
                        <li>Identify genes underlying adaptive traits</li>
                        <li>Understand evolutionary relationships</li>
                        <li>Study speciation mechanisms</li>
                    </ul>
                </div>
                <div class="highlight-box">
                    <h3>Impact</h3>
                    <ul>
                        <li>Advance evolutionary biology knowledge</li>
                        <li>Support conservation efforts</li>
                        <li>Enable comparative genomics research</li>
                        <li>Foster scientific collaboration</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="personnel" class="section section-alt">
    <div class="container">
        <h2>Our Team</h2>
        <div class="personnel-grid">
            {% assign sorted_team = site.team | sort: 'order' %}
            {% for member in sorted_team %}
            <div class="person-card">
                <div class="person-photo">
                    <img src="{{ member.photo | relative_url }}" alt="{{ member.name }}">
                </div>
                <h3>{{ member.name }}</h3>
                <p class="person-title">{{ member.title }}</p>
                <p class="person-bio">{{ member.bio }}</p>
            </div>
            {% endfor %}
        </div>
    </div>
</section>

<section id="data" class="section">
    <div class="container">
        <h2>Data & Resources</h2>
        <div class="data-content">
            <p>
                We are committed to open science and making our genomic data freely available 
                to the research community. Data from the project will be deposited in public 
                repositories as they become available.
            </p>
            <div class="data-links">
                <div class="data-link-card">
                    <h3>Genome Assemblies</h3>
                    <p>High-quality genome assemblies for Hawaiian Drosophila species</p>
                    <a href="#" class="btn btn-disabled" tabindex="-1">Coming Soon</a>
                </div>
                <div class="data-link-card">
                    <h3>Sequence Data</h3>
                    <p>Raw sequencing data and processed datasets</p>
                    <a href="#" class="btn btn-disabled" tabindex="-1">Coming Soon</a>
                </div>
                <div class="data-link-card">
                    <h3>Analysis Tools</h3>
                    <p>Custom scripts and pipelines for data analysis</p>
                    <a href="#" class="btn btn-disabled" tabindex="-1">Coming Soon</a>
                </div>
                <div class="data-link-card">
                    <h3>Publications</h3>
                    <p>Research articles and preprints from the project</p>
                    <a href="#" class="btn btn-disabled" tabindex="-1">Coming Soon</a>
                </div>
            </div>
        </div>
    </div>
</section>
