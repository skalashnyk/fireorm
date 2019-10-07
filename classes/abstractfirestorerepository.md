
# Class: AbstractFirestoreRepository <**T**>

## Type parameters

▪ **T**: *[IEntity](../interfaces/ientity.md)*

## Hierarchy

* [BaseRepository](baserepository.md)

  ↳ **AbstractFirestoreRepository**

  ↳ [TransactionRepository](transactionrepository.md)

  ↳ [BaseFirestoreRepository](basefirestorerepository.md)

## Implements

* [IQueryBuilder](../interfaces/iquerybuilder.md)‹T›
* [IQueryExecutor](../interfaces/iqueryexecutor.md)‹T›

## Index

### Constructors

* [constructor](abstractfirestorerepository.md#constructor)

### Properties

* [colMetadata](abstractfirestorerepository.md#protected-colmetadata)
* [colName](abstractfirestorerepository.md#protected-colname)
* [collectionType](abstractfirestorerepository.md#protected-collectiontype)
* [docId](abstractfirestorerepository.md#protected-docid)
* [subColMetadata](abstractfirestorerepository.md#protected-subcolmetadata)
* [subColName](abstractfirestorerepository.md#protected-subcolname)

### Methods

* [execute](abstractfirestorerepository.md#abstract-execute)
* [extractTFromColSnap](abstractfirestorerepository.md#protected-extracttfromcolsnap)
* [extractTFromDocSnap](abstractfirestorerepository.md#protected-extracttfromdocsnap)
* [find](abstractfirestorerepository.md#find)
* [initializeSubCollections](abstractfirestorerepository.md#protected-initializesubcollections)
* [limit](abstractfirestorerepository.md#limit)
* [orderByAscending](abstractfirestorerepository.md#orderbyascending)
* [orderByDescending](abstractfirestorerepository.md#orderbydescending)
* [toSerializableObject](abstractfirestorerepository.md#protected-toserializableobject)
* [transformFirestoreTypes](abstractfirestorerepository.md#protected-transformfirestoretypes)
* [whereArrayContains](abstractfirestorerepository.md#wherearraycontains)
* [whereEqualTo](abstractfirestorerepository.md#whereequalto)
* [whereGreaterOrEqualThan](abstractfirestorerepository.md#wheregreaterorequalthan)
* [whereGreaterThan](abstractfirestorerepository.md#wheregreaterthan)
* [whereLessOrEqualThan](abstractfirestorerepository.md#wherelessorequalthan)
* [whereLessThan](abstractfirestorerepository.md#wherelessthan)

## Constructors

###  constructor

\+ **new AbstractFirestoreRepository**(`nameOrConstructor`: string | Function, `docId?`: string, `subColName?`: string): *[AbstractFirestoreRepository](abstractfirestorerepository.md)*

*Defined in [AbstractFirestoreRepository.ts:31](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L31)*

**Parameters:**

Name | Type |
------ | ------ |
`nameOrConstructor` | string &#124; Function |
`docId?` | string |
`subColName?` | string |

**Returns:** *[AbstractFirestoreRepository](abstractfirestorerepository.md)*

## Properties

### `Protected` colMetadata

• **colMetadata**: *[CollectionMetadata](../interfaces/collectionmetadata.md)*

*Defined in [AbstractFirestoreRepository.ts:27](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L27)*

___

### `Protected` colName

• **colName**: *string*

*Defined in [AbstractFirestoreRepository.ts:29](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L29)*

___

### `Protected` collectionType

• **collectionType**: *[FirestoreCollectionType](../enums/firestorecollectiontype.md)*

*Defined in [AbstractFirestoreRepository.ts:28](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L28)*

___

### `Protected` docId

• **docId**: *string*

*Defined in [AbstractFirestoreRepository.ts:30](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L30)*

___

### `Protected` subColMetadata

• **subColMetadata**: *[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)[]*

*Defined in [AbstractFirestoreRepository.ts:26](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L26)*

___

### `Protected` subColName

• **subColName**: *string*

*Defined in [AbstractFirestoreRepository.ts:31](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L31)*

## Methods

### `Abstract` execute

▸ **execute**(`queries`: [IFireOrmQueryLine](../interfaces/ifireormqueryline.md)[], `limitVal?`: number, `orderByObj?`: [IOrderByParams](../interfaces/iorderbyparams.md)): *Promise‹T[]›*

*Implementation of [IQueryExecutor](../interfaces/iqueryexecutor.md)*

*Defined in [AbstractFirestoreRepository.ts:297](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L297)*

Takes all the queries stored by QueryBuilder and executes them.
Must be implemented by base repositores

**`abstract`** 

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`queries` | [IFireOrmQueryLine](../interfaces/ifireormqueryline.md)[] | list of queries stored in QueryBuilder |
`limitVal?` | number | - |
`orderByObj?` | [IOrderByParams](../interfaces/iorderbyparams.md) | - |

**Returns:** *Promise‹T[]›*

results from firestore converted into
entities <T>

___

### `Protected` extractTFromColSnap

▸ **extractTFromColSnap**(`q`: QuerySnapshot): *T[]*

*Defined in [AbstractFirestoreRepository.ts:114](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L114)*

**Parameters:**

Name | Type |
------ | ------ |
`q` | QuerySnapshot |

**Returns:** *T[]*

___

### `Protected` extractTFromDocSnap

▸ **extractTFromDocSnap**(`doc`: DocumentSnapshot): *T*

*Defined in [AbstractFirestoreRepository.ts:99](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L99)*

**Parameters:**

Name | Type |
------ | ------ |
`doc` | DocumentSnapshot |

**Returns:** *T*

___

###  find

▸ **find**(): *Promise‹T[]›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:278](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L278)*

Execute the query and applies all the filters (if specified)

**`memberof`** AbstractFirestoreRepository

**Returns:** *Promise‹T[]›*

List of documents that matched the filters
(if specified)

___

### `Protected` initializeSubCollections

▸ **initializeSubCollections**(`entity`: T): *void*

*Defined in [AbstractFirestoreRepository.ts:84](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L84)*

**Parameters:**

Name | Type |
------ | ------ |
`entity` | T |

**Returns:** *void*

___

###  limit

▸ **limit**(`limitVal`: number): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:233](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L233)*

Returns a new QueryBuilder with a maximum number of results
to return. Can only be used once per query.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`limitVal` | number | maximum number of results to return Must be greater or equal than 0 |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

QueryBuilder A new QueryBuilder with
the specified limit applied

___

###  orderByAscending

▸ **orderByAscending**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:253](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L253)*

Returns a new QueryBuilder with an additional ascending order
specified by @param prop. Can only be used once per query.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be ordered on, where prop could be keyof T or a lambda where T is the first parameter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
ordering applied.

___

###  orderByDescending

▸ **orderByDescending**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:267](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L267)*

Returns a new QueryBuilder with an additional descending order
specified by @param prop. Can only be used once per query.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be ordered on, where prop could be keyof T or a lambda where T is the first parameter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
ordering applied.

___

### `Protected` toSerializableObject

▸ **toSerializableObject**(`obj`: T): *Object*

*Defined in [AbstractFirestoreRepository.ts:62](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L62)*

**Parameters:**

Name | Type |
------ | ------ |
`obj` | T |

**Returns:** *Object*

___

### `Protected` transformFirestoreTypes

▸ **transformFirestoreTypes**(`obj`: T): *T*

*Defined in [AbstractFirestoreRepository.ts:69](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L69)*

**Parameters:**

Name | Type |
------ | ------ |
`obj` | T |

**Returns:** *T*

___

###  whereArrayContains

▸ **whereArrayContains**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:216](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L216)*

Returns a new QueryBuilder with a filter specifying that the
value in @param val must be contained in @param prop.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be filtered on, where prop could be keyof T or a lambda where T is the first parameter |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) | value to compare in the filter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
query applied.

___

###  whereEqualTo

▸ **whereEqualTo**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:129](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L129)*

Returns a new QueryBuilder with a filter specifying that the
value in @param prop must be equal to @param val.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be filtered on, where prop could be keyof T or a lambda where T is the first parameter |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) | value to compare in the filter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
query applied.

___

###  whereGreaterOrEqualThan

▸ **whereGreaterOrEqualThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:162](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L162)*

Returns a new QueryBuilder with a filter specifying that the
value in @param prop must be greater or equal than @param val.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be filtered on, where prop could be keyof T or a lambda where T is the first parameter |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) | value to compare in the filter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
query applied.

___

###  whereGreaterThan

▸ **whereGreaterThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:144](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L144)*

Returns a new QueryBuilder with a filter specifying that the
value in @param prop must be greater than @param val.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be filtered on, where prop could be keyof T or a lambda where T is the first parameter |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) | value to compare in the filter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
query applied.

___

###  whereLessOrEqualThan

▸ **whereLessOrEqualThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:198](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L198)*

Returns a new QueryBuilder with a filter specifying that the
value in @param prop must be less or equal than @param val.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be filtered on, where prop could be keyof T or a lambda where T is the first parameter |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) | value to compare in the filter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
query applied.

___

###  whereLessThan

▸ **whereLessThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [AbstractFirestoreRepository.ts:180](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L180)*

Returns a new QueryBuilder with a filter specifying that the
value in @param prop must be less than @param val.

**`memberof`** AbstractFirestoreRepository

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› | field to be filtered on, where prop could be keyof T or a lambda where T is the first parameter |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) | value to compare in the filter |

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

A new QueryBuilder with the specified
query applied.
