
# fireorm🔥

## Index

### Enumerations

* [FirestoreCollectionType](enums/firestorecollectiontype.md)
* [FirestoreOperators](enums/firestoreoperators.md)

### Classes

* [AbstractFirestoreRepository](classes/abstractfirestorerepository.md)
* [BaseFirestoreRepository](classes/basefirestorerepository.md)
* [BaseRepository](classes/baserepository.md)
* [FirestoreBatchRepository](classes/firestorebatchrepository.md)
* [MetadataStorage](classes/metadatastorage.md)
* [QueryBuilder](classes/querybuilder.md)
* [TransactionRepository](classes/transactionrepository.md)

### Interfaces

* [CollectionMetadata](interfaces/collectionmetadata.md)
* [IEntity](interfaces/ientity.md)
* [IFireOrmQueryLine](interfaces/ifireormqueryline.md)
* [IMetadataStore](interfaces/imetadatastore.md)
* [IOrderByParams](interfaces/iorderbyparams.md)
* [IQueryBuilder](interfaces/iquerybuilder.md)
* [IQueryExecutor](interfaces/iqueryexecutor.md)
* [IRepository](interfaces/irepository.md)
* [RepositoryMetadata](interfaces/repositorymetadata.md)
* [SubCollectionMetadata](interfaces/subcollectionmetadata.md)

### Type aliases

* [IFirestoreVal](globals.md#ifirestoreval)
* [IQueryBuilderResult](globals.md#iquerybuilderresult)
* [ISubCollection](globals.md#isubcollection)
* [IWherePropParam](globals.md#iwherepropparam)
* [InstanstiableIEntity](globals.md#instanstiableientity)
* [PartialBy](globals.md#partialby)
* [WithOptionalId](globals.md#withoptionalid)

### Functions

* [Collection](globals.md#collection)
* [CustomRepository](globals.md#customrepository)
* [GetBaseRepository](globals.md#getbaserepository)
* [GetCustomRepository](globals.md#getcustomrepository)
* [GetRepository](globals.md#getrepository)
* [Initialize](globals.md#const-initialize)
* [SubCollection](globals.md#subcollection)
* [getMetadataStorage](globals.md#const-getmetadatastorage)

## Type aliases

###  IFirestoreVal

Ƭ **IFirestoreVal**: *string | number | Date | Boolean*

*Defined in [types.ts:21](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L21)*

___

###  IQueryBuilderResult

Ƭ **IQueryBuilderResult**: *[IFireOrmQueryLine](interfaces/ifireormqueryline.md)[]*

*Defined in [types.ts:47](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L47)*

___

###  ISubCollection

Ƭ **ISubCollection**: *[IRepository](interfaces/irepository.md)‹T› & [IQueryBuilder](interfaces/iquerybuilder.md)‹T›*

*Defined in [types.ts:83](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L83)*

___

###  IWherePropParam

Ƭ **IWherePropParam**: *keyof T | function*

*Defined in [types.ts:49](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L49)*

___

###  InstanstiableIEntity

Ƭ **InstanstiableIEntity**: *object*

*Defined in [types.ts:90](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L90)*

#### Type declaration:

___

###  PartialBy

Ƭ **PartialBy**: *Omit‹T, K› & Partial‹Pick‹T, K››*

*Defined in [types.ts:3](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L3)*

___

###  WithOptionalId

Ƭ **WithOptionalId**: *Pick‹T, Exclude‹keyof T, "id"›› & Partial‹Pick‹T, "id"››*

*Defined in [types.ts:15](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L15)*

## Functions

###  Collection

▸ **Collection**(`entityName?`: string): *Function*

*Defined in [Decorators/Collection.ts:4](https://github.com/wovalle/fireorm/blob/da6b863/src/Decorators/Collection.ts#L4)*

**Parameters:**

Name | Type |
------ | ------ |
`entityName?` | string |

**Returns:** *Function*

___

###  CustomRepository

▸ **CustomRepository**(`entity`: [InstanstiableIEntity](globals.md#instanstiableientity)): *Function*

*Defined in [Decorators/CustomRepository.ts:4](https://github.com/wovalle/fireorm/blob/da6b863/src/Decorators/CustomRepository.ts#L4)*

**Parameters:**

Name | Type |
------ | ------ |
`entity` | [InstanstiableIEntity](globals.md#instanstiableientity) |

**Returns:** *Function*

___

###  GetBaseRepository

▸ **GetBaseRepository**<**T**>(`entity`: object, `docId?`: string, `subColName?`: string): *[BaseFirestoreRepository](classes/basefirestorerepository.md)‹T›*

*Defined in [helpers.ts:21](https://github.com/wovalle/fireorm/blob/da6b863/src/helpers.ts#L21)*

**Type parameters:**

▪ **T**: *[IEntity](interfaces/ientity.md)*

**Parameters:**

Name | Type |
------ | ------ |
`entity` | object |
`docId?` | string |
`subColName?` | string |

**Returns:** *[BaseFirestoreRepository](classes/basefirestorerepository.md)‹T›*

___

###  GetCustomRepository

▸ **GetCustomRepository**<**T**>(`entity`: object, `docId?`: string, `subColName?`: string): *[BaseFirestoreRepository](classes/basefirestorerepository.md)‹T›*

*Defined in [helpers.ts:13](https://github.com/wovalle/fireorm/blob/da6b863/src/helpers.ts#L13)*

**Type parameters:**

▪ **T**: *[IEntity](interfaces/ientity.md)*

**Parameters:**

Name | Type |
------ | ------ |
`entity` | object |
`docId?` | string |
`subColName?` | string |

**Returns:** *[BaseFirestoreRepository](classes/basefirestorerepository.md)‹T›*

___

###  GetRepository

▸ **GetRepository**<**T**>(`entity`: object, `docId?`: string, `subColName?`: string): *[BaseFirestoreRepository](classes/basefirestorerepository.md)‹T›*

*Defined in [helpers.ts:5](https://github.com/wovalle/fireorm/blob/da6b863/src/helpers.ts#L5)*

**Type parameters:**

▪ **T**: *[IEntity](interfaces/ientity.md)*

**Parameters:**

Name | Type |
------ | ------ |
`entity` | object |
`docId?` | string |
`subColName?` | string |

**Returns:** *[BaseFirestoreRepository](classes/basefirestorerepository.md)‹T›*

___

### `Const` Initialize

▸ **Initialize**(`firestore`: Firestore, `metadataStore`: [IMetadataStore](interfaces/imetadatastore.md)): *void*

*Defined in [MetadataStorage.ts:99](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L99)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`firestore` | Firestore | - |
`metadataStore` | [IMetadataStore](interfaces/imetadatastore.md) |  globalStore |

**Returns:** *void*

___

###  SubCollection

▸ **SubCollection**(`entity`: Function, `entityName?`: string): *Function*

*Defined in [Decorators/SubCollection.ts:4](https://github.com/wovalle/fireorm/blob/da6b863/src/Decorators/SubCollection.ts#L4)*

**Parameters:**

Name | Type |
------ | ------ |
`entity` | Function |
`entityName?` | string |

**Returns:** *Function*

___

### `Const` getMetadataStorage

▸ **getMetadataStorage**(): *[MetadataStorage](classes/metadatastorage.md)*

*Defined in [MetadataStorage.ts:89](https://github.com/wovalle/fireorm/blob/da6b863/src/MetadataStorage.ts#L89)*

**Returns:** *[MetadataStorage](classes/metadatastorage.md)*
