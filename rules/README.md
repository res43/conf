# L和S的区别

## 远程订阅规则
- L
  - [Remote Rule]
  - 写法`https://raw.githubusercontent.com/Cats-Team/AdRules/main/adrules.list, policy=REJECT, tag=adrules.list, enabled=true`
- S
  - [Rule]
  - 写法`RULE-SET,https://raw.githubusercontent.com/Cats-Team/AdRules/main/adrules.list,REJECT,extended-matching`
    - `DOMAIN-SET`的清单里直接是网址。仅可使用 DOMAIN 和 DOMAIN-SUFFIX 两种形式的内容。使用了特别的逻辑进行优化，在内容非常多（千条以上）时性能有极大的提升。
    - `RULE-SET`的清单里有`DOMAIN,`。可包含所有类型的子规则，执行效率和在主配置中的规则没有区别

