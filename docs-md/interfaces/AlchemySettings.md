[alchemy-sdk](../README.md) / [Exports](../modules.md) / AlchemySettings

# Interface: AlchemySettings

Options object used to configure the Alchemy SDK.

## Table of contents

### Properties

- [apiKey](AlchemySettings.md#apikey)
- [authToken](AlchemySettings.md#authtoken)
- [batchRequests](AlchemySettings.md#batchrequests)
- [maxRetries](AlchemySettings.md#maxretries)
- [network](AlchemySettings.md#network)
- [requestTimeout](AlchemySettings.md#requesttimeout)
- [url](AlchemySettings.md#url)

## Properties

### apiKey

• `Optional` **apiKey**: `string`

The Alchemy API key that can be found in the Alchemy dashboard.

Defaults to: "demo" (a rate-limited public API key)

#### Defined in

[src/types/types.ts:25](https://github.com/alchemyplatform/alchemy-sdk-js/blob/7bf2430/src/types/types.ts#L25)

___

### authToken

• `Optional` **authToken**: `string`

Alchemy auth token required to use the Notify API. This token can be found
in the Alchemy Dashboard on the Notify tab.

#### Defined in

[src/types/types.ts:51](https://github.com/alchemyplatform/alchemy-sdk-js/blob/7bf2430/src/types/types.ts#L51)

___

### batchRequests

• `Optional` **batchRequests**: `boolean`

Optional setting that automatically batches and sends json-rpc requests for
higher throughput and reduced network IO. Defaults to false.

This implementation is based on the `JsonRpcBatchProvider` in ethers.

#### Defined in

[src/types/types.ts:65](https://github.com/alchemyplatform/alchemy-sdk-js/blob/7bf2430/src/types/types.ts#L65)

___

### maxRetries

• `Optional` **maxRetries**: `number`

The maximum number of retries to attempt if a request fails. Defaults to 5.

#### Defined in

[src/types/types.ts:36](https://github.com/alchemyplatform/alchemy-sdk-js/blob/7bf2430/src/types/types.ts#L36)

___

### network

• `Optional` **network**: [`Network`](../enums/Network.md)

The name of the network. Once configured, the network cannot be changed. To
use a different network, instantiate a new `Alchemy` instance.

Defaults to: Network.ETH_MAINNET

#### Defined in

[src/types/types.ts:33](https://github.com/alchemyplatform/alchemy-sdk-js/blob/7bf2430/src/types/types.ts#L33)

___

### requestTimeout

• `Optional` **requestTimeout**: `number`

Optional Request timeout provided in `ms` while using NFT and NOTIFY API.
Default to 0 (No timeout).

#### Defined in

[src/types/types.ts:57](https://github.com/alchemyplatform/alchemy-sdk-js/blob/7bf2430/src/types/types.ts#L57)

___

### url

• `Optional` **url**: `string`

Optional URL endpoint to use for all requests. Setting this field will
override the URL generated by the [network](AlchemySettings.md#network) and [apiKey](AlchemySettings.md#apikey) fields.

This field is useful for testing or for using a custom node endpoint. Note
that not all methods will work with custom URLs.

#### Defined in

[src/types/types.ts:45](https://github.com/alchemyplatform/alchemy-sdk-js/blob/7bf2430/src/types/types.ts#L45)
