# David Angosto git management

All commits should be significant in its content. This means that commits to temporaly save the work in progress should be squashed.
Github is used for remotes. Prefer ssh over https, except for public repositories and submoules.

## Branch strategy

Git flow is used as branch strategy, branch naming is discussed in the next section.

## Branch naming

All branches should have a keyword that states its purpose followed by a slash and name description of the branch.

All keywords are single words wrote in lower case. And it should be one of the following according to the purpose of the branch.
There are two expections: *develop* and *main*. For unit testing branches the prefix *ut* should be used; a ut branch is one that only modifies unit test source code.

### main 

* Principal branch with releases.
* No code should be committed to it, all commits should be merges of pull requests.

### develop 

* Principal branch with code in development.
* No code should be committed to it, all commits should be merges of pull requests. 

### feature/\*

* Branches that implement new source code or a new functionality.
* The name should be the class, module or functionlity that implements.
* They are created from develop and merged to it.

### staging/\*

* Branches used to create a release from develop, they may implement some bugfixing or testing, no new funcionality.
* They are created from develop and merged to main.

### bugfix/\*

* Branches that are used to solve a bug or an issue for a released code.
* They are created from main or staging and merged to it.
  

### hotfix/\*

* Branches that are used to solve a bug or an issue for a code in development.
* They are created from develop and merged to it.

### staging/\*

* Branches 
* They are created from develop and merged to main.

### doc/\*

* Branches that implement new source code or a new functionality.
* They are created from develop or main and merged to themselves.

### chore/\*

* Branches that are used for maintenance of the repository 
* They are created from develop or main and merged to themselves.


### \*/ut/\*

* Branches that implement new source code or a new functionality.
* They are created from develop and merged to it.


The text after the slash should be a short ( no more than 20 characters ) name that specify the objective of the branch.
This name should be camelCase, this means the first letter is lower case, unless it is an acronym.

Examples of valid branch names:

- hotfix/ut/newImplementation
- chore/addActions
- feature/ESP32GPIOClass

---

David Angosto