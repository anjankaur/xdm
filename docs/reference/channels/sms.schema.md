
# SMS Schema

```
https://ns.adobe.com/xdm/channels/sms
```

Short Message Service delivered to a mobile phone.

| Abstract | Extensible | Status | Identifiable | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|--------------|-------------------|-----------------------|------------|
| Can be instantiated | Yes | Experimental | Yes | Forbidden | Permitted | [channels/sms.schema.json](channels/sms.schema.json) |
## Schema Hierarchy

* SMS `https://ns.adobe.com/xdm/channels/sms`
  * [Extensibility base schema](../common/extensible.schema.md) `https://ns.adobe.com/xdm/common/extensible`
  * [Experience Channel](channel.schema.md) `https://ns.adobe.com/xdm/channels/channel`


## SMS Example
```json
{
  "@id": "https://ns.adobe.com/xdm/channels/sms",
  "@type": "https://ns.adobe.com/xdm/channel-types/messaging"
}
```

# SMS Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [@id](#@id) | `const` | **Required** | SMS (this schema) |
| [@type](#@type) | `const` | Optional | SMS (this schema) |
| [xdm:contentTypes](#xdmcontenttypes) | `const` | Optional | SMS (this schema) |
| [xdm:locationTypes](#xdmlocationtypes) | `const` | Optional | SMS (this schema) |
| [xdm:metricTypes](#xdmmetrictypes) | `const` | Optional | SMS (this schema) |
| [xdm:mode](#xdmmode) | `const` | Optional | SMS (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## @id

The ID uniquely identifies the channel. Each specific experience channel defines a constant `@id`.

`@id`
* is **required**
* type: `const`
* defined in this schema

The value of this property **must** be equal to:

```json
"https://ns.adobe.com/xdm/channels/sms"
```





## @type

The `@type` property is used to provide a rough classification of channels with similar properties.

`@type`
* is optional
* type: `const`
* defined in this schema

The value of this property **must** be equal to:

```json
"https://ns.adobe.com/xdm/channel-types/messaging"
```


### @type Known Values
| Value | Description |
|-------|-------------|
| `https://ns.adobe.com/xdm/channel-types/web` | The world wide web, including mobile web |
| `https://ns.adobe.com/xdm/channel-types/social` | Social media platforms |
| `https://ns.adobe.com/xdm/channel-types/mobile` | Mobile applications |
| `https://ns.adobe.com/xdm/channel-types/messaging` | Instant Messaging |
| `https://ns.adobe.com/xdm/channel-types/email` | E-Mail |
| `https://ns.adobe.com/xdm/channel-types/offline` | Non-Digital experience channels |




## xdm:contentTypes

The content types that this channel can deliver.

`xdm:contentTypes`
* is optional
* type: `const`

* defined in this schema

The value of this property **must** be equal to:

```json
[]
```





## xdm:locationTypes

The types of locations (virtual places) that this channel consists of and can deliver content to.

`xdm:locationTypes`
* is optional
* type: `const`

* defined in this schema

The value of this property **must** be equal to:

```json
[]
```





## xdm:metricTypes

The metrics that can be collected in this channel.

`xdm:metricTypes`
* is optional
* type: `const`

* defined in this schema

The value of this property **must** be equal to:

```json
[]
```





## xdm:mode

How experiences are delivered in this channel.

`xdm:mode`
* is optional
* type: `const`
* defined in this schema

The value of this property **must** be equal to:

```json
"push"
```


### xdm:mode Known Values
| Value | Description |
|-------|-------------|
| `push` | The publisher of an experience can initiate an experience by sending a message into the channel. Most `push` channels involve some form of subscription or opt-in. |
| `pull` | The consumer can initiate an experience by requesting a location in the channel. Most `pull` channels give publishers some control how the experience is then delivered. |
| `bidirectional` | Both `push` and `pull` interaction modes are supported by the channel. |



