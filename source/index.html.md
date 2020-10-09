---
title: Beatchain API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell

toc_footers:
  - <a href='https://beatchain.com'>Create Account</a>
  - <a href='mailto:enquiries@beatchain.com'>Contact Beatchain</a>

includes:
  - errors

search: true

code_clipboard: true
---

# Introduction

Welcome to Beatchain's API reference.

# Authentication

Beatchain uses cognito for authentication. Here there is information on how to generate session tokens <a href='https://docs.aws.amazon.com/cognito/latest/developerguide/authentication.html'>https://docs.aws.amazon.com/cognito/latest/developerguide/authentication.html</a>.
The User Pool ID is `eu-west-1_R6iRUgXku` and the APP client ID is `1udch7qs0q2692oacqsusf1621`

<aside class="notice">
You must replace <code>Bearer_Token</code> with your account's session JWT token.
</aside>

# Admin


## GET admin/artist/search

```shell
curl "https://api.beatchain.com/core/admin/artist/search"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/artist/search`


  
## POST admin/distribution

```shell
curl "https://api.beatchain.com/core/admin/distribution"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/distribution`


  
## GET admin/distribution/{userId}/{releaseId}

```shell
curl "https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}`


### Path Parameters

Parameter | Description
--------- | -----------
userId |
releaseId |

  
## GET admin/distribution/{userId}/{releaseId}/publish

```shell
curl "https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}/publish"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}/publish`


### Path Parameters

Parameter | Description
--------- | -----------
userId |
releaseId |

  
## GET admin/distribution/{userId}/{releaseId}/unpublish

```shell
curl "https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}/unpublish"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}/unpublish`


### Path Parameters

Parameter | Description
--------- | -----------
userId |
releaseId |

  
## POST admin/distribution/{userId}/{releaseId}/upsert

```shell
curl "https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}/upsert"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/distribution/{userId}/{releaseId}/upsert`


### Path Parameters

Parameter | Description
--------- | -----------
userId |
releaseId |

  
## GET admin/fanbuilder

```shell
curl "https://api.beatchain.com/core/admin/fanbuilder"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/fanbuilder`


  
## GET admin/fanbuilder/{userId}/{campaignId}

```shell
curl "https://api.beatchain.com/core/admin/fanbuilder/{userId}/{campaignId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/fanbuilder/{userId}/{campaignId}`


### Path Parameters

Parameter | Description
--------- | -----------
userId |
campaignId |

  
## GET admin/partners

```shell
curl "https://api.beatchain.com/core/admin/partners"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/partners`


  
## POST admin/partners

```shell
curl "https://api.beatchain.com/core/admin/partners"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/partners`


  
## DELETE admin/partners/{slug}

```shell
curl "https://api.beatchain.com/core/admin/partners/{slug}"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`DELETE https://api.beatchain.com/core/admin/partners/{slug}`


### Path Parameters

Parameter | Description
--------- | -----------
slug |

  
## GET admin/payouts

```shell
curl "https://api.beatchain.com/core/admin/payouts"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/payouts`


  
## POST admin/payouts/approve

```shell
curl "https://api.beatchain.com/core/admin/payouts/approve"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/payouts/approve`


  
## GET admin/signups/hubspot

```shell
curl "https://api.beatchain.com/core/admin/signups/hubspot"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/signups/hubspot`


  
## POST admin/signups/convert

```shell
curl "https://api.beatchain.com/core/admin/signups/convert"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/signups/convert`


  
## GET admin/user

```shell
curl "https://api.beatchain.com/core/admin/user"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user`


  
## POST admin/user

```shell
curl "https://api.beatchain.com/core/admin/user"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/user`


  
## DELETE admin/user/{email}

```shell
curl "https://api.beatchain.com/core/admin/user/{email}"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`DELETE https://api.beatchain.com/core/admin/user/{email}`


### Path Parameters

Parameter | Description
--------- | -----------
email |

  
## PUT admin/user/{email}

```shell
curl "https://api.beatchain.com/core/admin/user/{email}"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/admin/user/{email}`


### Path Parameters

Parameter | Description
--------- | -----------
email |

  
## PUT admin/user/{email}/act

```shell
curl "https://api.beatchain.com/core/admin/user/{email}/act"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/admin/user/{email}/act`


### Path Parameters

