[avalanche](../README.md) › [API-PlatformVM-ValidationTx](../modules/api_platformvm_validationtx.md) › [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)

# Class: AddDelegatorTx

Class representing an unsigned AddDelegatorTx transaction.

## Hierarchy

  ↳ [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md)

  ↳ **AddDelegatorTx**

  ↳ [AddValidatorTx](api_platformvm_validationtx.addvalidatortx.md)

## Index

### Constructors

* [constructor](api_platformvm_validationtx.adddelegatortx.md#constructor)

### Properties

* [_codecID](api_platformvm_validationtx.adddelegatortx.md#protected-_codecid)
* [_typeID](api_platformvm_validationtx.adddelegatortx.md#protected-_typeid)
* [_typeName](api_platformvm_validationtx.adddelegatortx.md#protected-_typename)
* [blockchainID](api_platformvm_validationtx.adddelegatortx.md#protected-blockchainid)
* [endTime](api_platformvm_validationtx.adddelegatortx.md#protected-endtime)
* [ins](api_platformvm_validationtx.adddelegatortx.md#protected-ins)
* [memo](api_platformvm_validationtx.adddelegatortx.md#protected-memo)
* [networkID](api_platformvm_validationtx.adddelegatortx.md#protected-networkid)
* [nodeID](api_platformvm_validationtx.adddelegatortx.md#protected-nodeid)
* [numins](api_platformvm_validationtx.adddelegatortx.md#protected-numins)
* [numouts](api_platformvm_validationtx.adddelegatortx.md#protected-numouts)
* [outs](api_platformvm_validationtx.adddelegatortx.md#protected-outs)
* [rewardOwners](api_platformvm_validationtx.adddelegatortx.md#protected-rewardowners)
* [stakeOuts](api_platformvm_validationtx.adddelegatortx.md#protected-stakeouts)
* [startTime](api_platformvm_validationtx.adddelegatortx.md#protected-starttime)
* [weight](api_platformvm_validationtx.adddelegatortx.md#protected-weight)

### Methods

* [clone](api_platformvm_validationtx.adddelegatortx.md#clone)
* [create](api_platformvm_validationtx.adddelegatortx.md#create)
* [deserialize](api_platformvm_validationtx.adddelegatortx.md#deserialize)
* [fromBuffer](api_platformvm_validationtx.adddelegatortx.md#frombuffer)
* [getBlockchainID](api_platformvm_validationtx.adddelegatortx.md#getblockchainid)
* [getCodecID](api_platformvm_validationtx.adddelegatortx.md#getcodecid)
* [getEndTime](api_platformvm_validationtx.adddelegatortx.md#getendtime)
* [getIns](api_platformvm_validationtx.adddelegatortx.md#getins)
* [getMemo](api_platformvm_validationtx.adddelegatortx.md#getmemo)
* [getNetworkID](api_platformvm_validationtx.adddelegatortx.md#getnetworkid)
* [getNodeID](api_platformvm_validationtx.adddelegatortx.md#getnodeid)
* [getNodeIDString](api_platformvm_validationtx.adddelegatortx.md#getnodeidstring)
* [getOuts](api_platformvm_validationtx.adddelegatortx.md#getouts)
* [getRewardOwners](api_platformvm_validationtx.adddelegatortx.md#getrewardowners)
* [getStakeAmount](api_platformvm_validationtx.adddelegatortx.md#getstakeamount)
* [getStakeAmountBuffer](api_platformvm_validationtx.adddelegatortx.md#getstakeamountbuffer)
* [getStakeOuts](api_platformvm_validationtx.adddelegatortx.md#getstakeouts)
* [getStakeOutsTotal](api_platformvm_validationtx.adddelegatortx.md#getstakeoutstotal)
* [getStartTime](api_platformvm_validationtx.adddelegatortx.md#getstarttime)
* [getTotalOuts](api_platformvm_validationtx.adddelegatortx.md#gettotalouts)
* [getTxType](api_platformvm_validationtx.adddelegatortx.md#gettxtype)
* [getTypeID](api_platformvm_validationtx.adddelegatortx.md#gettypeid)
* [getTypeName](api_platformvm_validationtx.adddelegatortx.md#gettypename)
* [getWeight](api_platformvm_validationtx.adddelegatortx.md#getweight)
* [getWeightBuffer](api_platformvm_validationtx.adddelegatortx.md#getweightbuffer)
* [select](api_platformvm_validationtx.adddelegatortx.md#select)
* [serialize](api_platformvm_validationtx.adddelegatortx.md#serialize)
* [sign](api_platformvm_validationtx.adddelegatortx.md#sign)
* [toBuffer](api_platformvm_validationtx.adddelegatortx.md#tobuffer)
* [toString](api_platformvm_validationtx.adddelegatortx.md#tostring)

## Constructors

###  constructor

\+ **new AddDelegatorTx**(`networkID`: number, `blockchainID`: Buffer, `outs`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `ins`: [TransferableInput](api_platformvm_inputs.transferableinput.md)[], `memo`: Buffer, `nodeID`: Buffer, `startTime`: BN, `endTime`: BN, `stakeAmount`: BN, `stakeOuts`: [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[], `rewardOwners`: [ParseableOutput](api_platformvm_outputs.parseableoutput.md)): *[AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[constructor](api_platformvm_validationtx.weightedvalidatortx.md#constructor)*

*Defined in [src/apis/platformvm/validationtx.ts:438](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L438)*

Class representing an unsigned AddDelegatorTx transaction.

**Parameters:**

Name | Type | Default | Description |
------ | ------ | ------ | ------ |
`networkID` | number | DefaultNetworkID | Optional. Networkid, [DefaultNetworkID](../modules/utils_constants.md#const-defaultnetworkid) |
`blockchainID` | Buffer | Buffer.alloc(32, 16) | Optional. Blockchainid, default Buffer.alloc(32, 16) |
`outs` | [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[] | undefined | Optional. Array of the [TransferableOutput](api_platformvm_outputs.transferableoutput.md)s |
`ins` | [TransferableInput](api_platformvm_inputs.transferableinput.md)[] | undefined | Optional. Array of the [TransferableInput](api_platformvm_inputs.transferableinput.md)s |
`memo` | Buffer | undefined | Optional. [Buffer](https://github.com/feross/buffer) for the memo field |
`nodeID` | Buffer | undefined | Optional. The node ID of the validator being added. |
`startTime` | BN | undefined | Optional. The Unix time when the validator starts validating the Primary Network. |
`endTime` | BN | undefined | Optional. The Unix time when the validator stops validating the Primary Network (and staked AVAX is returned). |
`stakeAmount` | BN | undefined | Optional. The amount of nAVAX the validator is staking. |
`stakeOuts` | [TransferableOutput](api_platformvm_outputs.transferableoutput.md)[] | undefined | Optional. The outputs used in paying the stake. |
`rewardOwners` | [ParseableOutput](api_platformvm_outputs.parseableoutput.md) | undefined | Optional. The [ParseableOutput](api_platformvm_outputs.parseableoutput.md) containing a [SECPOwnerOutput](api_platformvm_outputs.secpowneroutput.md) for the rewards.  |

**Returns:** *[AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [SigIdx](common_signature.sigidx.md).[_codecID](common_signature.sigidx.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:40](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L40)*

___

### `Protected` _typeID

• **_typeID**: *number* = PlatformVMConstants.ADDDELEGATORTX

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[_typeID](api_platformvm_validationtx.weightedvalidatortx.md#protected-_typeid)*

*Defined in [src/apis/platformvm/validationtx.ts:318](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L318)*

___

### `Protected` _typeName

• **_typeName**: *string* = "AddDelegatorTx"

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[_typeName](api_platformvm_validationtx.weightedvalidatortx.md#protected-_typename)*

*Defined in [src/apis/platformvm/validationtx.ts:317](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L317)*

___

### `Protected` blockchainID

• **blockchainID**: *Buffer* = Buffer.alloc(32)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[blockchainID](common_transactions.standardbasetx.md#protected-blockchainid)*

*Defined in [src/common/tx.ts:52](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L52)*

___

### `Protected` endTime

• **endTime**: *Buffer* = Buffer.alloc(8)

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[endTime](api_platformvm_validationtx.validatortx.md#protected-endtime)*

*Defined in [src/apis/platformvm/validationtx.ts:50](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L50)*

___

### `Protected` ins

• **ins**: *[StandardTransferableInput](common_inputs.standardtransferableinput.md)[]*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[ins](common_transactions.standardbasetx.md#protected-ins)*

*Defined in [src/common/tx.ts:56](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L56)*

___

### `Protected` memo

• **memo**: *Buffer* = Buffer.alloc(0)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[memo](common_transactions.standardbasetx.md#protected-memo)*

*Defined in [src/common/tx.ts:57](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L57)*

___

### `Protected` networkID

• **networkID**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[networkID](common_transactions.standardbasetx.md#protected-networkid)*

*Defined in [src/common/tx.ts:51](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L51)*

___

### `Protected` nodeID

• **nodeID**: *Buffer* = Buffer.alloc(20)

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[nodeID](api_platformvm_validationtx.validatortx.md#protected-nodeid)*

*Defined in [src/apis/platformvm/validationtx.ts:48](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L48)*

___

### `Protected` numins

• **numins**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[numins](common_transactions.standardbasetx.md#protected-numins)*

*Defined in [src/common/tx.ts:55](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L55)*

___

### `Protected` numouts

• **numouts**: *Buffer* = Buffer.alloc(4)

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[numouts](common_transactions.standardbasetx.md#protected-numouts)*

*Defined in [src/common/tx.ts:53](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L53)*

___

### `Protected` outs

• **outs**: *[StandardTransferableOutput](common_output.standardtransferableoutput.md)[]*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[outs](common_transactions.standardbasetx.md#protected-outs)*

*Defined in [src/common/tx.ts:54](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L54)*

___

### `Protected` rewardOwners

• **rewardOwners**: *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)* = undefined

*Defined in [src/apis/platformvm/validationtx.ts:340](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L340)*

___

### `Protected` stakeOuts

• **stakeOuts**: *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]* = []

*Defined in [src/apis/platformvm/validationtx.ts:339](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L339)*

___

### `Protected` startTime

• **startTime**: *Buffer* = Buffer.alloc(8)

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[startTime](api_platformvm_validationtx.validatortx.md#protected-starttime)*

*Defined in [src/apis/platformvm/validationtx.ts:49](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L49)*

___

### `Protected` weight

• **weight**: *Buffer* = Buffer.alloc(8)

*Inherited from [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[weight](api_platformvm_validationtx.weightedvalidatortx.md#protected-weight)*

*Defined in [src/apis/platformvm/validationtx.ts:138](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L138)*

## Methods

###  clone

▸ **clone**(): *this*

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[clone](api_platformvm_basetx.basetx.md#clone)*

*Defined in [src/apis/platformvm/validationtx.ts:430](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L430)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[create](api_platformvm_basetx.basetx.md#create)*

*Defined in [src/apis/platformvm/validationtx.ts:436](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L436)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/src_utils.md#serializedencoding)): *void*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[deserialize](api_platformvm_validationtx.weightedvalidatortx.md#deserialize)*

*Defined in [src/apis/platformvm/validationtx.ts:328](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L328)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/src_utils.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: Buffer, `offset`: number): *number*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[fromBuffer](api_platformvm_validationtx.weightedvalidatortx.md#frombuffer)*

*Defined in [src/apis/platformvm/validationtx.ts:392](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L392)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | Buffer | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getBlockchainID

▸ **getBlockchainID**(): *Buffer*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[getBlockchainID](common_transactions.standardbasetx.md#getblockchainid)*

*Defined in [src/common/tx.ts:72](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L72)*

Returns the Buffer representation of the BlockchainID

**Returns:** *Buffer*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [SigIdx](common_signature.sigidx.md).[getCodecID](common_signature.sigidx.md#getcodecid)*

*Defined in [src/utils/serialization.ts:59](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/utils/serialization.ts#L59)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getEndTime

▸ **getEndTime**(): *BN‹›*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getEndTime](api_platformvm_validationtx.validatortx.md#getendtime)*

*Defined in [src/apis/platformvm/validationtx.ts:75](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L75)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN‹›*

___

###  getIns

▸ **getIns**(): *[TransferableInput](api_platformvm_inputs.transferableinput.md)[]*

*Inherited from [BaseTx](api_platformvm_basetx.basetx.md).[getIns](api_platformvm_basetx.basetx.md#getins)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getIns](common_transactions.standardbasetx.md#abstract-getins)*

*Defined in [src/apis/platformvm/basetx.ts:52](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/basetx.ts#L52)*

**Returns:** *[TransferableInput](api_platformvm_inputs.transferableinput.md)[]*

___

###  getMemo

▸ **getMemo**(): *Buffer*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[getMemo](common_transactions.standardbasetx.md#getmemo)*

*Defined in [src/common/tx.ts:92](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L92)*

Returns the [Buffer](https://github.com/feross/buffer) representation of the memo

**Returns:** *Buffer*

___

###  getNetworkID

▸ **getNetworkID**(): *number*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[getNetworkID](common_transactions.standardbasetx.md#getnetworkid)*

*Defined in [src/common/tx.ts:67](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L67)*

Returns the NetworkID as a number

**Returns:** *number*

___

###  getNodeID

▸ **getNodeID**(): *Buffer*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getNodeID](api_platformvm_validationtx.validatortx.md#getnodeid)*

*Defined in [src/apis/platformvm/validationtx.ts:55](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L55)*

Returns a [Buffer](https://github.com/feross/buffer) for the stake amount.

**Returns:** *Buffer*

___

###  getNodeIDString

▸ **getNodeIDString**(): *string*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getNodeIDString](api_platformvm_validationtx.validatortx.md#getnodeidstring)*

*Defined in [src/apis/platformvm/validationtx.ts:62](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L62)*

Returns a string for the nodeID amount.

**Returns:** *string*

___

###  getOuts

▸ **getOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Inherited from [BaseTx](api_platformvm_basetx.basetx.md).[getOuts](api_platformvm_basetx.basetx.md#getouts)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[getOuts](common_transactions.standardbasetx.md#abstract-getouts)*

*Defined in [src/apis/platformvm/basetx.ts:48](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/basetx.ts#L48)*

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getRewardOwners

▸ **getRewardOwners**(): *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

*Defined in [src/apis/platformvm/validationtx.ts:384](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L384)*

Returns a [Buffer](https://github.com/feross/buffer) for the reward address.

**Returns:** *[ParseableOutput](api_platformvm_outputs.parseableoutput.md)*

___

###  getStakeAmount

▸ **getStakeAmount**(): *BN*

*Defined in [src/apis/platformvm/validationtx.ts:352](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L352)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN*

___

###  getStakeAmountBuffer

▸ **getStakeAmountBuffer**(): *Buffer*

*Defined in [src/apis/platformvm/validationtx.ts:359](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L359)*

Returns a [Buffer](https://github.com/feross/buffer) for the stake amount.

**Returns:** *Buffer*

___

###  getStakeOuts

▸ **getStakeOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Defined in [src/apis/platformvm/validationtx.ts:366](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L366)*

Returns the array of outputs being staked.

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getStakeOutsTotal

▸ **getStakeOutsTotal**(): *BN*

*Defined in [src/apis/platformvm/validationtx.ts:373](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L373)*

Should match stakeAmount. Used in sanity checking.

**Returns:** *BN*

___

###  getStartTime

▸ **getStartTime**(): *BN‹›*

*Inherited from [ValidatorTx](api_platformvm_validationtx.validatortx.md).[getStartTime](api_platformvm_validationtx.validatortx.md#getstarttime)*

*Defined in [src/apis/platformvm/validationtx.ts:68](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L68)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN‹›*

___

###  getTotalOuts

▸ **getTotalOuts**(): *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[getTotalOuts](api_platformvm_basetx.basetx.md#gettotalouts)*

*Defined in [src/apis/platformvm/validationtx.ts:388](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L388)*

**Returns:** *[TransferableOutput](api_platformvm_outputs.transferableoutput.md)[]*

___

###  getTxType

▸ **getTxType**(): *number*

*Overrides [BaseTx](api_platformvm_basetx.basetx.md).[getTxType](api_platformvm_basetx.basetx.md#gettxtype)*

*Defined in [src/apis/platformvm/validationtx.ts:345](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L345)*

Returns the id of the [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md)

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

###  getWeight

▸ **getWeight**(): *BN*

*Inherited from [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[getWeight](api_platformvm_validationtx.weightedvalidatortx.md#getweight)*

*Defined in [src/apis/platformvm/validationtx.ts:143](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L143)*

Returns a [BN](https://github.com/indutny/bn.js/) for the stake amount.

**Returns:** *BN*

___

###  getWeightBuffer

▸ **getWeightBuffer**(): *Buffer*

*Inherited from [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[getWeightBuffer](api_platformvm_validationtx.weightedvalidatortx.md#getweightbuffer)*

*Defined in [src/apis/platformvm/validationtx.ts:150](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L150)*

Returns a [Buffer](https://github.com/feross/buffer) for the stake amount.

**Returns:** *Buffer*

___

###  select

▸ **select**(`id`: number, ...`args`: any[]): *this*

*Inherited from [BaseTx](api_platformvm_basetx.basetx.md).[select](api_platformvm_basetx.basetx.md#select)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[select](common_transactions.standardbasetx.md#abstract-select)*

*Defined in [src/apis/platformvm/basetx.ts:143](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/basetx.ts#L143)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *this*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/src_utils.md#serializedencoding)): *object*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[serialize](api_platformvm_validationtx.weightedvalidatortx.md#serialize)*

*Defined in [src/apis/platformvm/validationtx.ts:320](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L320)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/src_utils.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  sign

▸ **sign**(`msg`: Buffer, `kc`: [KeyChain](api_platformvm_keychain.keychain.md)): *[Credential](common_signature.credential.md)[]*

*Inherited from [BaseTx](api_platformvm_basetx.basetx.md).[sign](api_platformvm_basetx.basetx.md#sign)*

*Overrides [StandardBaseTx](common_transactions.standardbasetx.md).[sign](common_transactions.standardbasetx.md#abstract-sign)*

*Defined in [src/apis/platformvm/basetx.ts:116](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/basetx.ts#L116)*

Takes the bytes of an [UnsignedTx](api_platformvm_transactions.unsignedtx.md) and returns an array of [Credential](common_signature.credential.md)s

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`msg` | Buffer | A Buffer for the [UnsignedTx](api_platformvm_transactions.unsignedtx.md) |
`kc` | [KeyChain](api_platformvm_keychain.keychain.md) | An [KeyChain](api_platformvm_keychain.keychain.md) used in signing  |

**Returns:** *[Credential](common_signature.credential.md)[]*

An array of [Credential](common_signature.credential.md)s

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Overrides [WeightedValidatorTx](api_platformvm_validationtx.weightedvalidatortx.md).[toBuffer](api_platformvm_validationtx.weightedvalidatortx.md#tobuffer)*

*Defined in [src/apis/platformvm/validationtx.ts:411](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/apis/platformvm/validationtx.ts#L411)*

Returns a [Buffer](https://github.com/feross/buffer) representation of the [AddDelegatorTx](api_platformvm_validationtx.adddelegatortx.md).

**Returns:** *Buffer*

___

###  toString

▸ **toString**(): *string*

*Inherited from [StandardBaseTx](common_transactions.standardbasetx.md).[toString](common_transactions.standardbasetx.md#tostring)*

*Defined in [src/common/tx.ts:129](https://github.com/ava-labs/avalanchejs/blob/ae78dee/src/common/tx.ts#L129)*

Returns a base-58 representation of the [StandardBaseTx](common_transactions.standardbasetx.md).

**Returns:** *string*
