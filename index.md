---
layout: default
title: Home
hero_image: /images/hero-placeholder.svg
hero_title: Hawaiian Drosophila Genomes Project
hero_subtitle: Advancing our understanding of evolution through genomic research on Hawaii's remarkable fruit fly diversity
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
            </div>
        </div>
    </div>
</section>

<section id="publications" class="section section-alt">
    <div class="container">
        <h2>Publications</h2>
        <div class="publications-content">
            <p>
                Research findings and discoveries from the Hawaiian Drosophila Genomes Project 
                are published in peer-reviewed journals. Publications will be listed here as they 
                become available.
            </p>
            <div class="publications-list">
                <div class="publication-item">
                    <h3 class="pub-title">Example Publication Title</h3>
                    <p class="pub-authors">Authors et al.</p>
                    <p class="pub-journal"><em>Journal Name</em>, Year. DOI: <a href="#">10.xxxx/example</a></p>
                    <p class="pub-description">Brief description of the publication content and findings.</p>
                </div>
                
                <div class="publication-placeholder">
                    <p><em>Publications from this project will be added here as they become available.</em></p>
                </div>
            </div>
        </div>
    </div>
</section>
