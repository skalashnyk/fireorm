
# Class: QueryBuilder <**T**>

## Type parameters

▪ **T**: *[IEntity](../interfaces/ientity.md)*

## Hierarchy

* **QueryBuilder**

## Implements

* [IQueryBuilder](../interfaces/iquerybuilder.md)‹T›

## Index

### Constructors

* [constructor](querybuilder.md#constructor)

### Properties

* [executor](querybuilder.md#protected-executor)
* [limitVal](querybuilder.md#protected-limitval)
* [orderByObj](querybuilder.md#protected-orderbyobj)
* [queries](querybuilder.md#protected-queries)

### Methods

* [extractWhereParam](querybuilder.md#private-extractwhereparam)
* [find](querybuilder.md#find)
* [limit](querybuilder.md#limit)
* [orderByAscending](querybuilder.md#orderbyascending)
* [orderByDescending](querybuilder.md#orderbydescending)
* [whereArrayContains](querybuilder.md#wherearraycontains)
* [whereEqualTo](querybuilder.md#whereequalto)
* [whereGreaterOrEqualThan](querybuilder.md#wheregreaterorequalthan)
* [whereGreaterThan](querybuilder.md#wheregreaterthan)
* [whereLessOrEqualThan](querybuilder.md#wherelessorequalthan)
* [whereLessThan](querybuilder.md#wherelessthan)

## Constructors

###  constructor

\+ **new QueryBuilder**(`executor`: [IQueryExecutor](../interfaces/iqueryexecutor.md)‹T›): *[QueryBuilder](querybuilder.md)*

*Defined in [QueryBuilder.ts:18](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L18)*

**Parameters:**

Name | Type |
------ | ------ |
`executor` | [IQueryExecutor](../interfaces/iqueryexecutor.md)‹T› |

**Returns:** *[QueryBuilder](querybuilder.md)*

## Properties

### `Protected` executor

• **executor**: *[IQueryExecutor](../interfaces/iqueryexecutor.md)‹T›*

*Defined in [QueryBuilder.ts:20](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L20)*

___

### `Protected` limitVal

• **limitVal**: *number*

*Defined in [QueryBuilder.ts:17](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L17)*

___

### `Protected` orderByObj

• **orderByObj**: *[IOrderByParams](../interfaces/iorderbyparams.md)*

*Defined in [QueryBuilder.ts:18](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L18)*

___

### `Protected` queries

• **queries**: *Array‹[IFireOrmQueryLine](../interfaces/ifireormqueryline.md)›* =  []

*Defined in [QueryBuilder.ts:16](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L16)*

## Methods

### `Private` extractWhereParam

▸ **extractWhereParam**(`param`: [IWherePropParam](../globals.md#iwherepropparam)‹T›): *string*

*Defined in [QueryBuilder.ts:22](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L22)*

**Parameters:**

Name | Type |
------ | ------ |
`param` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |

**Returns:** *string*

___

###  find

▸ **find**(): *Promise‹T[]›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:133](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L133)*

**Returns:** *Promise‹T[]›*

___

###  limit

▸ **limit**(`limitVal`: number): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:93](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L93)*

**Parameters:**

Name | Type |
------ | ------ |
`limitVal` | number |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  orderByAscending

▸ **orderByAscending**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:103](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L103)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  orderByDescending

▸ **orderByDescending**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:118](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L118)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  whereArrayContains

▸ **whereArrayContains**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:81](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L81)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  whereEqualTo

▸ **whereEqualTo**(`param`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:27](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L27)*

**Parameters:**

Name | Type |
------ | ------ |
`param` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  whereGreaterOrEqualThan

▸ **whereGreaterOrEqualThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:48](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L48)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  whereGreaterThan

▸ **whereGreaterThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:36](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L36)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  whereLessOrEqualThan

▸ **whereLessOrEqualThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:69](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L69)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*

___

###  whereLessThan

▸ **whereLessThan**(`prop`: [IWherePropParam](../globals.md#iwherepropparam)‹T›, `val`: [IFirestoreVal](../globals.md#ifirestoreval)): *[QueryBuilder](querybuilder.md)‹T›*

*Implementation of [IQueryBuilder](../interfaces/iquerybuilder.md)*

*Defined in [QueryBuilder.ts:60](https://github.com/wovalle/fireorm/blob/da6b863/src/QueryBuilder.ts#L60)*

**Parameters:**

Name | Type |
------ | ------ |
`prop` | [IWherePropParam](../globals.md#iwherepropparam)‹T› |
`val` | [IFirestoreVal](../globals.md#ifirestoreval) |

**Returns:** *[QueryBuilder](querybuilder.md)‹T›*
