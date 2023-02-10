# .github

## Profile

[Organization Profile Markdown](profile/README.md)

## Git Commit Message Specification

### Format

- **Header** (required)
- **Body** (optional)
- **Footer** (optional)

```plain text
<type>(<scope>): <subject>
\n
<body>
\n
<footer>
```

#### Header
`Header` should contain **type**(required), **scope**(optional) and **subject**(required) in one line.

##### 1. type
`type` is used to describe the type of a commit.
Several commonly used types are provided for consideration:

```text
    - feat: new feature
    - fix: fix bug
    - refactor: modifications other than features or fixes
    - release: release a new version
    - style: format or beautify code without effects on main function
    - chore: modifications of dependencies or build tools
    - docs: write documentation(e.g. README.md)
```

##### 2. scope
`scope` describes the scope of a commit, such as view layer, data layer, etc.

##### 3. subject
`subject` is a brief description of a commit and it's suggested to be limited in 50 characters.

    - start with a verb
    - end without a period

#### Body
`Body` contains more detailed explanatory text where contents could be wapped to multiple lines.

```text
feat(font-end): click affix to back to homepage

- add affix component in all detail pages
- add css styles for user interface
```

#### Footer
`Footer` is an uncommon part. When some **breaking changes** are added to a commit, it's mainly used to append descriptions, reasons and methods of migration



### Sample

```vim
commit xxxxxx
Author: xxx <xxx@winchain.com>
Date:   Tue Feb 21 18:47:17 2021 +0000

    relase: version 0.5.9

    Change-Id: xxxxxx


commit xxxxxx
Author: xxx <xxx@winchain.com>
Date:   Mon Feb 20 22:12:18 2021 +0000

    feat: Optimize some details

    1. Toggle session
    2. welcome interface modification

    Change-Id: xxxxxx


commit xxxxxx
Author: xxx <xxx@winchain.com>
Date:   Mon Feb 20 13:21:58 2021 +0000

    fix: When the sessionid acquisition fails, the websocket is not reconnected

    Change-Id: xxxxxx


commit xxxxxx
Author: xxx <xxx@winchain.com>
Date:   Tue Feb 28 11:07:25 2021 +0000

    style: Remove colors that are not in the ui spec

    Change-Id: xxxxxx
```
