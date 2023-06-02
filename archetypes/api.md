---
outputs: ['json', 'html']
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: false
---
