# A2LiX JS - symfony-collection

Manage your Symfony Form collection simply with vanilla JS

[![npm version](https://badge.fury.io/js/%40a2lix%2Fsymfony-collection.svg)](https://badge.fury.io/js/%40a2lix%2Fsymfony-collection)


## Install

```
yarn install @a2lix/symfony-collection     or     npm install @a2lix/symfony-collection
```


## How to

After loading the dist version of **a2lix_sf_collection.min.js** file, init a2lix_lib.sfCollection, optionnaly with custom configuration.

Default configuration:

```
a2lix_lib.sfCollection.init({
    collectionsSelector: 'form div[data-prototype]',
    manageRemoveEntry: true
})
```


## Example

```
<script src="__PATH_TO__a2lix_sf_collection.min.js"></script>

<script>
// A global initialization on all Symfony Form collection with manageRemoveEntry feature enable
a2lix_lib.sfCollection.init()


// OR a custom initialization with restricted scope of Symfony Form collection with manageRemoveEntry feature disable
a2lix_lib.sfCollection.init({
    collectionsSelector: 'form div[data-a2lix-collection]',
    manageRemoveEntry: false
})
</script>
```


## Contribute help

```
docker run -it --rm --user $(id -u):$(id -g) --name a2lix_nodejs -v "$PWD":/usr/src/app -w /usr/src/app node:alpine npm install
docker run -it --rm --user $(id -u):$(id -g) --name a2lix_nodejs -v "$PWD":/usr/src/app -w /usr/src/app node:alpine npm run build

```


# Demo

See [Demo project](https://github.com/a2lix/Demo).
