---
patient: "{{ substr .Name  11 -10 | humanize | title }}"
type: "follow-up"
date: {{ substr .Name 0 10 }}
toc: false
---

# {{ substr .Name  11 -10 | humanize | title }}

**Date:** {{ dateFormat "2 January 2006" (substr .Name 0 10) }}

## Notes:

