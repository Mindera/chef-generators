# chef-generators

Set of Chef generators to generate Mindera specific Chef things, like cookbooks, templates, attributes, etc, when run "chef generate X"

## Usage

1. Clone this repo to a directory
2. Reference the code_generator directory (a folder inside this repo) when using `chef` to generate a new cookbook

### Example

```
chef generate cookbook my_cookbook -g SOMEPATH/chef-generators/code_generator
```

### Defaults

The following Chef generators variables were overrided to fill the Mindera requirements:
* Name of the copyright holder - 'Mindera'
* Email address of the author - 'social@mindera.com'
* Licence - 'MIT'


## Details

At this moment this repo only provides a Cookbook generator. Based on https://github.com/chef/chef-dk/tree/master/lib/chef-dk/skeletons/code_generator it also creates Gemfile with a gem dependency to cookbook_sdk found in https://github.com/Mindera/cookbook_sdk/tree/master
