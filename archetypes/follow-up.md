---
patient: "{{ substr .Name  17 -10 | humanize | title }}"
type: "follow-up"
date: {{ substr .Name 0 10 }}
time: "{{ replace (substr .Name 11 5) "-" ":" }}"
toc: false
---

# {{ substr .Name  17 -10 | humanize | title }}

**Date:** {{ dateFormat "2 January 2006" (substr .Name 0 10) }}, {{ replace (substr .Name 11 5) "-" ":" }}

## Notes:

