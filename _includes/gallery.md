<h2 id="gallery" style="margin: 2px 0px 20px;">Gallery</h2>

<div class="gallery-grid">
  {% for item in site.data.gallery %}
  <div class="gallery-item">
    <img src="{{ item.image }}" alt="{{ item.title }}" loading="lazy">
    <div class="gallery-caption">
      <strong>{{ item.title }}</strong><br>
      <span style="color: #6c757d;">{{ item.caption }}</span>
    </div>
  </div>
  {% endfor %}
</div>
