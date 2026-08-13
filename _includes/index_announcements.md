<div class="anchor" id="news"></div>

# News
## Announcements:
* * *

<div class="day-tabs">
  <button class="day-tab active" onclick="showDay('news1', this)">ISTC Technical Seminar -- 2026 May 27</button>
  <button class="day-tab" onclick="showDay('news2', this)">ISTC Technical Seminar -- 2026 Mar 18</button>
  <button class="day-tab" onclick="showDay('news3', this)">ISTC Technical Seminar -- 2026 Feb 9</button>
</div>

<div class="day-panel active" id="news1">
  <!-- {% include news/2026_05_27.md %} -->
  {% capture my_news1 %}{% include news/2026_05_27.md %}{% endcapture %}
  {{ my_news1 | liquify | markdownify }}
</div>

<div class="day-panel" id="news2">
  <!-- {% include news/2026_03_18.md %} -->
  {% capture my_news2 %}{% include news/2026_03_18.md %}{% endcapture %}
  {{ my_news2 | liquify | markdownify }}
</div>

<div class="day-panel" id="news3">
  <!-- {% include news/2026_02_09.md %} -->
  {% capture my_news3 %}{% include news/2026_02_09.md %}{% endcapture %}
  {{ my_news3 | liquify | markdownify }}
</div>

* * *

More announcements are available on the [Announcements](https://aiaa-istc.github.io/announcements.html) page.

<!-- --end-of-page-- -->
