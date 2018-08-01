# vke cli-extended
[vke_wrapper](vke_wrapper) is very experimental so use at your own risk. It 
is used to add features in an attempt to enhaunce the developer experience of
the VKE CLI. 

## Extensions to the VKE CLI
This wrapper provides the following enhauncements:
* Remove need for the `vke folder set` and `vke project set` commands by inferring
  the folder and project name based on resource name.
* If the folder or project name can not be inferred, present the user with a list
  to select from.
* Allow the use of the 'display name' to identify a resource.
* If a resource name can not be found, present the user with a list to select from.
* Default to latest K8s version when using `vke cluster upgrade`
* View IAM Policies for a cluster as a tree

## Usage
Use the wrapper by employing an alias, e.g.

    $ alias vke="$PWD/vke_wrapper"

To ignore the alias use a backslach before the command, i.e. `\vke ...`

## Pre-requisites
[jq](https://stedolan.github.io/jq/download/) is used to parse JSON responses from the VKE CLI.

## Other VKE utilities
You may have use for some other VKE projects:
* [Install VKE CLI using homebrew](https://github.com/ali5ter/homebrew-vke)
* [VKE CLI bash or zsh completion](https://github.com/ali5ter/vke-completion)
* [A bash VKE prompt](https://github.com/ali5ter/vke-prompt)
* [Scripts used with VKE](https://github.com/ali5ter/vmware_scripts/tree/master/vke)