Parameter | Description
--------- | -----------
email |

  
## GET admin/user/{email}/impersonate

```shell
curl "https://api.beatchain.com/core/admin/user/{email}/impersonate"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user/{email}/impersonate`


### Path Parameters

Parameter | Description
--------- | -----------
email |

  
## GET admin/user/{email}/event

```shell
curl "https://api.beatchain.com/core/admin/user/{email}/event"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user/{email}/event`


### Path Parameters

Parameter | Description
--------- | -----------
email |

  
## PUT admin/user/{email}/role

```shell
curl "https://api.beatchain.com/core/admin/user/{email}/role"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/admin/user/{email}/role`


### Path Parameters

Parameter | Description
--------- | -----------
email |

  
## PUT admin/user/{email}/cohort

```shell
curl "https://api.beatchain.com/core/admin/user/{email}/cohort"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/admin/user/{email}/cohort`


### Path Parameters

Parameter | Description
--------- | -----------
email |

  
## GET admin/user/act

```shell
curl "https://api.beatchain.com/core/admin/user/act"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user/act`


  
## GET admin/user/event

```shell
curl "https://api.beatchain.com/core/admin/user/event"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user/event`


  
## GET admin/user/role

```shell
curl "https://api.beatchain.com/core/admin/user/role"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user/role`


  
## GET admin/user/cohort

```shell
curl "https://api.beatchain.com/core/admin/user/cohort"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user/cohort`


  
## GET admin/user/search

```shell
curl "https://api.beatchain.com/core/admin/user/search"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/user/search`


  
## POST admin/user/scrape

```shell
curl "https://api.beatchain.com/core/admin/user/scrape"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/user/scrape`


  
## GET admin/userpool

```shell
curl "https://api.beatchain.com/core/admin/userpool"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/userpool`


  
## POST admin/userpool

```shell
curl "https://api.beatchain.com/core/admin/userpool"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/admin/userpool`


  
## GET admin/userpool/{userId}

```shell
curl "https://api.beatchain.com/core/admin/userpool/{userId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/userpool/{userId}`


### Path Parameters

Parameter | Description
--------- | -----------
userId |

  
## GET admin/warehouse/analytics

```shell
curl "https://api.beatchain.com/core/admin/warehouse/analytics"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/admin/warehouse/analytics`


  
    
# Analytics


## GET analytics/fuga/{actId}

```shell
curl "https://api.beatchain.com/core/analytics/fuga/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/analytics/fuga/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET analytics/manager

```shell
curl "https://api.beatchain.com/core/analytics/manager"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/analytics/manager`


  
## GET analytics/multi/{actId}

```shell
curl "https://api.beatchain.com/core/analytics/multi/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/analytics/multi/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET analytics/social/fan_stats/{actId}

```shell
curl "https://api.beatchain.com/core/analytics/social/fan_stats/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/analytics/social/fan_stats/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET analytics/social/scores/{actId}

```shell
curl "https://api.beatchain.com/core/analytics/social/scores/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/analytics/social/scores/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET analytics/social/social_engagement_map/{actId}

```shell
curl "https://api.beatchain.com/core/analytics/social/social_engagement_map/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/analytics/social/social_engagement_map/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
    
# Artist


## GET artist/getByName/{name}

```shell
curl "https://api.beatchain.com/core/artist/getByName/{name}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/artist/getByName/{name}`


### Path Parameters

Parameter | Description
--------- | -----------
name |

  
## GET artist/musicbrainz

```shell
curl "https://api.beatchain.com/core/artist/musicbrainz"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/artist/musicbrainz`


  
## GET artist/search/public/{artistName}

```shell
curl "https://api.beatchain.com/core/artist/search/public/{artistName}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/artist/search/public/{artistName}`


### Path Parameters

Parameter | Description
--------- | -----------
artistName |

  
## GET artist/search/{searchTerm}

```shell
curl "https://api.beatchain.com/core/artist/search/{searchTerm}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/artist/search/{searchTerm}`


### Path Parameters

Parameter | Description
--------- | -----------
searchTerm |

  
## POST artist/social/validate

```shell
curl "https://api.beatchain.com/core/artist/social/validate"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/artist/social/validate`


  
## GET artist/social/state-machine

```shell
curl "https://api.beatchain.com/core/artist/social/state-machine"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/artist/social/state-machine`


  
## POST artist/{actId}/location

