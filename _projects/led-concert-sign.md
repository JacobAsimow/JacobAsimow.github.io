---
title: LED Concert Sign
subtitle: Concerts and shows at walkable SF venues
tags: [Hardware, LED matrix, Video]
video: /assets/projects/led-concert-sign/demo.mp4
---

{% if page.video %}
<video class="project-video" src="{{ page.video | relative_url }}" controls playsinline muted loop poster="{{ '/assets/projects/led-concert-sign/photo.jpg' | relative_url }}"></video>
{% else %}
{% include image_with_caption.html url="/assets/projects/led-concert-sign/photo.jpg" description="The sign on the wall, showing an upcoming show at The Fillmore" width="100%" %}
{% endif %}

An LED marquee that lists out concerts and shows at walkable SF venues. Please don't triangulate my home address.
