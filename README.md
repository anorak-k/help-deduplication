[![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-Ready--to--Code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/dhruvkapur91/help-deduplication)  [![Build Status](https://travis-ci.org/dhruvkapur91/help-deduplication.svg?branch=master)](https://travis-ci.org/dhruvkapur91/help-deduplication) 

Hey there, thanks for helping Syed :smiley:

So Syed learned about Set and that set does not store duplicates. Syed was super happy knowing that. Syed had a requirement of getting a list of Points, and he had to deduplicate them. It seemed like Syed found the solution! Just put them in a Set, and it'll automatically deduplicate it for him.

So he went ahead, created Point class and override the equal method. The equality worked like a charm. However much to his surprise, the set did not deduplicate the Points at all :roll_eyes: and he has a failing that he just cannot get to pass.

He verified his understanding of Set with Integers, and it worked just fine. He now wonders if Set deduplicate elements only for pre-defined or if he is doing something wrong. Can you help him pass his test? :handshake:


SOLUTION:<br>
If two objects are logically equal, then both of them should be having the same hash (which is used Sets). So, we need to override the hashcode function which generates it, along with the equals function to generate same hash.