```shell
curl "https://api.beatchain.com/core/artist/{actId}/location"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/artist/{actId}/location`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET artist/{actId}/genre

```shell
curl "https://api.beatchain.com/core/artist/{actId}/genre"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/artist/{actId}/genre`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST artist/{actId}/genre

```shell
curl "https://api.beatchain.com/core/artist/{actId}/genre"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/artist/{actId}/genre`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## PUT artist/{actId}/name

```shell
curl "https://api.beatchain.com/core/artist/{actId}/name"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/artist/{actId}/name`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## PUT artist/{actId}/profile

```shell
curl "https://api.beatchain.com/core/artist/{actId}/profile"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/artist/{actId}/profile`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## PUT artist/{actId}/profile/image

```shell
curl "https://api.beatchain.com/core/artist/{actId}/profile/image"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/artist/{actId}/profile/image`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## PUT artist/{actId}/social

```shell
curl "https://api.beatchain.com/core/artist/{actId}/social"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/artist/{actId}/social`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## PUT artist/{actId}/shop

```shell
curl "https://api.beatchain.com/core/artist/{actId}/shop"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/artist/{actId}/shop`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE artist/{actId}/media

```shell
curl "https://api.beatchain.com/core/artist/{actId}/media"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/artist/{actId}/media`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## PUT artist/{actId}/media

```shell
curl "https://api.beatchain.com/core/artist/{actId}/media"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/artist/{actId}/media`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
    
# Artist Email


## GET artistEmail/campaigns/{actId}

