# github-class
A class in using Git and GitHub for the RobotGarden makerspace.

# Installation

Mac OS X
* Install SourceTree.

Windows
* Install SourceTree.
* Install P4Mere.

# Initial Setup

SourceTree
* In Preferences, add your name and email address.
* Change "Check default remotes for updates" to every 1 minute?
* Windows users: In Preferences > Diff tab, set P4Merge to your diff and merge tools.

Command Line
* Set your identity.

        git config --global user.name "John Doe"
        git config --global user.email johndoe@example.com

* Optionally, set your desired editor for commit messages. Examples:

        git config --global core.editor emacs
        git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -nosession"

# Getting Help

SourceTree
[SourceTree Knowledge Base](https://confluence.atlassian.com/display/SOURCETREEKB/SourceTree+Knowledge+Base+Home?continue=https%3A%2F%2Fconfluence.atlassian.com%2Fdisplay%2FSOURCETREEKB%2FSourceTree%2BKnowledge%2BBase%2BHome&application=cac)

Command Line
* `git help` or `git help command`

        rivoli:forking-test merose$ git help checkout
        
        GIT-CHECKOUT(1)                   Git Manual                   GIT-CHECKOUT(1)
        
        NAME
               git-checkout - Checkout a branch or paths to the working tree
        
        SYNOPSIS
               git checkout [-q] [-f] [-m] [<branch>]
        ...

* [Pro Git Book](https://git-scm.com/book/en/v2)

# Standalone Workflow

[Standalone workflow instructions](standalone.md)

# Forking Workflow

[Forking workflow instructions](forking.md)

# Tags

[Information on tags](tags.md)

# Notes

GitHub does not use git-flow: http://scottchacon.com/2011/08/31/github-flow.html

# License

The materials for this class are licensed under the Apache license. See the file LICENSE for details.

Copyright 2015 Mark Rose

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
