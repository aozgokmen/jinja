# jinja

###################### Filebeat Configuration Example #########################

# This file is an example configuration file highlighting only the most common
# options. The filebeat.reference.yml file from the same directory contains all the
# supported options with more comments. You can use it as a reference.
#
# You can find the full configuration reference here:
# https://www.elastic.co/guide/en/beats/filebeat/index.html

# ============================== Filebeat inputs ===============================

filebeat.inputs:

- type: log
  enabled: true
  paths:
    - {{ log_path }}
  fields:
    index: "{{ index_name }}"
  multiline.pattern: '^[[:space:]]'
  multiline.negate: false
  multiline.match: after

# ============================== Filebeat modules ==============================

filebeat.config.modules:
  # Glob pattern for configuration loading
  path: ${path.config}/modules.d/*.yml

  # Set to true to enable config reloading
  reload.enabled: false

# ======================= Elasticsearch template setting =======================
setup.ilm.enabled: false

setup.template:
  name: 'filebeat'
  pattern: 'filebeat-*'
  enabled: false
