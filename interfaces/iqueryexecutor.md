
# Interface: IQueryExecutor <**T**>

## Type parameters

▪ **T**

## Hierarchy

* **IQueryExecutor**

## Implemented by

* [AbstractFirestoreRepository](../classes/abstractfirestorerepository.md)
* [BaseFirestoreRepository](../classes/basefirestorerepository.md)
* [TransactionRepository](../classes/transactionrepository.md)

## Index

### Methods

* [execute](iqueryexecutor.md#execute)

## Methods

###  execute

▸ **execute**(`queries`: [IFireOrmQueryLine](ifireormqueryline.md)[], `limitVal?`: number, `orderByObj?`: [IOrderByParams](iorderbyparams.md)): *Promise‹T[]›*

*Defined in [types.ts:76](https://github.com/wovalle/fireorm/blob/da6b863/src/types.ts#L76)*

**Parameters:**

Name | Type |
------ | ------ |
`queries` | [IFireOrmQueryLine](ifireormqueryline.md)[] |
`limitVal?` | number |
`orderByObj?` | [IOrderByParams](iorderbyparams.md) |

**Returns:** *Promise‹T[]›*
