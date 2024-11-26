# Surge

## UK Wi-Fi Calling
For now we only have EE, Vodafone UK and Three UK tested. CMLink May also be able to use. Feel free to submit your findings.

### How to use
In your config, add `UK Wi-Fi Calling` in `[Proxy Group]` section:
```conf
UK Wi-Fi Calling = select, DIRECT, UK
```

Then enclose this in your `[Rules]` section:
```conf
# Wi-Fi Calling
RULE-SET,https://ghp.ous50.moe/https://raw.githubusercontent.com/ous50/Surge/refs/heads/master/wifi-calling/uk.conf,UK Wi-Fi Calling
```

Remember to set `include-all-networks=true` and `include-cellular-services=true`
