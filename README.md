## Challenges
- False positives
  - antialias related ignore is needed, otherwise, lots noise
  - not able to ignore a section on the page is making it impossible to testing layout of page with dynamic section
- server side device detection is honored?
- friendly test writing interface & workflow?


## Features

## Desired Features

[  ] Home Page 
[ ... ] Login / Create Account
[  ] Create Account Variant & Default
[ V ] Different screen size 
[  ] independent repo from storefront
## Great to Have Features (Divert to another ticket if POC is accepted)

PDP
Checkout
## Challenging Features (Divert to another ticket if POC is accepted)

Handling of Login (Ask Brandon)
Handling of Test Account, Entries, CRUD (Ask Brandon)

# Existing Tools and references

# Findings


| Framework              | Bamboo Integration    | Github    | Support        | IngoreDom  | hot reload  | snapshot compare UI  | test scenario view    | compare with another site      | compare with history  | Development Flow   | AI Analysis  |
| ---                    | ---                   | ---       | ---            | ---        | ---         | ---                  | ---                   | ---                            | ---                   | ---                | ---          |
| Cypress                |     docker            |     x     |     good       |     x      |     v       |     external tool    |     v                 |     x                          |     v                 |     good           |     x        |
| Backstopjs             |     docker            |     x     |     very poor  |     v      |     x       |     v                |     x                 |     v                          |     x                 |     horrible       |     x        |
| Applitool              |     ?                 |     ?     |     ?          |     v      |     ?       |     v                |     x                 |     ?                          |     ?                 |     ?              |     v        |
| Jest Image Snapshot    |     v                 |     v     |     good       |     x      |     v       |     ?                |     v                 |     ?                          |     v                 |     good           |     x        |

# BackstopJS Challenge
## How to easily select specific test to run instead of whole thing in local?
  - Solution #1: build a node & react app with typescipt that parse the file and turn on a commandline app and start running?
    - can use electron app https://stackoverflow.com/questions/48702337/node-js-open-terminal-window-electron-on-mac-os
      - open terminal in app: https://stackoverflow.com/questions/52468659/electron-starting-terminal-in-main-window
## How to integrate it into CI?


# Major Blocker
- Being able to ignore certain regions within a snpahot when compare