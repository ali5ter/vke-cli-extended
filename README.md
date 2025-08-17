> **⚠️ Archived 2025-08-16. No longer maintained.**

# vke cli-extended
[vke_wrapper](vke_wrapper) is very experimental so use at your own risk. It 
is used to to enhaunce the developer experience of the VMware Cloud PKS (formerly VKE) CLI. 

## Extensions to the Cloud PKS CLI
This wrapper provides the following features to the Cloud PKS CLI:
* ~~Remove need for the `vke folder set` and `vke project set` commands by inferring
  the folder and project name based on resource name.~~ The CLI now does this.
  :white_check_mark:
* ~~If the folder or project name can not be inferred, present the user with a list
  to select from.~~ The CLI now does this.
  :white_check_mark:
* ~~Allow the use of the 'display name' to identify a resource.~~ The CLI now does this.
  :white_check_mark:
* ~~If a resource name can not be found, present the user with a list to select from.~~ The CLI now does this.
  :white_check_mark:
* Default to latest K8s version when using `vke cluster upgrade`
* ~~Change output of `vke folder iam show`, `vke project iam show` and 
  `vke cluster iam show` to display a tree of policies, roles and identites.~~
  The CLI now does this. :white_check_mark:

## Usage
Use the wrapper by employing an alias, e.g.

    $ alias vke="$PWD/vke_wrapper"

To ignore the alias use a backslach before the command, i.e. `ke ...`

## Pre-requisites
[jq](https://stedolan.github.io/jq/download/) is used to parse JSON responses from the Cloud PKS CLI.

## Other VKE utilities
You may have use for some other VKE projects:
* [Install Cloud PKS CLI using homebrew](https://github.com/ali5ter/homebrew-vke-cli)
* [Cloud PKS CLI bash or zsh completion](https://github.com/ali5ter/vke-completion)
* [A bash Cloud PKS prompt](https://github.com/ali5ter/vke-prompt)
* [Scripts used with Cloud PKS](https://github.com/ali5ter/vmware_scripts/tree/master/vke)
