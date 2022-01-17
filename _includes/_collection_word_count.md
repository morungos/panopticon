{%- assign sections = site[include.collection] -%}
{%- assign word_count = 0 -%}
{%- for section in sections -%}
{%- assign word_count = section.content | number_of_words | plus: word_count -%}
{%- endfor -%}
{{- word_count -}}
