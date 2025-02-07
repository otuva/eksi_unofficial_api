# Ekşisözlük Unofficial API Documentation - 2021

Version 1 of this documentation has been [deprecated](doc/V1.md).

Version 2 is [documented on Postman](https://documenter.getpostman.com/view/6963920/TzzEoZpq).

The Version 2 collection can be   [![collection](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/6963920-32242d64-126b-4382-8fb1-0501844f107a?action=collection%2Ffork&collection-url=entityId%3D6963920-32242d64-126b-4382-8fb1-0501844f107a%26entityType%3Dcollection%26workspaceId%3De549a4c7-acfa-45b4-8689-4599ee859e9a).

This library is a work in progress, any contribution are welcome.

# EksiSozluk.py

### Installation

```shell
pip install eksisozluk
```

### Usage

```python
from eksisozluk.EksiSozluk import EksiApi

client = EksiApi()  # or EksiApi(username, password)

entry = client.get_entry( < entry_id >)
topic = client.get_topic( < topic_id >, < page >)
author = client.get_user( < user_nick >)
```

```
(büyük t)oken
/v2/account/anonymoustoken
/v2/account/canregisternick/
/v2/account/login/facebook
/v2/account/logout
/v2/account/register
/v2/account/register/facebook
/v2/azure/register
/v2/azure/unregister
/v2/billing/subscription/anonymousstatus
/v2/billing/subscription/playstore/purchase
/v2/billing/subscription/status
/v2/billing/subscription/transfer/playstore
/v2/entry/favorite
/v2/entry/unfavorite
/v2/image/upload <--- resim yükleme şeysi.
/v2/matter/answer/delete
/v2/matter/delete
/v2/message/recipientinfo/{nick}
/v2/message/unreadthreadauthors
/v2/settings/get/personal
/v2/settings/get/preferences
/v2/settings/hide/facebook
/v2/settings/hide/instagram
/v2/settings/hide/twitter
/v2/settings/link/facebook
/v2/settings/link/instagram
/v2/settings/link/twitter
/v2/settings/reset/email
/v2/settings/reset/password
/v2/settings/set/personal
/v2/settings/set/preferences
/v2/settings/show/facebook
/v2/settings/show/instagram
/v2/settings/show/twitter
/v2/settings/twitter/authorizationurl
/v2/settings/unlink/facebook
/v2/settings/unlink/instagram
/v2/settings/unlink/twitter
/v2/user/add-pinned-entry
/v2/user/blocks
/v2/user/buddies
/v2/user/index-title-blocks
/v2/user/isdeveloper
/v2/user/remove-pinned-entry
/v2/user/remove/avatar
/v2/user/upload/avatar <--- resim yükleme şeysi.
v2/autocomplete/nick/{querystring}
v2/autocomplete/query/{querystring}
v2/azure/getregistrationid
v2/channel/list
v2/clientsettings/info
v2/comment/add
v2/comment/delete
v2/comment/edit
v2/comment/list/{entryıd}/
v2/comment/removevote/
v2/comment/vote/
v2/entry/add
v2/entry/delete
v2/entry/edit
v2/entry/edit/{entryıd}
v2/entry/vote
v2/entry/vote/remove
v2/entry/{entryıd}/
v2/entry/{entryıd}/caylakfavorites
v2/entry/{entryıd}/favorites
v2/image/delete
v2/index/getfilterchannels
v2/index/getuserchannelfilters
v2/index/popular/
v2/index/search/
v2/index/setchannelfilter
v2/index/{querypath}/
v2/matter/add
v2/matter/answer/add
v2/matter/answer/edit
v2/matter/answer/vote/
v2/matter/answer/vote/remove/
v2/matter/answer/{matterıd}
v2/matter/edit
v2/matter/follow
v2/matter/query/
v2/matter/unfollow
v2/matter/vote/
v2/matter/vote/remove
v2/matter/{matterıd}/{actionname}/
v2/matterindex/{topicıd}/{actionname}/
v2/message/archive
v2/message/archiveprocessthread
v2/message/archivethread/nick/{username}
v2/message/deleteprocessarchive
v2/message/deleteprocessthread
v2/message/markread/nick
v2/message/reportarchivedmessages
v2/message/reportmessages
v2/message/sendmessage
v2/message/thread/nick/{username}
v2/message/thread/unread
v2/message/{searchpath}
v2/pushnotification/register
v2/pushnotification/unregister
v2/topic/deletedraft
v2/topic/follow
v2/topic/query/
v2/topic/savedraft
v2/topic/unfollow
v2/topic/unreadtopiccount
v2/topic/{topicıd}/{actionname}
v2/trash
v2/trash/delete
v2/trash/empty
v2/user/block
v2/user/follow
v2/user/indextitlesblock
v2/user/removeindextitlesblock
v2/user/unblock
v2/user/unfollow
v2/user/{username}/
v2/user/{username}//images
v2/user/{username}/{actionname}/
v2/{actionname}
```
