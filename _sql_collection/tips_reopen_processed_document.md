---
title: Reopen a processed document
layout: default
tag: Tips
lang: en
---

## Problem

Sometimes you want to open a document that you completed in a test environment.

this shows you how to do it:

### Flatrate Condition

```
update c_flatrate_conditions
set docstatus = 'DR' , processed = 'N'
where c_flatrate_conditions_id in (?);
```

