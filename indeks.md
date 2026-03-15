---
layout: default
title: Indeks Tokoh
permalink: /indeks/
---

<div class="wrapper">
    <header class="tokoh-header">
        <h1>Indeks Tokoh</h1>
        <p class="card-meta">Daftar seluruh pemikir Indonesia yang terarsip, disusun secara alfabetis.</p>
    </header>

    <div class="indeks-container">
        {% assign sorted_tokoh = site.tokoh | sort: "title" %}
        {% assign current_letter = "" %}

        {% for tokoh in sorted_tokoh %}
            {% assign first_letter = tokoh.title | slice: 0 | upcase %}
            
            {% if first_letter != current_letter %}
                {% if current_letter != "" %}
                    </ul>
                </div>
                {% endif %}
                
                <div class="indeks-group">
                    <h2 id="{{ first_letter }}">{{ first_letter }}</h2>
                    <ul class="indeks-list">
                {% assign current_letter = first_letter %}
            {% endif %}
            
            <li>
                <div class="indeks-item">
                    <div class="indeks-main">
                        <a href="{{ tokoh.url | relative_url }}">{{ tokoh.title }}</a>
                        {% if tokoh.lahir or tokoh.wafat %}
                            <span class="card-meta">({{ tokoh.lahir | default: "?" }}–{{ tokoh.wafat | default: "sekarang" }})</span>
                        {% endif %}
                    </div>
                    {% if tokoh.bidang or tokoh.periode %}
                    <div class="indeks-meta">
                        {% if tokoh.bidang %}
                            <span class="indeks-bidang">{{ tokoh.bidang | join: ", " }}</span>
                        {% endif %}
                        {% if tokoh.periode %}
                            <span class="indeks-periode-sep">•</span>
                            <span class="indeks-periode">{{ tokoh.periode }}</span>
                        {% endif %}
                    </div>
                    {% endif %}
                </div>
            </li>
        {% endfor %}
        
        {% if current_letter != "" %}
            </ul>
        </div>
        {% endif %}
    </div>
</div>

<style>
    .indeks-container {
        margin-top: 2rem;
        column-count: 2;
        column-gap: 3rem;
    }
    .indeks-group {
        break-inside: avoid;
        margin-bottom: 2rem;
    }
    .indeks-group h2 {
        margin-top: 0;
        border-bottom: 2px solid var(--color-accent);
        display: inline-block;
        min-width: 1.5em;
        text-align: center;
    }
    .indeks-list {
        list-style: none;
        padding: 0;
        margin: 1rem 0;
    }
    .indeks-list li {
        margin-bottom: 1rem;
        font-size: 1.05rem;
        border-bottom: 1px solid rgba(201, 176, 138, 0.2);
        padding-bottom: 0.5rem;
    }
    .indeks-list a {
        font-weight: bold;
    }
    .indeks-meta {
        font-size: 0.8rem;
        color: var(--color-text-mute);
        margin-top: 0.1rem;
        line-height: 1.4;
    }
    .indeks-periode-sep {
        margin: 0 0.4rem;
        color: var(--color-border);
    }
    .indeks-periode {
        text-transform: capitalize;
        font-style: italic;
    }
    @media (max-width: 768px) {
        .indeks-container {
            column-count: 1;
        }
    }
</style>
