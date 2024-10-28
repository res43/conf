# L和S的区别

## 远程订阅规则
- L
  - [Remote Rule]
  - 写法`https://raw.githubusercontent.com/Cats-Team/AdRules/main/adrules.list, policy=REJECT, tag=adrules.list, enabled=true`
- S
  - [Rule]
  - 写法`RULE-SET,https://raw.githubusercontent.com/Cats-Team/AdRules/main/adrules.list,REJECT,extended-matching`
    - `DOMAIN-SET`的清单里直接是网址。
    - `RULE-SET`的清单里有`DOMAIN,`。

