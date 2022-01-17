> This is a work in progress, not even a draft. Please do not use it or cite it
> as it stands, at least, 
> [not without checking with me first](mailto:morungos@gmail.com). My goal is to 
> complete this by summer 2022, and if you'd like to 
> [buy me a coffee](https://www.buymeacoffee.com/morungos) to assist
> my thinking process, I will be extremely grateful and name you as a supporter. 
> And comments and feedback
> will always be welcome, particularly if you disagree, have data, evidence,
> or references I can use.

## Table of contents

- [*Introduction*]({{ "/introduction" | relative_url }}) - {% include _collection_word_count.md collection="front-matter" %} words
- [1\. A Postmodern Panopticon]({{ "/chapter-01" | relative_url }}) - {% include _collection_word_count.md collection="chapter-01" %} words
- 2\. A Precession of Simulacra
- 3\. Creative Destruction
- 4\. Artificial Intelligence
- 5\. The Office Landscape
- 6\. Politics
- 7\. Crime, Money, and Property
- 8\. Learning
- 9\. Health
- 10\. Outside the Panopticon
{: .table-of-contents}

* * *

{% assign total_word_count = 0 %}
{% for collection in site.collections %}
{% capture word_count %}{% include _collection_word_count.md collection=collection.label %}{% endcapture %}
{% assign total_word_count = word_count | plus: total_word_count %}
{% endfor %}

Total word count: {{ total_word_count }}  
Last updated: {{ site.time | date_to_string: "ordinal", "US" }}
