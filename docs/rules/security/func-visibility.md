<!---
This is a dynamically generated file. Do not edit manually.
date:        Sat, 24 Aug 2019 01:45:09 GMT
author:      "Peter Chung <touhonoob@gmail.com>"
--->

# func-visibility
![Recommended Badge](https://img.shields.io/badge/-Recommended-brightgreen)
![Category Badge](https://img.shields.io/badge/-Security%20Rules-informational)
![Default Severity Badge warn](https://img.shields.io/badge/Default%20Severity-warn-yellow)
> The {"extends": "solhint:recommended"} property in a configuration file enables this rule.


## Description
Explicitly mark visibility in function.

## Options
This rule does not have options.

## Examples
### 👍 Examples of **correct** code for this rule

#### Functions explicitly marked with visibility

```solidity
function b() internal { }
function b() external { }
function b() private { }
function b() public { }
```

### 👎 Examples of **incorrect** code for this rule

#### Functions without explicitly marked visibility

```solidity
function b() { }
```

## Version
This rule was introduced in [Solhint 2.0.0-alpha.0](https://github.com/protofire/solhint/tree/v2.0.0-alpha.0)

## Resources
- [Rule source](https://github.com/protofire/solhint/tree/master/lib/rules/security/func-visibility.js)
- [Document source](https://github.com/protofire/solhint/tree/master/docs/rules/security/func-visibility.md)
- [Test cases](https://github.com/protofire/solhint/tree/master/test/rules/security/func-visibility.js)
