# Unraid Community Applications templates

Templates for the apps I maintain, in the layout Community Applications
expects. Registered through https://ca.unraid.net/submit, which scans this
repository and publishes what it finds.

| App | What it is | Image |
| --- | --- | --- |
| [CouchElephant](templates/couchelephant.xml) | A Plex DVR sidecar that records the live broadcast, not the repeat | `ghcr.io/datbird/couchelephant` |

## Layout

```
ca_profile.xml          who maintains this repository, shown in CA
templates/*.xml         one file per Docker app
icons/*.png             the artwork each template points at
```

Each template's `TemplateURL` is the raw URL of that exact file, which is how
CA identifies it and how an installed app picks up a corrected template.

## Changing a template

Edit the file and push. CA rebuilds its feed every few hours and takes the new
version from `TemplateURL`. Nothing has to be resubmitted.

## Licence

MIT, see [LICENSE](LICENSE). It covers the templates and metadata here. The
applications themselves carry their own licences.
