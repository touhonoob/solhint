<!---
This is a dynamically generated file. Do not edit manually.
date:        Sat, 24 Aug 2019 01:45:04 GMT
author:      "Peter Chung <touhonoob@gmail.com>"
--->

# max-states-count
![Recommended Badge](https://img.shields.io/badge/-Recommended-brightgreen)
![Category Badge](https://img.shields.io/badge/-Best%20Practise%20Rules-informational)
![Default Severity Badge warn](https://img.shields.io/badge/Default%20Severity-warn-yellow)
> The {"extends": "solhint:recommended"} property in a configuration file enables this rule.


## Description
Contract has "some count" states declarations but allowed no more than maxstates.

## Options
This rule accepts an array of options:

| Index | Description                                    | Default Value |
| ----- | ---------------------------------------------- | ------------- |
| 0     | Rule severity. Must be one of "error", "warn". | warn          |
| 1     | Maximum allowed number of states declarations  | 15            |


## Examples
### 👍 Examples of **correct** code for this rule

#### Low number of states

```solidity

      pragma solidity 0.4.4;
        
        
      contract A {
                uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
        uint private constant TEST = 1;
      }
    
```

### 👎 Examples of **incorrect** code for this rule

#### High number of states

```solidity

      pragma solidity 0.4.4;
        
        
      contract A {
                uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
        uint private a;
      }
    
```

## Version
This rule was introduced in [Solhint 1.1.5](https://github.com/protofire/solhint/tree/v1.1.5)

## Resources
- [Rule source](https://github.com/protofire/solhint/tree/master/lib/rules/best-practises/max-states-count.js)
- [Document source](https://github.com/protofire/solhint/tree/master/docs/rules/best-practises/max-states-count.md)
- [Test cases](https://github.com/protofire/solhint/tree/master/test/rules/best-practises/max-states-count.js)
