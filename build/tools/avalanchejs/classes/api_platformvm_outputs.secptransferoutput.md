[avalanche](../README.md) › [API-PlatformVM-Outputs](../modules/api_platformvm_outputs.md) › [SECPTransferOutput](api_platformvm_outputs.secptransferoutput.md)

# Class: SECPTransferOutput

An [Output](../modules/src_common.md#output) class which specifies an Output that carries an ammount for an assetID and uses secp256k1 signature scheme.

## Hierarchy

  ↳ [AmountOutput](api_platformvm_outputs.amountoutput.md)

  ↳ **SECPTransferOutput**

## Index

### Constructors

* [constructor](api_platformvm_outputs.secptransferoutput.md#constructor)

### Properties

* [_codecID](api_platformvm_outputs.secptransferoutput.md#protected-_codecid)
* [_typeID](api_platformvm_outputs.secptransferoutput.md#protected-_typeid)
* [_typeName](api_platformvm_outputs.secptransferoutput.md#protected-_typename)
* [addresses](api_platformvm_outputs.secptransferoutput.md#protected-addresses)
* [amount](api_platformvm_outputs.secptransferoutput.md#protected-amount)
* [amountValue](api_platformvm_outputs.secptransferoutput.md#protected-amountvalue)
* [locktime](api_platformvm_outputs.secptransferoutput.md#protected-locktime)
* [numaddrs](api_platformvm_outputs.secptransferoutput.md#protected-numaddrs)
* [threshold](api_platformvm_outputs.secptransferoutput.md#protected-threshold)

### Methods

* [clone](api_platformvm_outputs.secptransferoutput.md#clone)
* [create](api_platformvm_outputs.secptransferoutput.md#create)
* [deserialize](api_platformvm_outputs.secptransferoutput.md#deserialize)
* [fromBuffer](api_platformvm_outputs.secptransferoutput.md#frombuffer)
* [getAddress](api_platformvm_outputs.secptransferoutput.md#getaddress)
* [getAddressIdx](api_platformvm_outputs.secptransferoutput.md#getaddressidx)
* [getAddresses](api_platformvm_outputs.secptransferoutput.md#getaddresses)
* [getAmount](api_platformvm_outputs.secptransferoutput.md#getamount)
* [getCodecID](api_platformvm_outputs.secptransferoutput.md#getcodecid)
* [getLocktime](api_platformvm_outputs.secptransferoutput.md#getlocktime)
* [getOutputID](api_platformvm_outputs.secptransferoutput.md#getoutputid)
* [getSpenders](api_platformvm_outputs.secptransferoutput.md#getspenders)
* [getThreshold](api_platformvm_outputs.secptransferoutput.md#getthreshold)
* [getTypeID](api_platformvm_outputs.secptransferoutput.md#gettypeid)
* [getTypeName](api_platformvm_outputs.secptransferoutput.md#gettypename)
* [makeTransferable](api_platformvm_outputs.secptransferoutput.md#maketransferable)
* [meetsThreshold](api_platformvm_outputs.secptransferoutput.md#meetsthreshold)
* [select](api_platformvm_outputs.secptransferoutput.md#select)
* [serialize](api_platformvm_outputs.secptransferoutput.md#serialize)
* [toBuffer](api_platformvm_outputs.secptransferoutput.md#tobuffer)
* [toString](api_platformvm_outputs.secptransferoutput.md#tostring)
* [comparator](api_platformvm_outputs.secptransferoutput.md#static-comparator)

## Constructors

###  constructor

\+ **new SECPTransferOutput**(`amount`: BN, `addresses`: Buffer[], `locktime`: BN, `threshold`: number): *[SECPTransferOutput](api_platformvm_outputs.secptransferoutput.md)*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[constructor](api_platformvm_outputs.amountoutput.md#constructor)*

*Overrides [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md).[constructor](api_platformvm_outputs.secpowneroutput.md#constructor)*

*Defined in [src/common/output.ts:473](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L473)*

A [StandardAmountOutput](../modules/src_common.md#standardamountoutput) class which issues a payment on an assetID.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`amount` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the amount in the output |
`addresses` | Buffer[] | undefined | An array of [Buffer](https://github.com/feross/buffer)s representing addresses |
`locktime` | BN | undefined | A [BN](https://github.com/indutny/bn.js/) representing the locktime |
`threshold` | number | undefined | A number representing the the threshold number of signers required to sign the transaction  |

**Returns:** *[SECPTransferOutput](api_platformvm_outputs.secptransferoutput.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:40](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L40)*

___

### `Protected` _typeID

• **_typeID**: *number* = PlatformVMConstants.SECPXFEROUTPUTID

*Overrides [AmountOutput](api_platformvm_outputs.amountoutput.md).[_typeID](api_platformvm_outputs.amountoutput.md#protected-_typeid)*

*Defined in [src/apis/platformvm/outputs.ts:100](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/outputs.ts#L100)*

___

### `Protected` _typeName

• **_typeName**: *string* = "SECPTransferOutput"

*Overrides [AmountOutput](api_platformvm_outputs.amountoutput.md).[_typeName](api_platformvm_outputs.amountoutput.md#protected-_typename)*

*Defined in [src/apis/platformvm/outputs.ts:99](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/outputs.ts#L99)*

___

### `Protected` addresses

• **addresses**: *[Address](common_output.address.md)[]* = []

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[addresses](api_platformvm_outputs.amountoutput.md#protected-addresses)*

*Defined in [src/common/output.ts:121](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L121)*

___

### `Protected` amount

• **amount**: *Buffer* = Buffer.alloc(8)

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[amount](api_platformvm_outputs.amountoutput.md#protected-amount)*

*Defined in [src/common/output.ts:446](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L446)*

___

### `Protected` amountValue

• **amountValue**: *BN* = new BN(0)

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[amountValue](api_platformvm_outputs.amountoutput.md#protected-amountvalue)*

*Defined in [src/common/output.ts:447](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L447)*

___

### `Protected` locktime

• **locktime**: *Buffer* = Buffer.alloc(8)

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[locktime](api_platformvm_outputs.amountoutput.md#protected-locktime)*

*Defined in [src/common/output.ts:118](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L118)*

___

### `Protected` numaddrs

• **numaddrs**: *Buffer* = Buffer.alloc(4)

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[numaddrs](api_platformvm_outputs.amountoutput.md#protected-numaddrs)*

*Defined in [src/common/output.ts:120](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L120)*

___

### `Protected` threshold

• **threshold**: *Buffer* = Buffer.alloc(4)

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[threshold](api_platformvm_outputs.amountoutput.md#protected-threshold)*

*Defined in [src/common/output.ts:119](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L119)*

## Methods

###  clone

▸ **clone**(): *this*

*Overrides [AmountOutput](api_platformvm_outputs.amountoutput.md).[clone](api_platformvm_outputs.amountoutput.md#abstract-clone)*

*Defined in [src/apis/platformvm/outputs.ts:115](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/outputs.ts#L115)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [AmountOutput](api_platformvm_outputs.amountoutput.md).[create](api_platformvm_outputs.amountoutput.md#abstract-create)*

*Defined in [src/apis/platformvm/outputs.ts:111](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/outputs.ts#L111)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/src_utils.md#serializedencoding)): *void*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[deserialize](api_platformvm_outputs.amountoutput.md#deserialize)*

*Overrides [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md).[deserialize](api_platformvm_outputs.secpowneroutput.md#deserialize)*

*Defined in [src/common/output.ts:440](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L440)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/src_utils.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`outbuff`: Buffer, `offset`: number): *number*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[fromBuffer](api_platformvm_outputs.amountoutput.md#frombuffer)*

*Overrides [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md).[fromBuffer](api_platformvm_outputs.secpowneroutput.md#frombuffer)*

*Defined in [src/common/output.ts:457](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L457)*

Popuates the instance from a [Buffer](https://github.com/feross/buffer) representing the [StandardAmountOutput](../modules/src_common.md#standardamountoutput) and returns the size of the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`outbuff` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getAddress

▸ **getAddress**(`idx`: number): *Buffer*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[getAddress](api_platformvm_outputs.amountoutput.md#getaddress)*

*Defined in [src/common/output.ts:168](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L168)*

Returns the address from the index provided.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`idx` | number | The index of the address.  |

**Returns:** *Buffer*

Returns the string representing the address.

___

###  getAddressIdx

▸ **getAddressIdx**(`address`: Buffer): *number*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[getAddressIdx](api_platformvm_outputs.amountoutput.md#getaddressidx)*

*Defined in [src/common/output.ts:151](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L151)*

Returns the index of the address.

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`address` | Buffer | A [Buffer](https://github.com/feross/buffer) of the address to look up to return its index.  |

**Returns:** *number*

The index of the address.

___

###  getAddresses

▸ **getAddresses**(): *Buffer[]*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[getAddresses](api_platformvm_outputs.amountoutput.md#getaddresses)*

*Defined in [src/common/output.ts:136](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L136)*

Returns an array of [Buffer](https://github.com/feross/buffer)s for the addresses.

**Returns:** *Buffer[]*

___

###  getAmount

▸ **getAmount**(): *BN*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[getAmount](api_platformvm_outputs.amountoutput.md#getamount)*

*Defined in [src/common/output.ts:452](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L452)*

Returns the amount as a [BN](https://github.com/indutny/bn.js/).

**Returns:** *BN*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:59](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L59)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getLocktime

▸ **getLocktime**(): *BN*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[getLocktime](api_platformvm_outputs.amountoutput.md#getlocktime)*

*Defined in [src/common/output.ts:131](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L131)*

Returns the a [BN](https://github.com/indutny/bn.js/) repersenting the UNIX Timestamp when the lock is made available.

**Returns:** *BN*

___

###  getOutputID

▸ **getOutputID**(): *number*

*Overrides [AmountOutput](api_platformvm_outputs.amountoutput.md).[getOutputID](api_platformvm_outputs.amountoutput.md#abstract-getoutputid)*

*Defined in [src/apis/platformvm/outputs.ts:107](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/outputs.ts#L107)*

Returns the outputID for this output

**Returns:** *number*

___

###  getSpenders

▸ **getSpenders**(`addresses`: Buffer[], `asOf`: BN): *Buffer[]*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[getSpenders](api_platformvm_outputs.amountoutput.md#getspenders)*

*Defined in [src/common/output.ts:197](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L197)*

Given an array of addresses and an optional timestamp, select an array of address [Buffer](https://github.com/feross/buffer)s of qualified spenders for the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`addresses` | Buffer[] | - |
`asOf` | BN | undefined |

**Returns:** *Buffer[]*

___

###  getThreshold

▸ **getThreshold**(): *number*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[getThreshold](api_platformvm_outputs.amountoutput.md#getthreshold)*

*Defined in [src/common/output.ts:126](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L126)*

Returns the threshold of signers required to spend this output.

**Returns:** *number*

___

###  getTypeID

▸ **getTypeID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeID](common_signature.sigidx.md#gettypeid)*

*Defined in [src/utils/serialization.ts:52](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L52)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getTypeName

▸ **getTypeName**(): *string*

*Inherited from [SigIdx](common_signature.sigidx.md).[getTypeName](common_signature.sigidx.md#gettypename)*

*Defined in [src/utils/serialization.ts:45](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L45)*

Used in serialization. TypeName is a string name for the type of object being output.

**Returns:** *string*

___

###  makeTransferable

▸ **makeTransferable**(`assetID`: Buffer): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[makeTransferable](api_platformvm_outputs.amountoutput.md#maketransferable)*

*Overrides [Output](common_output.output.md).[makeTransferable](common_output.output.md#abstract-maketransferable)*

*Defined in [src/apis/platformvm/outputs.ts:86](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/outputs.ts#L86)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`assetID` | Buffer | An assetID which is wrapped around the Buffer of the Output  |

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)*

___

###  meetsThreshold

▸ **meetsThreshold**(`addresses`: Buffer[], `asOf`: BN): *boolean*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[meetsThreshold](api_platformvm_outputs.amountoutput.md#meetsthreshold)*

*Defined in [src/common/output.ts:178](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L178)*

Given an array of address [Buffer](https://github.com/feross/buffer)s and an optional timestamp, returns true if the addresses meet the threshold required to spend the output.

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`addresses` | Buffer[] | - |
`asOf` | BN | undefined |

**Returns:** *boolean*

___

###  select

▸ **select**(`id`: number, ...`args`: any[]): *[Output](common_output.output.md)*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[select](api_platformvm_outputs.amountoutput.md#select)*

*Overrides [Output](common_output.output.md).[select](common_output.output.md#abstract-select)*

*Defined in [src/apis/platformvm/outputs.ts:90](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/outputs.ts#L90)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *[Output](common_output.output.md)*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/src_utils.md#serializedencoding)): *object*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[serialize](api_platformvm_outputs.amountoutput.md#serialize)*

*Overrides [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md).[serialize](api_platformvm_outputs.secpowneroutput.md#serialize)*

*Defined in [src/common/output.ts:433](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L433)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/src_utils.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[toBuffer](api_platformvm_outputs.amountoutput.md#tobuffer)*

*Overrides [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md).[toBuffer](api_platformvm_outputs.secpowneroutput.md#tobuffer)*

*Defined in [src/common/output.ts:467](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L467)*

Returns the buffer representing the [StandardAmountOutput](../modules/src_common.md#standardamountoutput) instance.

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[toString](api_platformvm_outputs.amountoutput.md#tostring)*

*Defined in [src/common/output.ts:262](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L262)*

Returns a base-58 string representing the [Output](../modules/src_common.md#output).

**Returns:** *string*

___

### `Static` comparator

▸ **comparator**(): *function*

*Inherited from [AmountOutput](api_platformvm_outputs.amountoutput.md).[comparator](api_platformvm_outputs.amountoutput.md#static-comparator)*

*Defined in [src/common/output.ts:266](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/output.ts#L266)*

**Returns:** *function*

▸ (`a`: [Output](common_output.output.md), `b`: [Output](common_output.output.md)): *1 | -1 | 0*

**Parameters:**

Name | Type |
------ | ------ |
`a` | [Output](common_output.output.md) |
`b` | [Output](common_output.output.md) |
