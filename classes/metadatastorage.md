
# Class: MetadataStorage

## Hierarchy

* **MetadataStorage**

## Index

### Properties

* [collections](metadatastorage.md#collections)
* [firestoreRef](metadatastorage.md#firestoreref)
* [repositories](metadatastorage.md#repositories)
* [subCollections](metadatastorage.md#subcollections)

### Methods

* [getCollection](metadatastorage.md#getcollection)
* [getRepository](metadatastorage.md#getrepository)
* [getSubCollection](metadatastorage.md#getsubcollection)
* [getSubCollectionsFromParent](metadatastorage.md#getsubcollectionsfromparent)
* [setCollection](metadatastorage.md#setcollection)
* [setRepository](metadatastorage.md#setrepository)
* [setSubCollection](metadatastorage.md#setsubcollection)

## Properties

###  collections

• **collections**: *Array‹[CollectionMetadata](../interfaces/collectionmetadata.md)›* =  []

*Defined in [MetadataStorage.ts:29](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L29)*

___

###  firestoreRef

• **firestoreRef**: *Firestore* =  null

*Defined in [MetadataStorage.ts:86](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L86)*

___

###  repositories

• **repositories**: *Map‹unknown, [RepositoryMetadata](../interfaces/repositorymetadata.md)›* =  new Map()

*Defined in [MetadataStorage.ts:31](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L31)*

___

###  subCollections

• **subCollections**: *Array‹[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)›* =  []

*Defined in [MetadataStorage.ts:30](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L30)*

## Methods

###  getCollection

▸ **getCollection**(`param`: string | Function): *[CollectionMetadata](../interfaces/collectionmetadata.md)*

*Defined in [MetadataStorage.ts:33](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L33)*

**Parameters:**

Name | Type |
------ | ------ |
`param` | string &#124; Function |

**Returns:** *[CollectionMetadata](../interfaces/collectionmetadata.md)*

___

###  getRepository

▸ **getRepository**(`param`: Function): *[RepositoryMetadata](../interfaces/repositorymetadata.md)*

*Defined in [MetadataStorage.ts:64](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L64)*

**Parameters:**

Name | Type |
------ | ------ |
`param` | Function |

**Returns:** *[RepositoryMetadata](../interfaces/repositorymetadata.md)*

___

###  getSubCollection

▸ **getSubCollection**(`param`: string | Function): *[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)*

*Defined in [MetadataStorage.ts:51](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L51)*

**Parameters:**

Name | Type |
------ | ------ |
`param` | string &#124; Function |

**Returns:** *[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)*

___

###  getSubCollectionsFromParent

▸ **getSubCollectionsFromParent**(`parentEntity`: Function): *[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)[]*

*Defined in [MetadataStorage.ts:47](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L47)*

**Parameters:**

Name | Type |
------ | ------ |
`parentEntity` | Function |

**Returns:** *[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)[]*

___

###  setCollection

▸ **setCollection**(`col`: [CollectionMetadata](../interfaces/collectionmetadata.md)): *void*

*Defined in [MetadataStorage.ts:40](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L40)*

**Parameters:**

Name | Type |
------ | ------ |
`col` | [CollectionMetadata](../interfaces/collectionmetadata.md) |

**Returns:** *void*

___

###  setRepository

▸ **setRepository**(`repo`: [RepositoryMetadata](../interfaces/repositorymetadata.md)): *void*

*Defined in [MetadataStorage.ts:68](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L68)*

**Parameters:**

Name | Type |
------ | ------ |
`repo` | [RepositoryMetadata](../interfaces/repositorymetadata.md) |

**Returns:** *void*

___

###  setSubCollection

▸ **setSubCollection**(`subCol`: [SubCollectionMetadata](../interfaces/subcollectionmetadata.md)): *void*

*Defined in [MetadataStorage.ts:60](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L60)*

**Parameters:**

Name | Type |
------ | ------ |
`subCol` | [SubCollectionMetadata](../interfaces/subcollectionmetadata.md) |

**Returns:** *void*
