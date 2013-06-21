Menu Item Semver
================

##### A list of semver rules for menu items in a restaurant.



1. Menu items using Semantic Versioning MUST declare a list of ingredients. These items could be declared in the menu itself or in a separate appendix document available on request. Menu items MAY be assigned a type category to aid with deciding (breakfast, dinner, soup, tapas). Menu items MAY include OPTIONAL recipe details to aid in the pre-ordering process of a patron.

2. As with software Semver, a normal menu item version number MUST take the form X.Y.Z where X, Y, and Z are non-negative integers, and MUST NOT contain leading zeroes. X is the major version, Y is the minor version, and Z is the patch version. Each element MUST increase numerically. For instance: 1.9.0 -> 1.10.0 -> 1.11.0.

3. Once a versioned menu item has been printed, the ingredients of that version MUST NOT be modified. Any modifications MUST be released as a new version. The OPTIONAL category can be modified without releasing a new version, assuming this does not add, remove, or change any of the item's existing ingredients.

4. Major version zero (0.y.z) is for initial development of the dish. Anything may change at any time, including ingredients, source of ingredients, and recipe. These should not be considered consistent, and the menu item category may be inaccurate or undecided.

5. Version 1.0.0 defines a complete list of ingredients. Version 1.0.0 also MUST NOT change the recipe, regardless of if the recipe is publicly provided.  The way in which the version number is incremented after this release is dependent on how the ingredients and recipe changes. 

6. Patch version Z (x.y.Z | x > 0) MUST be incremented if only alternately sourced but otherwise identical ingredients are introduced. An ingredient is defined as any consumable item used in the construction of the menu-item which may impact its flavor, consistency, or texture.

7. Minor version Y (x.Y.z | x > 0) MUST be incremented if either an ingredient stays consistent but its cultivar or variety is changed (for example, switching from Roma to Santorini tomatoes), and/or if the recipe's process is modified but does not include addition or removal of steps (for example, changing a sauce's simmer time from 10 to 20 minutes to slightly change its consistency).

8. Major version X (X.y.z | X > 0) MUST be incremented if the menu item's ingredients or recipe are changed. It MAY include minor and patch level changes. Patch and minor version MUST be reset to 0 when major version is incremented.

10. Items 9-11 from [semver.org](http://semver.org) do not change.
