# Surge

## UK Wi-Fi Calling
For now we only have EE, Vodafone UK and Three UK tested. CMLink May also be able to use. Feel free to submit your findings.

### How to use
In your config, add `UK Operator` in `Rule-Providers` section:
```yaml
  UK Operator:
    type: http
    behavior: classical
    url: https://cdn.jsdelivr.net/gh/ous50/clash@master/wifi-calling/uk.yaml
    path: ./Rule/UK-Operator.yaml
    interval: 3600
```

Then enclose this in your `rules` section:
```yaml
  - RULE-SET,UK Operator,UK Operator
```

