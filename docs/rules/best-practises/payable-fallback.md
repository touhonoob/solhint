<!---
This is a dynamically generated file. Do not edit manually.
date:        Sat, 24 Aug 2019 01:45:05 GMT
author:      "Peter Chung <touhonoob@gmail.com>"
--->

# payable-fallback
![Recommended Badge](https://img.shields.io/badge/-Recommended-brightgreen)
![Category Badge](https://img.shields.io/badge/-Best%20Practise%20Rules-informational)
![Default Severity Badge warn](https://img.shields.io/badge/Default%20Severity-warn-yellow)
> The {"extends": "solhint:recommended"} property in a configuration file enables this rule.


## Description
When fallback is not payable you will not be able to receive ethers.

## Options
This rule does not have options.

## Examples
### 👍 Examples of **correct** code for this rule

#### Fallback is payable

```solidity

      pragma solidity 0.4.4;
        
        
      contract A {
        function () public payable {}
      }
    
```

### 👎 Examples of **incorrect** code for this rule

#### Fallback is not payable

```solidity

      pragma solidity 0.4.4;
        
        
      contract A {
        function () public {}
      }
    
```

## Version
This rule was introduced in [Solhint 2.0.0-alpha.0](https://github.com/protofire/solhint/tree/v2.0.0-alpha.0)

## Resources
- [Rule source](https://github.com/protofire/solhint/tree/master/lib/rules/best-practises/payable-fallback.js)
- [Document source](https://github.com/protofire/solhint/tree/master/docs/rules/best-practises/payable-fallback.md)
- [Test cases](https://github.com/protofire/solhint/tree/master/test/rules/best-practises/payable-fallback.js)
