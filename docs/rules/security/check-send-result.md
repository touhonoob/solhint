<!---
This is a dynamically generated file. Do not edit manually.
date:        Sat, 24 Aug 2019 01:45:09 GMT
author:      "Peter Chung <touhonoob@gmail.com>"
--->

# check-send-result
![Recommended Badge](https://img.shields.io/badge/-Recommended-brightgreen)
![Category Badge](https://img.shields.io/badge/-Security%20Rules-informational)
![Default Severity Badge warn](https://img.shields.io/badge/Default%20Severity-warn-yellow)
> The {"extends": "solhint:recommended"} property in a configuration file enables this rule.


## Description
Check result of "send" call.

## Options
This rule does not have options.

## Examples
### 👍 Examples of **correct** code for this rule

#### result of "send" call checked with if statement

```solidity
if(x.send(55)) {}
```

### 👎 Examples of **incorrect** code for this rule

#### result of "send" call ignored

```solidity
x.send(55);
```

## Version
This rule was introduced in [Solhint 2.0.0-alpha.0](https://github.com/protofire/solhint/tree/v2.0.0-alpha.0)

## Resources
- [Rule source](https://github.com/protofire/solhint/tree/master/lib/rules/security/check-send-result.js)
- [Document source](https://github.com/protofire/solhint/tree/master/docs/rules/security/check-send-result.md)
- [Test cases](https://github.com/protofire/solhint/tree/master/test/rules/security/check-send-result.js)
