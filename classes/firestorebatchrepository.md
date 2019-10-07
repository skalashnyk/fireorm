
# Class: FirestoreBatchRepository <**T**>

## Type parameters

▪ **T**: *[IEntity](../interfaces/ientity.md)*

## Hierarchy

* **FirestoreBatchRepository**

## Index

### Constructors

* [constructor](firestorebatchrepository.md#constructor)

### Properties

* [batch](firestorebatchrepository.md#private-batch)
* [collection](firestorebatchrepository.md#private-collection)
* [serializer](firestorebatchrepository.md#private-serializer)

### Methods

* [commit](firestorebatchrepository.md#commit)
* [create](firestorebatchrepository.md#create)
* [delete](firestorebatchrepository.md#delete)
* [update](firestorebatchrepository.md#update)

## Constructors

###  constructor

\+ **new FirestoreBatchRepository**(`collection`: CollectionReference, `serializer`: Function): *[FirestoreBatchRepository](firestorebatchrepository.md)*

*Defined in [BatchFirestoreRepository.ts:7](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L7)*

**Parameters:**

Name | Type |
------ | ------ |
`collection` | CollectionReference |
`serializer` | Function |

**Returns:** *[FirestoreBatchRepository](firestorebatchrepository.md)*

## Properties

### `Private` batch

• **batch**: *WriteBatch*

*Defined in [BatchFirestoreRepository.ts:7](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L7)*

___

### `Private` collection

• **collection**: *CollectionReference*

*Defined in [BatchFirestoreRepository.ts:10](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L10)*

___

### `Private` serializer

• **serializer**: *Function*

*Defined in [BatchFirestoreRepository.ts:11](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L11)*

## Methods

###  commit

▸ **commit**(): *Promise‹WriteResult[]›*

*Defined in [BatchFirestoreRepository.ts:33](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L33)*

**Returns:** *Promise‹WriteResult[]›*

___

###  create

▸ **create**(`item`: [WithOptionalId](../globals.md#withoptionalid)‹T›): *void*

*Defined in [BatchFirestoreRepository.ts:16](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L16)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | [WithOptionalId](../globals.md#withoptionalid)‹T› |

**Returns:** *void*

___

###  delete

▸ **delete**(`item`: T): *void*

*Defined in [BatchFirestoreRepository.ts:29](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L29)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | T |

**Returns:** *void*

___

###  update

▸ **update**(`item`: T): *void*

*Defined in [BatchFirestoreRepository.ts:25](https://github.com/wovalle/fireorm/blob/da6b863/src/BatchFirestoreRepository.ts#L25)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | T |

**Returns:** *void*
