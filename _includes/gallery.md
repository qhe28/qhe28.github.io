<h2 id="gallery" style="margin: 2px 0px 20px;">Gallery</h2>

<div class="gallery-grid">
  {% for item in site.data.gallery %}
    
    {% if item.subfigures %}
      <figure class="latex-figure">
        <div class="subfigures-wrapper">
          {% for sub in item.subfigures %}
            <figure class="latex-subfigure">
              <img src="{{ sub.image }}" alt="{{ sub.title }}" loading="lazy">
              <figcaption>{{ sub.title }}</figcaption>
            </figure>
          {% endfor %}
        </div>
        <figcaption class="master-caption">
          <strong>{{ item.master_title }}:</strong> {{ item.master_caption }}
        </figcaption>
      </figure>

    {% else %}
      <div class="gallery-item">
        <img src="{{ item.image }}" alt="{{ item.title }}" loading="lazy">
        <div class="gallery-caption">
          <strong>{{ item.title }}</strong><br>
          <span style="color: #6c757d;">{{ item.caption }}</span>
        </div>
      </div>
    {% endif %}

  {% endfor %}
</div>
