# Overview

```
Module Name: AdKernel Bidder Adapter
Module Type: Bidder Adapter
Maintainer: denis@adkernel.com
```

# Description

Connects to AdKernel whitelabel platform.
Banner and video formats are supported.
The AdKernel adapter doesn't support multiple sizes per ad-unit and will use the first one if multiple sizes are defined.


# Test Parameters
```
    var adUnits = [
      {
        code: 'banner-ad-div',
        sizes: [[300, 250]],  // banner size
        bids: [
          {
            bidder: 'adkernel',
            params: {
              zoneId: '30164',  //required parameter
              host: 'cpm.metaadserving.com' //required parameter
            }
          }
        ]
      }, {
        code: 'video-ad-player',
        sizes: [640, 480],   // video player size
        bids: [
          {
            bidder: 'adkernel',
            mediaType : 'video',
            params: {
              zoneId: '30164',  //required parameter
              host: 'cpm.metaadserving.com' //required parameter
            }
          }
        ]
      }
    ];
```
