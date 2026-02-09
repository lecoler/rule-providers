# rule-providers
classical rule-providers


```yaml
rule-providers:
  Loyalsoldier-cn:
    type: http
    behavior: domain
    url: >-
      https://raw.githubusercontent.com/Loyalsoldier/clash-rules/release/direct.txt
    path: ./ruleset/direct.yaml
    interval: 86400
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
  - RULE-SET,Loyalsoldier-cn,DIRECT
```
