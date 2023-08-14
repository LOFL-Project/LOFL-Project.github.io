---
layout: page
title: APIs
---

Currently, data from LOFLCAB can be accessed in the following ways:

## JSON
**Entry point**: <a href="{{'/api/loflcab.json' | relative_url }}">{{'/api/loflcab.json' | relative_url}}</a>

**Type**: Single file

This file contains every LOFLCAB entry in a single file, using the same structure as the underlying YAML files.

## CSV
**Entry point**: <a href="{{'/api/loflcab.csv' | relative_url }}">{{'/api/loflcab.csv' | relative_url}}</a>

**Type**: Single file

This file contains every LOFLCAB entry in a single file, broken down by LOFLCAB and command.

## YAML
**Type**: File per entry

Finally, it is possible to access the raw YAML files via GitHub. The file structure can be found on <a href="https://github.com/LOFLCAB/LOFLCAB/tree/master/yml">GitHub</a>.
