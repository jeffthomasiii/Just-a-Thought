---
layout: default
title: Just A Thought
---

![Blog Banner]({{ '/assets/images/header.jpg' | relative_url }})

# Just A Thought

Welcome to *Just A Thought* — a personal blog exploring faith, marriage, culture, technology, and the great outdoors.

Each post is a reflection in progress. Thanks for joining the journey.

“…just a thought.”


## 📝 Latest Posts

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})
<small>{{ post.date | date: "%B %-d, %Y" }}</small>

{{ post.excerpt | strip_html | truncatewords: 30 }}

{% endfor %}


### 📬 Stay Connected

🐦 [X](https://twitter.com/jeffthomasiii) | 💼 [LinkedIn](https://www.linkedin.com/in/jeffthomasiii/) | 📸 [Instagram](https://www.instagram.com/jeffthomasiii) | 🧠 [GitHub](https://github.com/jeffthomasiii)
