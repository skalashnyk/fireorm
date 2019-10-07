
# Class: BaseFirestoreRepository <**T**>

## Type parameters

▪ **T**: *[IEntity](../interfaces/ientity.md)*

## Hierarchy

  ↳ [AbstractFirestoreRepository](abstractfirestorerepository.md)‹T›

  ↳ **BaseFirestoreRepository**

## Implements

* [IQueryBuilder](../interfaces/iquerybuilder.md)‹T›
* [IQueryExecutor](../interfaces/iqueryexecutor.md)‹T›
* [IRepository](../interfaces/irepository.md)‹T›

## Index

### Constructors

* [constructor](basefirestorerepository.md#constructor)

### Properties

* [colMetadata](basefirestorerepository.md#protected-colmetadata)
* [colName](basefirestorerepository.md#protected-colname)
* [collectionType](basefirestorerepository.md#protected-collectiontype)
* [docId](basefirestorerepository.md#protected-docid)
* [firestoreColRef](basefirestorerepository.md#private-firestorecolref)
* [subColMetadata](basefirestorerepository.md#protected-subcolmetadata)
* [subColName](basefirestorerepository.md#protected-subcolname)

### Methods

* [create](basefirestorerepository.md#create)
* [createBatch](basefirestorerepository.md#createbatch)
* [delete](basefirestorerepository.md#delete)
* [execute](basefirestorerepository.md#execute)
* [extractTFromColSnap](basefirestorerepository.md#protected-extracttfromcolsnap)
* [extractTFromDocSnap](basefirestorerepository.md#protected-extracttfromdocsnap)
* [find](basefirestorerepository.md#find)
* [findById](basefirestorerepository.md#findbyid)
* [initializeSubCollections](basefirestorerepository.md#protected-initializesubcollections)
* [limit](basefirestorerepository.md#limit)
* [orderByAscending](basefirestorerepository.md#orderbyascending)
* [orderByDescending](basefirestorerepository.md#orderbydescending)
* [runTransaction](basefirestorerepository.md#runtransaction)
* [toSerializableObject](basefirestorerepository.md#protected-toserializableobject)
* [transformFirestoreTypes](basefirestorerepository.md#protected-transformfirestoretypes)
* [update](basefirestorerepository.md#update)
* [whereArrayContains](basefirestorerepository.md#wherearraycontains)
* [whereEqualTo](basefirestorerepository.md#whereequalto)
* [whereGreaterOrEqualThan](basefirestorerepository.md#wheregreaterorequalthan)
* [whereGreaterThan](basefirestorerepository.md#wheregreaterthan)
* [whereLessOrEqualThan](basefirestorerepository.md#wherelessorequalthan)
* [whereLessThan](basefirestorerepository.md#wherelessthan)

## Constructors

###  constructor

\+ **new BaseFirestoreRepository**(`colName`: string): *[BaseFirestoreRepository](basefirestorerepository.md)*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[constructor](abstractfirestorerepository.md#constructor)*

*Defined in [BaseFirestoreRepository.ts:22](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L22)*

**Parameters:**

Name | Type |
------ | ------ |
`colName` | string |

**Returns:** *[BaseFirestoreRepository](basefirestorerepository.md)*

\+ **new BaseFirestoreRepository**(`colName`: string, `docId`: string, `subColName`: string): *[BaseFirestoreRepository](basefirestorerepository.md)*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[constructor](abstractfirestorerepository.md#constructor)*

*Defined in [BaseFirestoreRepository.ts:24](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L24)*

**Parameters:**

Name | Type |
------ | ------ |
`colName` | string |
`docId` | string |
`subColName` | string |

**Returns:** *[BaseFirestoreRepository](basefirestorerepository.md)*

## Properties

### `Protected` colMetadata

• **colMetadata**: *[CollectionMetadata](../interfaces/collectionmetadata.md)*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[colMetadata](abstractfirestorerepository.md#protected-colmetadata)*

*Defined in [AbstractFirestoreRepository.ts:27](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L27)*

___

### `Protected` colName

• **colName**: *string*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[colName](abstractfirestorerepository.md#protected-colname)*

*Defined in [AbstractFirestoreRepository.ts:29](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L29)*

___

### `Protected` collectionType

• **collectionType**: *[FirestoreCollectionType](../enums/firestorecollectiontype.md)*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[collectionType](abstractfirestorerepository.md#protected-collectiontype)*

*Defined in [AbstractFirestoreRepository.ts:28](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L28)*

___

### `Protected` docId

• **docId**: *string*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[docId](abstractfirestorerepository.md#protected-docid)*

*Defined in [AbstractFirestoreRepository.ts:30](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L30)*

___

### `Private` firestoreColRef

• **firestoreColRef**: *CollectionReference*

*Defined in [BaseFirestoreRepository.ts:22](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L22)*

___

### `Protected` subColMetadata

• **subColMetadata**: *[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)[]*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[subColMetadata](abstractfirestorerepository.md#protected-subcolmetadata)*

*Defined in [AbstractFirestoreRepository.ts:26](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L26)*

___

### `Protected` subColName

• **subColName**: *string*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[subColName](abstractfirestorerepository.md#protected-subcolname)*

*Defined in [AbstractFirestoreRepository.ts:31](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L31)*

## Methods

###  create

▸ **create**(`item`: T): *Promise‹T›*

*Defined in [BaseFirestoreRepository.ts:52](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L52)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | T |

**Returns:** *Promise‹T›*

___

###  createBatch

▸ **createBatch**(): *[FirestoreBatchRepository](firestorebatchrepository.md)‹[IEntity](../interfaces/ientity.md)›*

*Defined in [BaseFirestoreRepository.ts:104](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L104)*

**Returns:** *[FirestoreBatchRepository](firestorebatchrepository.md)‹[IEntity](../interfaces/ientity.md)›*

___

###  delete

▸ **delete**(`id`: string): *Promise‹void›*

*Implementation of [IRepository](../interfaces/irepository.md)*

*Defined in [BaseFirestoreRepository.ts:87](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L87)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | string |

**Returns:** *Promise‹void›*

___

###  execute

▸ **execute**(`queries`: Array‹[IFireOrmQueryLine](../interfaces/ifireormqueryline.md)›, `limitVal?`: number, `orderByObj?`: [IOrderByParams](../interfaces/iorderbyparams.md)): *Promise‹T[]›*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[execute](abstractfirestorerepository.md#abstract-execute)*

*Defined in [BaseFirestoreRepository.ts:111](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L111)*

**Parameters:**

Name | Type |
------ | ------ |
`queries` | Array‹[IFireOrmQueryLine](../interfaces/ifireormqueryline.md)› |
`limitVal?` | number |
`orderByObj?` | [IOrderByParams](../interfaces/iorderbyparams.md) |

**Returns:** *Promise‹T[]›*

___

### `Protected` extractTFromColSnap

▸ **extractTFromColSnap**(`q`: QuerySnapshot): *T[]*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md)*

*Defined in [AbstractFirestoreRepository.ts:114](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L114)*

**Parameters:**

Name | Type |
------ | ------ |
`q` | QuerySnapshot |

**Returns:** *T[]*

___

### `Protected` extractTFromDocSnap

▸ **extractTFromDocSnap**(`doc`: DocumentSnapshot): *T*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[find](abstractfirestorerepository.md#find)*

*Defined in [AbstractFirestoreRepository.ts:278](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L278)*

Execute the query and applies all the filters (if specified)

**`memberof`** AbstractFirestoreRepository

**Returns:** *Promise‹T[]›*

List of documents that matched the filters
(if specified)

___

###  findById

▸ **findById**(`id`: string): *Promise‹T›*

*Implementation of [IRepository](../interfaces/irepository.md)*

*Defined in [BaseFirestoreRepository.ts:45](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L45)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | string |

**Returns:** *Promise‹T›*

___

### `Protected` initializeSubCollections

▸ **initializeSubCollections**(`entity`: T): *void*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md)*

*Defined in [AbstractFirestoreRepository.ts:84](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L84)*

**Parameters:**

Name | Type |
------ | ------ |
`entity` | T |

**Returns:** *void*

___

###  limit

▸ **limit**(`limitVal`: number): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IRepository](../interfaces/irepository.md)*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[limit](abstractfirestorerepository.md#limit)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[orderByAscending](abstractfirestorerepository.md#orderbyascending)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[orderByDescending](abstractfirestorerepository.md#orderbydescending)*

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

###  runTransaction

▸ **runTransaction**(`executor`: function): *Promise‹void›*

*Defined in [BaseFirestoreRepository.ts:92](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L92)*

**Parameters:**

▪ **executor**: *function*

▸ (`tran`: [TransactionRepository](transactionrepository.md)‹T›): *Promise‹void›*

**Parameters:**

Name | Type |
------ | ------ |
`tran` | [TransactionRepository](transactionrepository.md)‹T› |

**Returns:** *Promise‹void›*

___

### `Protected` toSerializableObject

▸ **toSerializableObject**(`obj`: T): *Object*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md)*

*Defined in [AbstractFirestoreRepository.ts:62](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L62)*

**Parameters:**

Name | Type |
------ | ------ |
`obj` | T |

**Returns:** *Object*

___

### `Protected` transformFirestoreTypes

▸ **transformFirestoreTypes**(`obj`: T): *T*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md)*

*Defined in [AbstractFirestoreRepository.ts:69](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L69)*

**Parameters:**

Name | Type |
------ | ------ |
`obj` | T |

**Returns:** *T*

___

###  update

▸ **update**(`item`: T): *Promise‹T›*

*Defined in [BaseFirestoreRepository.ts:79](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreRepository.ts#L79)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | T |

**Returns:** *Promise‹T›*

___

###  whereArrayContains

▸ **whereArrayContains**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[whereArrayContains](abstractfirestorerepository.md#wherearraycontains)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[whereEqualTo](abstractfirestorerepository.md#whereequalto)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[whereGreaterOrEqualThan](abstractfirestorerepository.md#wheregreaterorequalthan)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[whereGreaterThan](abstractfirestorerepository.md#wheregreaterthan)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[whereLessOrEqualThan](abstractfirestorerepository.md#wherelessorequalthan)*

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

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[whereLessThan](abstractfirestorerepository.md#wherelessthan)*

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
