<!---
This is a dynamically generated file. Do not edit manually.
date:        Sat, 24 Aug 2019 01:45:08 GMT
author:      "Peter Chung <touhonoob@gmail.com>"
--->

# visibility-modifier-order
![Recommended Badge](https://img.shields.io/badge/-Recommended-brightgreen)
![Category Badge](https://img.shields.io/badge/-Style%20Guide%20Rules-informational)
![Default Severity Badge warn](https://img.shields.io/badge/Default%20Severity-warn-yellow)
> The {"extends": "solhint:recommended"} property in a configuration file enables this rule.


## Description
Visibility modifier must be first in list of modifiers.

## Options
This rule does not have options.

## Examples
### 👍 Examples of **correct** code for this rule

#### Visibility modifier placed first

```solidity

      pragma solidity 0.4.4;
        
        
      contract A {
        function a() public ownable() payable {}
      }
    
```

### 👎 Examples of **incorrect** code for this rule

#### Visibility modifier not placed first

```solidity

      pragma solidity 0.4.4;
        
        
      contract A {
        function a() ownable() public payable {}
      }
    
```

## Version
This rule was introduced in [Solhint 1.1.5](https://github.com/protofire/solhint/tree/v1.1.5)

## Resources
- [Rule source](https://github.com/protofire/solhint/tree/master/lib/rules/order/visibility-modifier-order.js)
- [Document source](https://github.com/protofire/solhint/tree/master/docs/rules/order/visibility-modifier-order.md)
- [Test cases](https://github.com/protofire/solhint/tree/master/test/rules/order/visibility-modifier-order.js)