```shell
curl "https://api.beatchain.com/core/artistEmail/campaigns/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/artistEmail/campaigns/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE artistEmail/campaigns/{actId}/{campaignId}

```shell
curl "https://api.beatchain.com/core/artistEmail/campaigns/{actId}/{campaignId}"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/artistEmail/campaigns/{actId}/{campaignId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
campaignId |

  
## POST artistEmail/campaigns/{actId}/{campaignId}

```shell
curl "https://api.beatchain.com/core/artistEmail/campaigns/{actId}/{campaignId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/artistEmail/campaigns/{actId}/{campaignId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
campaignId |

  
## POST artistEmail/campaigns/{actId}/{campaignId}/sendtestemail

```shell
curl "https://api.beatchain.com/core/artistEmail/campaigns/{actId}/{campaignId}/sendtestemail"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/artistEmail/campaigns/{actId}/{campaignId}/sendtestemail`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
campaignId |

  
## POST artistEmail/emailFile/{actId}/uploadFileData

```shell
curl "https://api.beatchain.com/core/artistEmail/emailFile/{actId}/uploadFileData"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/artistEmail/emailFile/{actId}/uploadFileData`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET artistEmail/emailFile/signRequest

```shell
curl "https://api.beatchain.com/core/artistEmail/emailFile/signRequest"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/artistEmail/emailFile/signRequest`


  
## POST artistEmail/emailFile/getDataProbe

```shell
curl "https://api.beatchain.com/core/artistEmail/emailFile/getDataProbe"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/artistEmail/emailFile/getDataProbe`


  
    
# Audio


## POST audio/validatetrack

```shell
curl "https://api.beatchain.com/core/audio/validatetrack"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/audio/validatetrack`


  
    
# Distribution


## GET distribution/check

```shell
curl "https://api.beatchain.com/core/distribution/check"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/distribution/check`


  
## GET distribution/count

```shell
curl "https://api.beatchain.com/core/distribution/count"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/distribution/count`


  
## GET distribution/{actId}/releases

```shell
curl "https://api.beatchain.com/core/distribution/{actId}/releases"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/distribution/{actId}/releases`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE distribution/{actId}/{releaseId}

```shell
curl "https://api.beatchain.com/core/distribution/{actId}/{releaseId}"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/distribution/{actId}/{releaseId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
releaseId |

  
## GET distribution/{actId}/{releaseId}

```shell
curl "https://api.beatchain.com/core/distribution/{actId}/{releaseId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/distribution/{actId}/{releaseId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
releaseId |

  
## POST distribution/{actId}/{releaseId}

```shell
curl "https://api.beatchain.com/core/distribution/{actId}/{releaseId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/distribution/{actId}/{releaseId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
releaseId |

  
    
# Download


## GET download/{actId}/getUserDownloads

```shell
curl "https://api.beatchain.com/core/download/{actId}/getUserDownloads"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/download/{actId}/getUserDownloads`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET download/{actId}/email/getMalingListUrl

```shell
curl "https://api.beatchain.com/core/download/{actId}/email/getMalingListUrl"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/download/{actId}/email/getMalingListUrl`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET download/{actId}/email/prepareMailingListFile

```shell
curl "https://api.beatchain.com/core/download/{actId}/email/prepareMailingListFile"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/download/{actId}/email/prepareMailingListFile`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
    
# Entity


## POST entity/graph/search

```shell
curl "https://api.beatchain.com/core/entity/graph/search"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/entity/graph/search`


  
## GET entity/graph/{objectNo}

```shell
curl "https://api.beatchain.com/core/entity/graph/{objectNo}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/entity/graph/{objectNo}`


### Path Parameters

Parameter | Description
--------- | -----------
objectNo |

  
## GET entity/graph/{objectNo}/{itemNo}

```shell
curl "https://api.beatchain.com/core/entity/graph/{objectNo}/{itemNo}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/entity/graph/{objectNo}/{itemNo}`


### Path Parameters

Parameter | Description
--------- | -----------
objectNo |
itemNo |

  
## GET entity/graph/{objectNo}/{itemNo}/related

```shell
curl "https://api.beatchain.com/core/entity/graph/{objectNo}/{itemNo}/related"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/entity/graph/{objectNo}/{itemNo}/related`


### Path Parameters

Parameter | Description
--------- | -----------
objectNo |
itemNo |

  
    
# Facebook


## POST facebook/{actId}/token

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/token"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/facebook/{actId}/token`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE facebook/{actId}/page

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/page"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/facebook/{actId}/page`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST facebook/{actId}/page

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/page"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/facebook/{actId}/page`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE facebook/{actId}/instagram

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/instagram"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/facebook/{actId}/instagram`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST facebook/{actId}/instagram

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/instagram"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/facebook/{actId}/instagram`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET facebook/{actId}/adCampaign/{campaignId}/insights

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/adCampaign/{campaignId}/insights"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/facebook/{actId}/adCampaign/{campaignId}/insights`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
campaignId |

  
## GET facebook/{actId}/adCampaign/{campaignId}/processing

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/adCampaign/{campaignId}/processing"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/facebook/{actId}/adCampaign/{campaignId}/processing`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
campaignId |

  
## POST facebook/{actId}/adCampaign/{campaignId}/pause

```shell
curl "https://api.beatchain.com/core/facebook/{actId}/adCampaign/{campaignId}/pause"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/facebook/{actId}/adCampaign/{campaignId}/pause`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
campaignId |

  
    
# Fanhub


## PUT fanhub/{actId}/config

```shell
curl "https://api.beatchain.com/core/fanhub/{actId}/config"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/fanhub/{actId}/config`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
    
# File


## DELETE file/media

```shell
curl "https://api.beatchain.com/core/file/media"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`DELETE https://api.beatchain.com/core/file/media`


  
## GET file/media

```shell
curl "https://api.beatchain.com/core/file/media"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/file/media`


  
## PUT file/media

```shell
curl "https://api.beatchain.com/core/file/media"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/file/media`


  
## DELETE file/media/{mediaId}

```shell
curl "https://api.beatchain.com/core/file/media/{mediaId}"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`DELETE https://api.beatchain.com/core/file/media/{mediaId}`


### Path Parameters

Parameter | Description
--------- | -----------
mediaId |

  
## GET file/media/{mediaId}

```shell
curl "https://api.beatchain.com/core/file/media/{mediaId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/file/media/{mediaId}`


### Path Parameters

Parameter | Description
--------- | -----------
mediaId |

  
## PUT file/media/{mediaId}

```shell
curl "https://api.beatchain.com/core/file/media/{mediaId}"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/file/media/{mediaId}`


### Path Parameters

Parameter | Description
--------- | -----------
mediaId |

  
## GET file/palette

```shell
curl "https://api.beatchain.com/core/file/palette"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/file/palette`


  
## POST file/pornFilter

```shell
curl "https://api.beatchain.com/core/file/pornFilter"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/file/pornFilter`


  
## GET file/signrequest

```shell
curl "https://api.beatchain.com/core/file/signrequest"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/file/signrequest`


  
    
# Genre


## GET genre/search

```shell
curl "https://api.beatchain.com/core/genre/search"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/genre/search`


  
    
# GraphQL


## GET graphql/server

```shell
curl "https://api.beatchain.com/core/graphql/server"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/graphql/server`


  
## POST graphql/server

```shell
curl "https://api.beatchain.com/core/graphql/server"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/graphql/server`


  
    
# Hypelink


## GET hypelink/{actId}/releases

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/releases"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/hypelink/{actId}/releases`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET hypelink/{actId}/new/{albumId}

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/new/{albumId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/hypelink/{actId}/new/{albumId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
albumId |

  
## POST hypelink/{actId}/new/{albumId}

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/new/{albumId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/hypelink/{actId}/new/{albumId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
albumId |

  
## POST hypelink/{actId}/links/{albumId}

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/links/{albumId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/hypelink/{actId}/links/{albumId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
albumId |

  
## POST hypelink/{actId}/orderlinks/{albumId}

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/orderlinks/{albumId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/hypelink/{actId}/orderlinks/{albumId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
albumId |

  
## POST hypelink/{actId}/player/{albumId}

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/player/{albumId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/hypelink/{actId}/player/{albumId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
albumId |

  
## POST hypelink/{actId}/player/presave/{releaseId}

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/player/presave/{releaseId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/hypelink/{actId}/player/presave/{releaseId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
releaseId |

  
## DELETE hypelink/{actId}/all

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/all"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/hypelink/{actId}/all`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST hypelink/{actId}/all

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/all"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/hypelink/{actId}/all`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET hypelink/{actId}/{hypeLinkId}/analytics

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/analytics"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/analytics`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
hypeLinkId |

  
## GET hypelink/{actId}/{hypeLinkId}/analytics2

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/analytics2"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/analytics2`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
hypeLinkId |

  
## DELETE hypelink/{actId}/{hypeLinkId}/publish

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/publish"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/publish`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
hypeLinkId |

  
## POST hypelink/{actId}/{hypeLinkId}/publish

```shell
curl "https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/publish"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/hypelink/{actId}/{hypeLinkId}/publish`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
hypeLinkId |

  
    
# Launchpad


## GET launchpad/{actId}

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/launchpad/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST launchpad/{actId}

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/launchpad/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## PUT launchpad/{actId}/layout

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}/layout"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/launchpad/{actId}/layout`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE launchpad/{actId}/{launchPadId}

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
launchPadId |

  
## GET launchpad/{actId}/{launchPadId}

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
launchPadId |

  
## POST launchpad/{actId}/{launchPadId}

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
launchPadId |

  
## POST launchpad/{actId}/{launchPadId}/postnow

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}/postnow"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}/postnow`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
launchPadId |

  
## DELETE launchpad/{actId}/{launchPadId}/creative

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}/creative"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}/creative`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
launchPadId |

  
## PUT launchpad/{actId}/{launchPadId}/creative

```shell
curl "https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}/creative"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`PUT https://api.beatchain.com/core/launchpad/{actId}/{launchPadId}/creative`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
launchPadId |

  
    
# Link Tracking


## GET linktracking/{actId}/{linkName}/analytics

```shell
curl "https://api.beatchain.com/core/linktracking/{actId}/{linkName}/analytics"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/linktracking/{actId}/{linkName}/analytics`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
linkName |

  
    
# Location


## GET location/country

```shell
curl "https://api.beatchain.com/core/location/country"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/location/country`


  
## GET location/search

```shell
curl "https://api.beatchain.com/core/location/search"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/location/search`


  
    
# Logging


## POST logging/logevent

```shell
curl "https://api.beatchain.com/core/logging/logevent"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/logging/logevent`


  
    
# Merch


## GET merch/{actId}

```shell
curl "https://api.beatchain.com/core/merch/{actId}"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/merch/{actId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE merch/{actId}/{catalogueId}

```shell
curl "https://api.beatchain.com/core/merch/{actId}/{catalogueId}"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/merch/{actId}/{catalogueId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
catalogueId |

  
## POST merch/{actId}/{catalogueId}

```shell
curl "https://api.beatchain.com/core/merch/{actId}/{catalogueId}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/merch/{actId}/{catalogueId}`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
catalogueId |

  
    
# Payments


## GET payments/payment-rails/{actId}/widget

```shell
curl "https://api.beatchain.com/core/payments/payment-rails/{actId}/widget"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/payments/payment-rails/{actId}/widget`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET payments/payment-rails/{actId}/recipient

```shell
curl "https://api.beatchain.com/core/payments/payment-rails/{actId}/recipient"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/payments/payment-rails/{actId}/recipient`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST payments/payment-rails/{actId}/payout

```shell
curl "https://api.beatchain.com/core/payments/payment-rails/{actId}/payout"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/payments/payment-rails/{actId}/payout`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST payments/stripe/coupon

```shell
curl "https://api.beatchain.com/core/payments/stripe/coupon"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/payments/stripe/coupon`


  
## POST payments/stripe/setup-intent

```shell
curl "https://api.beatchain.com/core/payments/stripe/setup-intent"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/payments/stripe/setup-intent`


  
## PUT payments/stripe/subscription-v2

```shell
curl "https://api.beatchain.com/core/payments/stripe/subscription-v2"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/payments/stripe/subscription-v2`


  
## DELETE payments/stripe/trial

```shell
curl "https://api.beatchain.com/core/payments/stripe/trial"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`DELETE https://api.beatchain.com/core/payments/stripe/trial`


  
## GET payments/stripe/trial

```shell
curl "https://api.beatchain.com/core/payments/stripe/trial"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/payments/stripe/trial`


  
## POST payments/stripe/trial

```shell
curl "https://api.beatchain.com/core/payments/stripe/trial"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/payments/stripe/trial`


  
## POST payments/stripe/trial/without-card

```shell
curl "https://api.beatchain.com/core/payments/stripe/trial/without-card"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/payments/stripe/trial/without-card`


  
## PUT payments/stripe/trial/without-card

```shell
curl "https://api.beatchain.com/core/payments/stripe/trial/without-card"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/payments/stripe/trial/without-card`


  
## POST payments/stripe/trial/without-card/activate

```shell
curl "https://api.beatchain.com/core/payments/stripe/trial/without-card/activate"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/payments/stripe/trial/without-card/activate`


  
## PUT payments/stripe/card

```shell
curl "https://api.beatchain.com/core/payments/stripe/card"
  -X PUT
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PUT https://api.beatchain.com/core/payments/stripe/card`


  
    
# Public


## GET public/butter

```shell
curl "https://api.beatchain.com/core/public/butter"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/butter`


  
## POST public/checkout/create-session

```shell
curl "https://api.beatchain.com/core/public/checkout/create-session"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/public/checkout/create-session`


  
## GET public/distribution/{userId}/{releaseId}

```shell
curl "https://api.beatchain.com/core/public/distribution/{userId}/{releaseId}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/distribution/{userId}/{releaseId}`


### Path Parameters

Parameter | Description
--------- | -----------
userId |
releaseId |

  
## GET public/distribution2/{webAlias}/{releaseSlug}

```shell
curl "https://api.beatchain.com/core/public/distribution2/{webAlias}/{releaseSlug}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/distribution2/{webAlias}/{releaseSlug}`


### Path Parameters

Parameter | Description
--------- | -----------
webAlias |
releaseSlug |

  
## GET public/emailpreview/{emailSnapshotId}

```shell
curl "https://api.beatchain.com/core/public/emailpreview/{emailSnapshotId}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/emailpreview/{emailSnapshotId}`


### Path Parameters

Parameter | Description
--------- | -----------
emailSnapshotId |

  
## GET public/fanhub/{webAlias}

```shell
curl "https://api.beatchain.com/core/public/fanhub/{webAlias}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/fanhub/{webAlias}`


### Path Parameters

Parameter | Description
--------- | -----------
webAlias |

  
## POST public/fanhub/{webAlias}/payments

```shell
curl "https://api.beatchain.com/core/public/fanhub/{webAlias}/payments"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/public/fanhub/{webAlias}/payments`


### Path Parameters

Parameter | Description
--------- | -----------
webAlias |

  
## GET public/hypelink/{hypeLinkId}

```shell
curl "https://api.beatchain.com/core/public/hypelink/{hypeLinkId}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/hypelink/{hypeLinkId}`


### Path Parameters

Parameter | Description
--------- | -----------
hypeLinkId |

  
## POST public/mailinglist/{webAlias}

```shell
curl "https://api.beatchain.com/core/public/mailinglist/{webAlias}"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/public/mailinglist/{webAlias}`


### Path Parameters

Parameter | Description
--------- | -----------
webAlias |

  
## GET public/partners/{slug}

```shell
curl "https://api.beatchain.com/core/public/partners/{slug}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/partners/{slug}`


### Path Parameters

Parameter | Description
--------- | -----------
slug |

  
## POST public/payments/validate-coupon

```shell
curl "https://api.beatchain.com/core/public/payments/validate-coupon"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/public/payments/validate-coupon`


  
## GET public/playlists/{spotifyUserId}

```shell
curl "https://api.beatchain.com/core/public/playlists/{spotifyUserId}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/playlists/{spotifyUserId}`


### Path Parameters

Parameter | Description
--------- | -----------
spotifyUserId |

  
## POST public/presave/{hypeLinkId}

```shell
curl "https://api.beatchain.com/core/public/presave/{hypeLinkId}"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/public/presave/{hypeLinkId}`


### Path Parameters

Parameter | Description
--------- | -----------
hypeLinkId |

  
## POST public/presaveComplete/{hypeLinkId}

```shell
curl "https://api.beatchain.com/core/public/presaveComplete/{hypeLinkId}"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/public/presaveComplete/{hypeLinkId}`


### Path Parameters

Parameter | Description
--------- | -----------
hypeLinkId |

  
## GET public/store/{webAlias}

```shell
curl "https://api.beatchain.com/core/public/store/{webAlias}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/store/{webAlias}`


### Path Parameters

Parameter | Description
--------- | -----------
webAlias |

  
## GET public/tracking_link/{web_alias}/{link_name}

```shell
curl "https://api.beatchain.com/core/public/tracking_link/{web_alias}/{link_name}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/tracking_link/{web_alias}/{link_name}`


### Path Parameters

Parameter | Description
--------- | -----------
web_alias |
link_name |

  
## POST public/unsubscribe

```shell
curl "https://api.beatchain.com/core/public/unsubscribe"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/public/unsubscribe`


  
## GET public/website/{webAlias}

```shell
curl "https://api.beatchain.com/core/public/website/{webAlias}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/website/{webAlias}`


### Path Parameters

Parameter | Description
--------- | -----------
webAlias |

  
## GET public/website/{webAlias}/v2

```shell
curl "https://api.beatchain.com/core/public/website/{webAlias}/v2"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/website/{webAlias}/v2`


### Path Parameters

Parameter | Description
--------- | -----------
webAlias |

  
## GET public/websitefromhost/{host}

```shell
curl "https://api.beatchain.com/core/public/websitefromhost/{host}"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/websitefromhost/{host}`


### Path Parameters

Parameter | Description
--------- | -----------
host |

  
## GET public/websitefromhost/{host}/v2

```shell
curl "https://api.beatchain.com/core/public/websitefromhost/{host}/v2"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/public/websitefromhost/{host}/v2`


### Path Parameters

Parameter | Description
--------- | -----------
host |

  
    
# Signup


## POST signup/account

```shell
curl "https://api.beatchain.com/core/signup/account"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/signup/account`


  
## POST signup/hubspot

```shell
curl "https://api.beatchain.com/core/signup/hubspot"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/signup/hubspot`


  
    
# TV Stats


## GET tvStats/dashboard

```shell
curl "https://api.beatchain.com/core/tvStats/dashboard"
  -X GET
  
```



### Security
Public endpoint.

### HTTP Request

`GET https://api.beatchain.com/core/tvStats/dashboard`


  
    
# Twitter


## POST twitter/signin

```shell
curl "https://api.beatchain.com/core/twitter/signin"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/twitter/signin`


  
## DELETE twitter/{actId}/token

```shell
curl "https://api.beatchain.com/core/twitter/{actId}/token"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/twitter/{actId}/token`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET twitter/{actId}/token

```shell
curl "https://api.beatchain.com/core/twitter/{actId}/token"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/twitter/{actId}/token`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
    
# User


## POST user/confirm

```shell
curl "https://api.beatchain.com/core/user/confirm"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/confirm`


  
## DELETE user/delete

```shell
curl "https://api.beatchain.com/core/user/delete"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`DELETE https://api.beatchain.com/core/user/delete`


  
## POST user/force_change_password_finish

```shell
curl "https://api.beatchain.com/core/user/force_change_password_finish"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/force_change_password_finish`


  
## DELETE user/locked-out-acts

```shell
curl "https://api.beatchain.com/core/user/locked-out-acts"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`DELETE https://api.beatchain.com/core/user/locked-out-acts`


  
## GET user/me

```shell
curl "https://api.beatchain.com/core/user/me"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/user/me`


  
## PATCH user/me

```shell
curl "https://api.beatchain.com/core/user/me"
  -X PATCH
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`PATCH https://api.beatchain.com/core/user/me`


  
## POST user/me/act

```shell
curl "https://api.beatchain.com/core/user/me/act"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/me/act`


  
## POST user/referral_code

```shell
curl "https://api.beatchain.com/core/user/referral_code"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/referral_code`


  
## GET user/reset

```shell
curl "https://api.beatchain.com/core/user/reset"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/user/reset`


  
## POST user/reset/act

```shell
curl "https://api.beatchain.com/core/user/reset/act"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/reset/act`


  
## POST user/survey

```shell
curl "https://api.beatchain.com/core/user/survey"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/survey`


  
## GET user/verification-email

```shell
curl "https://api.beatchain.com/core/user/verification-email"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/user/verification-email`


  
## POST user/verification-email

```shell
curl "https://api.beatchain.com/core/user/verification-email"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/verification-email`


  
## POST user/wipe

```shell
curl "https://api.beatchain.com/core/user/wipe"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/user/wipe`


  
    
# Warehouse


## GET warehouse/analytics/{actId}/fuga

```shell
curl "https://api.beatchain.com/core/warehouse/analytics/{actId}/fuga"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/warehouse/analytics/{actId}/fuga`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET warehouse/analytics/{actId}/website

```shell
curl "https://api.beatchain.com/core/warehouse/analytics/{actId}/website"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/warehouse/analytics/{actId}/website`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
    
# Webhooks


## POST webhooks/butter

```shell
curl "https://api.beatchain.com/core/webhooks/butter"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/webhooks/butter`


  
## POST webhooks/payment-rails

```shell
curl "https://api.beatchain.com/core/webhooks/payment-rails"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/webhooks/payment-rails`


  
## POST webhooks/slack

```shell
curl "https://api.beatchain.com/core/webhooks/slack"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/webhooks/slack`


  
## POST webhooks/stripe

```shell
curl "https://api.beatchain.com/core/webhooks/stripe"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/webhooks/stripe`


  
## POST webhooks/stripe/{account}

```shell
curl "https://api.beatchain.com/core/webhooks/stripe/{account}"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`POST https://api.beatchain.com/core/webhooks/stripe/{account}`


### Path Parameters

Parameter | Description
--------- | -----------
account |

  
## POST webhooks/webflow

```shell
curl "https://api.beatchain.com/core/webhooks/webflow"
  -X POST
  
```



### Security
Public endpoint.

### HTTP Request

`POST https://api.beatchain.com/core/webhooks/webflow`


  
    
# Website


## GET website/fonts

```shell
curl "https://api.beatchain.com/core/website/fonts"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication.

### HTTP Request

`GET https://api.beatchain.com/core/website/fonts`


  
## GET website/{actId}/config

```shell
curl "https://api.beatchain.com/core/website/{actId}/config"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/website/{actId}/config`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST website/{actId}/config

```shell
curl "https://api.beatchain.com/core/website/{actId}/config"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/website/{actId}/config`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## DELETE website/{actId}/custom_domain

```shell
curl "https://api.beatchain.com/core/website/{actId}/custom_domain"
  -X DELETE
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`DELETE https://api.beatchain.com/core/website/{actId}/custom_domain`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## GET website/{actId}/custom_domain

```shell
curl "https://api.beatchain.com/core/website/{actId}/custom_domain"
  -X GET
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`GET https://api.beatchain.com/core/website/{actId}/custom_domain`


### Path Parameters

Parameter | Description
--------- | -----------
actId |

  
## POST website/{actId}/custom_domain

```shell
curl "https://api.beatchain.com/core/website/{actId}/custom_domain"
  -X POST
  -H "Authorization: Bearer_Token"
```



### Security
Bearer token authentication and access to actId specified in path required.

### HTTP Request

`POST https://api.beatchain.com/core/website/{actId}/custom_domain`


### Path Parameters

Parameter | Description
--------- | -----------
actId |
