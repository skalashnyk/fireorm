
# Interface: IRepository <**T**>

## Type parameters

▪ **T**: *object*

## Hierarchy

* **IRepository**

## Implemented by

* [BaseFirestoreRepository](../classes/basefirestorerepository.md)
* [TransactionRepository](../classes/transactionrepository.md)

## Index

### Methods

* [create](irepository.md#create)
* [delete](irepository.md#delete)
* [findById](irepository.md#findbyid)
* [limit](irepository.md#limit)
* [orderByAscending](irepository.md#orderbyascending)
* [orderByDescending](irepository.md#orderbydescending)
* [update](irepository.md#update)

## Methods

###  create

▸ **create**(`item`: [PartialBy](../globals.md#partialby)‹T, "id"›): *Promise‹T›*

*Defined in [types.ts:10](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L10)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | [PartialBy](../globals.md#partialby)‹T, "id"› |

**Returns:** *Promise‹T›*

___

###  delete

▸ **delete**(`id`: string): *Promise‹void›*

*Defined in [types.ts:12](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L12)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | string |

**Returns:** *Promise‹void›*

___

###  findById

▸ **findById**(`id`: string): *Promise‹T›*

*Defined in [types.ts:9](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L9)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | string |

**Returns:** *Promise‹T›*

___

###  limit

▸ **limit**(`limitVal`: number): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:6](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L6)*

**Parameters:**

Name | Type |
------ | ------ |
`limitVal` | number |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  orderByAscending

▸ **orderByAscending**(`prop`: keyof T & string): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:7](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L7)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | keyof T & string |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  orderByDescending

▸ **orderByDescending**(`prop`: keyof T & string): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:8](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L8)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | keyof T & string |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  update

▸ **update**(`item`: T): *Promise‹T›*

*Defined in [types.ts:11](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L11)*

**Parameters:**

Name | Type |
------ | ------ |
`item` | T |

**Returns:** *Promise‹T›*
