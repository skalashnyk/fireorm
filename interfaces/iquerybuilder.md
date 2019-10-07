
# Interface: IQueryBuilder <**T**>

## Type parameters

▪ **T**: *[IEntity](ientity.md)*

## Hierarchy

* **IQueryBuilder**

## Implemented by

* [AbstractFirestoreRepository](../classes/abstractfirestorerepository.md)
* [BaseFirestoreRepository](../classes/basefirestorerepository.md)
* [QueryBuilder](../classes/querybuilder.md)
* [TransactionRepository](../classes/transactionrepository.md)

## Index

### Methods

* [find](iquerybuilder.md#find)
* [limit](iquerybuilder.md#limit)
* [orderByAscending](iquerybuilder.md#orderbyascending)
* [orderByDescending](iquerybuilder.md#orderbydescending)
* [whereArrayContains](iquerybuilder.md#wherearraycontains)
* [whereEqualTo](iquerybuilder.md#whereequalto)
* [whereGreaterOrEqualThan](iquerybuilder.md#wheregreaterorequalthan)
* [whereGreaterThan](iquerybuilder.md#wheregreaterthan)
* [whereLessOrEqualThan](iquerybuilder.md#wherelessorequalthan)
* [whereLessThan](iquerybuilder.md#wherelessthan)

## Methods

###  find

▸ **find**(): *Promise‹T[]›*

*Defined in [types.ts:72](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L72)*

**Returns:** *Promise‹T[]›*

___

###  limit

▸ **limit**(`limitVal`: number): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:71](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L71)*

**Parameters:**

Name | Type |
------ | ------ |
`limitVal` | number |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  orderByAscending

▸ **orderByAscending**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:69](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L69)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  orderByDescending

▸ **orderByDescending**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:70](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L70)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  whereArrayContains

▸ **whereArrayContains**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:65](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L65)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  whereEqualTo

▸ **whereEqualTo**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:51](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L51)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  whereGreaterOrEqualThan

▸ **whereGreaterOrEqualThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:56](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L56)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  whereGreaterThan

▸ **whereGreaterThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:52](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L52)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  whereLessOrEqualThan

▸ **whereLessOrEqualThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:61](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L61)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*

___

###  whereLessThan

▸ **whereLessThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[IQueryBuilder](iquerybuilder.md)‹T›*

*Defined in [types.ts:60](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L60)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[IQueryBuilder](iquerybuilder.md)‹T›*
