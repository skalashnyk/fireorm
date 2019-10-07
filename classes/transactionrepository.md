
# Class: TransactionRepository <**T**>

## Type parameters

▪ **T**: *[IEntity](../interfaces/ientity.md)*

## Hierarchy

  ↳ [AbstractFirestoreRepository](abstractfirestorerepository.md)‹T›

  ↳ **TransactionRepository**

## Implements

* [IQueryBuilder](../interfaces/iquerybuilder.md)‹T›
* [IQueryExecutor](../interfaces/iqueryexecutor.md)‹T›
* [IRepository](../interfaces/irepository.md)‹T›

## Index

### Constructors

* [constructor](transactionrepository.md#constructor)

### Properties

* [colMetadata](transactionrepository.md#protected-colmetadata)
* [colName](transactionrepository.md#protected-colname)
* [collection](transactionrepository.md#private-collection)
* [collectionType](transactionrepository.md#protected-collectiontype)
* [docId](transactionrepository.md#protected-docid)
* [subColMetadata](transactionrepository.md#protected-subcolmetadata)
* [subColName](transactionrepository.md#protected-subcolname)
* [transaction](transactionrepository.md#private-transaction)

### Methods

* [create](transactionrepository.md#create)
* [delete](transactionrepository.md#delete)
* [execute](transactionrepository.md#execute)
* [extractTFromColSnap](transactionrepository.md#protected-extracttfromcolsnap)
* [extractTFromDocSnap](transactionrepository.md#protected-extracttfromdocsnap)
* [find](transactionrepository.md#find)
* [findById](transactionrepository.md#findbyid)
* [initializeSubCollections](transactionrepository.md#protected-initializesubcollections)
* [limit](transactionrepository.md#limit)
* [orderByAscending](transactionrepository.md#orderbyascending)
* [orderByDescending](transactionrepository.md#orderbydescending)
* [toSerializableObject](transactionrepository.md#protected-toserializableobject)
* [transformFirestoreTypes](transactionrepository.md#protected-transformfirestoretypes)
* [update](transactionrepository.md#update)
* [whereArrayContains](transactionrepository.md#wherearraycontains)
* [whereEqualTo](transactionrepository.md#whereequalto)
* [whereGreaterOrEqualThan](transactionrepository.md#wheregreaterorequalthan)
* [whereGreaterThan](transactionrepository.md#wheregreaterthan)
* [whereLessOrEqualThan](transactionrepository.md#wherelessorequalthan)
* [whereLessThan](transactionrepository.md#wherelessthan)

## Constructors

###  constructor

\+ **new TransactionRepository**(`collection`: CollectionReference, `transaction`: Transaction, `entityConstructor`: Function): *[TransactionRepository](transactionrepository.md)*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[constructor](abstractfirestorerepository.md#constructor)*

*Defined in [BaseFirestoreTransactionRepository.ts:20](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L20)*

**Parameters:**

Name | Type |
------ | ------ |
`collection` | CollectionReference |
`transaction` | Transaction |
`entityConstructor` | Function |

**Returns:** *[TransactionRepository](transactionrepository.md)*

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

### `Private` collection

• **collection**: *CollectionReference*

*Defined in [BaseFirestoreTransactionRepository.ts:22](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L22)*

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

### `Protected` subColMetadata

• **subColMetadata**: *[SubCollectionMetadata](../interfaces/subcollectionmetadata.md)[]*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[subColMetadata](abstractfirestorerepository.md#protected-subcolmetadata)*

*Defined in [AbstractFirestoreRepository.ts:26](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L26)*

___

### `Protected` subColName

• **subColName**: *string*

*Inherited from [AbstractFirestoreRepository](abstractfirestorerepository.md).[subColName](abstractfirestorerepository.md#protected-subcolname)*

*Defined in [AbstractFirestoreRepository.ts:31](https://github.com/wovalle/fireorm/blob/da6b863/src/AbstractFirestoreRepository.ts#L31)*

___

### `Private` transaction

• **transaction**: *Transaction*

*Defined in [BaseFirestoreTransactionRepository.ts:23](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L23)*

## Methods

###  create

▸ **create**(`item`: [WithOptionalId](../globals.md#withoptionalid)‹T›): *Promise‹T›*

*Implementation of [IRepository](../interfaces/irepository.md)*

*Defined in [BaseFirestoreTransactionRepository.ts:43](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L43)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | [WithOptionalId](../globals.md#withoptionalid)‹T› |

**Returns:** *Promise‹T›*

___

###  delete

▸ **delete**(`id`: string): *Promise‹void›*

*Implementation of [IRepository](../interfaces/irepository.md)*

*Defined in [BaseFirestoreTransactionRepository.ts:74](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L74)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | string |

**Returns:** *Promise‹void›*

___

###  execute

▸ **execute**(`queries`: [IFireOrmQueryLine](../interfaces/ifireormqueryline.md)[]): *Promise‹T[]›*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[execute](abstractfirestorerepository.md#abstract-execute)*

*Defined in [BaseFirestoreTransactionRepository.ts:29](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L29)*

**Parameters:**

Name | Type |
------ | ------ |
`queries` | [IFireOrmQueryLine](../interfaces/ifireormqueryline.md)[] |

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

*Defined in [BaseFirestoreTransactionRepository.ts:38](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L38)*

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

▸ **limit**(): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[limit](abstractfirestorerepository.md#limit)*

*Defined in [BaseFirestoreTransactionRepository.ts:78](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L78)*

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

___

###  orderByAscending

▸ **orderByAscending**(): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[orderByAscending](abstractfirestorerepository.md#orderbyascending)*

*Defined in [BaseFirestoreTransactionRepository.ts:82](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L82)*

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

___

###  orderByDescending

▸ **orderByDescending**(): *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

*Overrides [AbstractFirestoreRepository](abstractfirestorerepository.md).[orderByDescending](abstractfirestorerepository.md#orderbydescending)*

*Defined in [BaseFirestoreTransactionRepository.ts:86](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L86)*

**Returns:** *[IQueryBuilder](../interfaces/iquerybuilder.md)‹T›*

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

*Defined in [BaseFirestoreTransactionRepository.ts:68](https://github.com/wovalle/fireorm/blob/da6b863/src/BaseFirestoreTransactionRepository.ts#L68)*

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
