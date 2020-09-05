---
patient: "{{ .Dir | path.Dir | path.Dir | path.Base | humanize | title }}"
type: "other"
description: {{ $string := split .Name "-" }}{{ $description := index $string 7 }}"{{ $description | humanize | title }}"
date:  {{ substr .Name 0 10 }}
time: "{{ replace (substr .Name 11 5) "-" ":" }}"
toc: false
---

# {{ .Dir | path.Dir | path.Dir| path.Base | humanize | title }}

**Date:** {{ dateFormat "2 January 2006" (substr .Name 0 10) }}, {{ replace (substr .Name 11 5) "-" ":" }}

## {{ $description | humanize | title }}

Insert here.
