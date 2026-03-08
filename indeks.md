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
                <a href="{{ tokoh.url | relative_url }}">{{ tokoh.title }}</a>
                {% if tokoh.lahir or tokoh.wafat %}
                    <span class="card-meta">({{ tokoh.lahir | default: "?" }}–{{ tokoh.wafat | default: "sekarang" }})</span>
                {% endif %}
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
        margin-bottom: 0.5rem;
        font-size: 1.05rem;
    }
    .indeks-list a {
        font-weight: bold;
    }
    @media (max-width: 600px) {
        .indeks-container {
            column-count: 1;
        }
    }
</style>
