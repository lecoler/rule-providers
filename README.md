# rule-providers
classical rule-providers


```yaml
rule-providers:
  general-cn:
    type: http
    format: yaml
    url: >-
      https://raw.githubusercontent.com/lecoler/rule-providers/master/DIRECT.yaml
    behavior: classical
    path: ./ruleset/general.yaml
    interval: 86400

rules:
  - RULE-SET,general-cn,DIRECT
```
