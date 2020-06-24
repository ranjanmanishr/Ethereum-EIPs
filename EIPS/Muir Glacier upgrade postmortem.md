---
eip: TBD
title: Muir Glacier upgrade assessment report
author: James Hancock and Pooja Ranjan 
discussions-to: 
type: Informational
status: Draft
created: 2020-06-24
---

## Abstract

To describe the process of preparing and activating the Muir Glacier network upgrade.

## Motivation

Ethereum is growing and documentation of decisions & events that occurred during an upgrade process is extremely valuable.

## Specification

### Upgrade summary 
* Date and time (in UTC): January 02, 2020 at 08:30:49 AM UTC
* Block Number (Mainnet): 9200000
* Mined by: Spark Pool
* Block Reward: 2.04862589667520444 Ether (2 + 0.04862589667520444)
* Uncles Reward: 0
* Difficulty: 2,458,589,766,091,800
* Total Difficulty: 13,525,747,653,928,155,934,639
* Block number (Ropsten): 7117117

*Data collected from Etherscan.*

### EIP Included 

Muir Glacier had only one improvement proposal, [EIP 2384](https://eips.ethereum.org/EIPS/eip-2384). This EIP delayed the difficulty bomb for another 4,000,000 blocks so that the Ethereum chain doesn’t freeze/halt. 

* Muir Glacier Fork meta: [EIP 2387](https://eips.ethereum.org/EIPS/eip-2387) 

**Process of EIP selection**

Muir Glacier was an emergency upgrade required to address a situation which was imminent if not deployed quickly. Only one proposal was submitted, so not much of a selection was needed however developers did address relevant concerns and made appropriate adjustments for the numbers of blocks targeted to be pushed with the originally proposed EIP.

### Timeline - Backlog check

Previously, the increase in difficulty level was [predicted](https://www.reddit.com/r/ethereum/comments/4iozgf/in_around_14_month_the_difficulty_bomb_will_make/d30c0lq/) to be coming in 2021. However, the events and landmarks in the Ethereum project were developing faster, and the difficulty bomb started to show-up earlier than expected. It became noticeable again on October 5th 2019 at block 8,600,000. Block times had been around 13.1s on average and as of block 8,900,000 were around 14.3s. It was predicted to accelerate exponentially every 100,000 blocks. 

#### Discovery of problem 
* Nov 13th - First brought to the attention of the Core devs https://gitter.im/ethereum/AllCoreDevs?at=5dcc599050010612b2b1b950
* Nov 15h - ACD call [Agenda](https://github.com/ethereum/pm/issues/138), [Video](https://youtu.be/3qZFiETlDtk?t=3457)
* Nov 19th - block Time increases again - https://gitter.im/ethereum/AllCoreDevs?at=5dd4ce8050010612b2eeb9d6

#### Validation of problem
* Nov 19th - Verified it is the Difficulty Bomb https://gitter.im/ethereum/AllCoreDevs?at=5dd4e00352b73c7cb24b54a5
* Nov 20th - Confirmed https://gitter.im/ethereum/AllCoreDevs?at=5dd4ecba2c9bf5413e607488

#### Discussion & decision making 
* Nov 20th Discussed targeting Mid January
* Nov 20th - first discussion on Muir Glacier being its own fork after istanbul. - https://gitter.im/ethereum/AllCoreDevs?at=5dd542414941f9513fc23269
* Nov 20th - EIP-2384 submitted
* Nov 22nd - Hard Fork Meta submitted under name Mountain Glacier - https://gitter.im/ethereum/AllCoreDevs?at=5dd8364699dfe74c958c75f7 
* Next Core Dev Call - https://github.com/ethereum/pm/issues/140
* Nov 29th -  First Suggestion of Muir Glacier - https://gitter.im/ethereum/AllCoreDevs?at=5de12f891659720ca8ca9de9 - Real link is in the Eth Magicians forum somewhere
* Nov 29th - 7117117 Ropsten Block number Suggested. Predicted 6th of Jan https://gitter.im/ethereum/AllCoreDevs?at=5de1317ab065c6433c08cf7d
* Nov 29th - Decision to not included PoA Chains because muir glacier never activates on PoA chains -- thus have zero impact on forkid
* Nov 29th - EIP-2384 and EIP-2387 moved to [Last Call](https://github.com/ethereum/EIPs/pull/2408)
* Dec 13th - [ACD meeting 77](https://github.com/ethereum/pm/blob/master/All%20Core%20Devs%20Meetings/Meeting%2077.md) The difficulty bomb (4 mil blocks) will be addressed at some point post Muir Glacier upgrade.

#### Implementation
* Jan 02, 2020: Activation on Ethereum main network
* Jan 13, 2020: Activation on Ropsten network


### Best Practices
* Have the EF reblog content from other sources

### Suggested Corrective Action
(Problem and suggestions)

#### Ropsten Blocks being really irregular.
(TO DO)

#### There isn’t a process for checking important dates/blocks for interclient coordination. 
Suggested Solution: 
* Data Checking list
* We take turns, Two others check numbers, posting the data and the process. People from this group sign up 

#### Blocks are not predictable for timing things.
Suggested solution:
Time-Based forks.

#### Single Source of current info for main-net Variables
Suggestion Solution: 
* Getting specific information about main-net variables Take a lot of digging in the EIP repo. Difficult to do.
* The Spec as of current EIPs in a Digest

#### Ethereum RedPhone Initiative
Suggestion Solution: 
* Communicating from the CoreDevs out
* Pub/Sub model


## Rationale

An informational EIP with upgrade analysis should help in visibility and traceability of the scope of changes as well as provide an easy accessibility of historic data for community reference.

## Resources
* All Core Dev Gitter - https://gitter.im/ethereum/AllCoreDevs?at=5de7d9bf550662459868c742
* Etherscan - https://etherscan.io/block/9200000

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
