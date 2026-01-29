---
layout: default
title: Home
hero_image: /images/sproati.jpg
hero_title: Hawaiian <em>Drosophila</em> Genomes Project
hero_subtitle: Evolutionary genomics of Hawaiian flies for conservation and discovery
---

<section id="about" class="section">
    <div class="container">
        <h2>About the project</h2>
        <div class="about-content">
            <p>
                The Hawaiian <em>Drosophila</em> Genomes Project is a collaborative effort to sequence, assemble, and compare the
                genomes of all of the estimated 1,000 species of flies in the family Drosophilidae 
                endemic to the Hawaiian Islands. This evolutionary radiation is one of the most remarkable examples 
                of biological diversification in our 
                modern world, and it provides an unparalleled opportunity to understand how evolution acts upon the genome to 
                generate novel morphological, ecological, and behavioral traits. At the same time, threats from habitat loss
                and invasive species, among others, present an urgent need to monitor and conserve this unique biodiversity.
                Our objectives are to build a comprehensive and publicly available genomic resource that will unlock our 
                understanding of the genetic basis of evolutionary innovation while providing new tools to aid in their conservation
                for generations to come.
            </p>
            <div class="highlights">
                <div class="highlight-box">
                    <h3>Research Goals</h3>
                    <ul>
                        <li>Sequence, assemble, and annotate genomes from all species of Hawaiian <em>Drosophila</em> and <em>Scaptomyza</em></li>
                        <li>Reconstruct the evolutionary relationships and history of the clade</li>
                        <li>Analyze genomic variation, population structure, and signatures of selection</li>
                        <li>Build genomic tools for species identification, monitoring, and conservation</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="team" class="section section-alt">
    <div class="container">
        <h2>Team</h2>
        <div class="personnel-grid">
            {% assign sorted_team = site.team | sort: 'order' %}
            {% for member in sorted_team %}
            <div class="person-card">
                <div class="person-photo">
                    <img src="{{ member.photo | relative_url }}" alt="{{ member.name }}">
                </div>
                <h3>{{ member.name }}</h3>
                <p class="person-institution">{{ member.institution }}</p>
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
                All new data generated for this work will be made publicly available and deposited at NCBI SRA and GenBank.
            </p>
            <p> Data from previous publications is available under BioProject <a href="https://www.ncbi.nlm.nih.gov/bioproject/PRJNA1020440">PRJNA1020440</a>. The whole-genome alignment is archived at <a href="https://doi.org/10.5061/dryad.x0k6djhrd">Dryad</a>. Illumina-only assemblies, RepeatModeler2 libraries, variant calls, diploid assemblies, genomes, and phylogenetic trees are archived at <a href="https://doi.org/10.5281/zenodo.11200891">Zenodo</a>. Raw Nanopore signal data (fast5, pod5) are available upon email request due to large file sizes.
            </p>
            <div class="data-links">
                <div class="data-link-card">
                    <h3>NCBI BioProject</h3>
                    <p>Sequencing data and genome assemblies (SRA/GenBank)</p>
                    <a href="https://www.ncbi.nlm.nih.gov/bioproject/PRJNA1020440" class="btn">View on NCBI</a>
                </div>
                <div class="data-link-card">
                    <h3>Whole-Genome Alignment</h3>
                    <p>Genome alignment files archived at Dryad</p>
                    <a href="https://doi.org/10.5061/dryad.x0k6djhrd" class="btn">View on Dryad</a>
                </div>
                <div class="data-link-card">
                    <h3>Illumina-Only Assemblies & Analyses</h3>
                    <p>Supporting files, trees, and analyses on Zenodo</p>
                    <a href="https://doi.org/10.5281/zenodo.11200891" class="btn">View on Zenodo</a>
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
                Research findings and discoveries from the Hawaiian <em>Drosophila</em> Genomes Project 
                are published in peer-reviewed journals. Publications will be listed here as they 
                become available.
            </p>
            <div class="publications-list">
                {% bibliography --query @*[year=2024] %}
            </div>
        </div>
    </div>
</section>
