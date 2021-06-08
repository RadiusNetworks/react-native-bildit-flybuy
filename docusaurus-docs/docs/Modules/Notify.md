## Initialize SDK

## Create for Sites in Region

#### Params

| Name | Type | Example |
|------|------|---------|
| region | Obj | `{latitude: 47.6234207,longitude: -122.3300605,radius: 100}` |
| notification | Obj | `{title: 'Test Notification',message: 'Test Notification message',data: {key1: 'value',key2: 'value'}` |

#### Example

```jsx
    const region = {
      latitude: 47.6234207,
      longitude: -122.3300605,
      radius: 100,
    };

    const notification = {
      title: 'Test Notification',
      message: 'Test Notification message',
      data: {
        key1: 'value',
        key2: 'value',
      }

    Flybuy.Notify.createForSitesInRegion(region, notification)
```
**[flybuy Create for Sites in Region Documentation](https://www.radiusnetworks.com/developers/flybuy/#/sdk-2.0/notify?id=create-for-sites-in-region)**

## Clear Notifications

#### Params

| Name | Type |
|------|------|
| None | None |

#### Example

```jsx
Flybuy.Notify.clearNotifications()
```

**[flybuy Clear Notifications Documentation](https://www.radiusnetworks.com/developers/flybuy/#/sdk-2.0/notify?id=clear-notifications)**

## Create for Sites

#### Params

| Name | Type | Example |
|------|------|---------|
| notification | Obj | `{title: 'Test Notification',message: 'Test Notification message',data: {key1: 'value',key2: 'value',}` |
| sites | List | `[{},...]`

#### Example

```jsx
const notification = {
      title: 'Test Notification',
      message: 'Test Notification message',
      data: {
        key1: 'value',
        key2: 'value',
      },
    };

const sites: ISite[] = [
    {
    id: 15942,
    name: 'Test Site',
    phone: '333-333-3333',
    streetAddress: null,
    fullAddress: '500 Yale Ave N, Seattle, WA 98109, USA',
    locality: null,
    region: null,
    country: null,
    postalCode: null,
    latitude: '47.6234207',
    longitude: '-122.3300605',
    coverPhotoUrl: null,
    iconUrl: null,
    instructions: '',
    description: '',
    partnerIdentifier: '001',
    },
];

Flybuy.Notify.createForSites(sites, notification)
```

**[flybuy Create for Sites Documentation](https://www.radiusnetworks.com/developers/flybuy/#/sdk-2.0/notify?id=additional-methods)**