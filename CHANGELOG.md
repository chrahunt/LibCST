# 0.2.0 - 2019-10-04

## Added

 - Added matchers which allow comparing LibCST trees against arbitrary patterns.
 - Improved tree manipulation with `deep_remove` and `deep_replace` helper methods on CSTNode.
 - Added new metadata providers: parent node and qualified name.

## Updated

 - Updated Pyre to latest release.
 - Updated scope metadata to provide additional helpers.
 - Updated preferred method of removing a node from its parent in a visitor.

## Fixed

 - Metadata classes and methods are now exported from "libcst.metadata" instead of several submodules.
 - Fixed LICENSE file to explicitly reference individual files in the repo with different licenses.
 - Fixed `deep_clone` to correctly clone leaf nodes.
 - Fixed all parse entrypoints to always return a tree with no duplicated leaf nodes.

# 0.1.3 - 2019-09-18

## Added

 - Added preliminary support for parsing Python 3.5 and Python 3.6 source.
 - Added scope analysis metadata provider.
 - Added mypy type support for built package.

## Fixed

 - Several typos in documentation are fixed.

# 0.1.2 - 2019-08-29

## Added

 - Added attribute visitor hooks.
 - Added base visit/leave methods which can be subclassed.
 - Hypothesis fuzz testing suite, courtesy of Zac Hatfield-Dodds.

## Fixed

 - Metadata documentation is much more complete.
 - Fixed several whitespace validation issues caught by Hypothesis.
 - Parser syntax errors are now used inside parser.

# 0.1.1 - 2019-08-20

## Added

- Metadata interface is now exported.

## Fixed

- Dependencies are now specified with minimum revisions.
- Lots of documentation fixes.

# 0.1 - 2019-07-23

## Added

 - First public release of LibCST.
 - Complete, fully typed syntax tree for Python 3.6.
 - Full suite of tests for each defined node type.
