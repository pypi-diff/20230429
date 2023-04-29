# Comparing `tmp/esi_client-0.1.0a1.tar.gz` & `tmp/esi_client-0.1.0a2.tar.gz`

## Comparing `esi_client-0.1.0a1.tar` & `esi_client-0.1.0a2.tar`

### file list

```diff
@@ -1,1138 +1,1138 @@
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/__init__.py
--rw-r--r--   0        0        0    39119 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api_client.py
--rw-r--r--   0        0        0    16447 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/configuration.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/exceptions.py
--rw-r--r--   0        0        0    82553 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model_utils.py
--rw-r--r--   0        0        0    14230 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/rest.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/__init__.py
--rw-r--r--   0        0        0    26044 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/alliance_api.py
--rw-r--r--   0        0        0    44642 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/assets_api.py
--rw-r--r--   0        0        0    30304 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/bookmarks_api.py
--rw-r--r--   0        0        0    30943 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/calendar_api.py
--rw-r--r--   0        0        0    95070 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/character_api.py
--rw-r--r--   0        0        0    14596 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/clones_api.py
--rw-r--r--   0        0        0    66232 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/contacts_api.py
--rw-r--r--   0        0        0    67661 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/contracts_api.py
--rw-r--r--   0        0        0   156673 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/corporation_api.py
--rw-r--r--   0        0        0    31563 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/dogma_api.py
--rw-r--r--   0        0        0    49800 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/faction_warfare_api.py
--rw-r--r--   0        0        0    21482 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/fittings_api.py
--rw-r--r--   0        0        0    97465 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/fleets_api.py
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/incursions_api.py
--rw-r--r--   0        0        0    57957 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/industry_api.py
--rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/insurance_api.py
--rw-r--r--   0        0        0    22976 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/killmails_api.py
--rw-r--r--   0        0        0    21634 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/location_api.py
--rw-r--r--   0        0        0    14814 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/loyalty_api.py
--rw-r--r--   0        0        0    63735 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/mail_api.py
--rw-r--r--   0        0        0    77534 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/market_api.py
--rw-r--r--   0        0        0    33307 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/opportunities_api.py
--rw-r--r--   0        0        0    29021 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/planetary_interaction_api.py
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/routes_api.py
--rw-r--r--   0        0        0    11532 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/search_api.py
--rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/skills_api.py
--rw-r--r--   0        0        0    18391 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/sovereignty_api.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/status_api.py
--rw-r--r--   0        0        0   198686 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/universe_api.py
--rw-r--r--   0        0        0    32604 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/user_interface_api.py
--rw-r--r--   0        0        0    45436 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/wallet_api.py
--rw-r--r--   0        0        0    19820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/api/wars_api.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/apis/__init__.py
--rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/AllianceApi.md
--rw-r--r--   0        0        0    31173 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/AssetsApi.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/BadRequest.md
--rw-r--r--   0        0        0    22756 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/BookmarksApi.md
--rw-r--r--   0        0        0    22607 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/CalendarApi.md
--rw-r--r--   0        0        0    69568 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/CharacterApi.md
--rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/ClonesApi.md
--rw-r--r--   0        0        0    47082 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/ContactsApi.md
--rw-r--r--   0        0        0    51239 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/ContractsApi.md
--rw-r--r--   0        0        0   118362 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/CorporationApi.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/DeleteCharactersCharacterIdMailLabelsLabelIdUnprocessableEntity.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/DeleteFleetsFleetIdMembersMemberIdNotFound.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/DeleteFleetsFleetIdSquadsSquadIdNotFound.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/DeleteFleetsFleetIdWingsWingIdNotFound.md
--rw-r--r--   0        0        0    20565 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/DogmaApi.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/ErrorLimited.md
--rw-r--r--   0        0        0    34440 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/FactionWarfareApi.md
--rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/FittingsApi.md
--rw-r--r--   0        0        0    69064 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/FleetsApi.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/Forbidden.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GatewayTimeout.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdContacts200Ok.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdContactsLabels200Ok.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdIconsNotFound.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdIconsOk.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdNotFound.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdOk.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAgentsResearch200Ok.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAssets200Ok.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAssetsNotFound.md
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAttributesOk.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBlueprints200Ok.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarks200Ok.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarksCoordinates.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarksFolders200Ok.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarksItem.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendar200Ok.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendees200Ok.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendeesNotFound.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdNotFound.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdOk.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdClonesHomeLocation.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdClonesJumpClone.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdClonesOk.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContacts200Ok.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContactsLabels200Ok.md
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContracts200Ok.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdBids200Ok.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdBidsNotFound.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdItems200Ok.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdItemsNotFound.md
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCorporationhistory200Ok.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFatigueOk.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFittings200Ok.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFittingsItem.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFleetNotFound.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFleetOk.md
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFwStatsKills.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFwStatsOk.md
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFwStatsVictoryPoints.md
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdIndustryJobs200Ok.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdKillmailsRecent200Ok.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdLocationOk.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdLoyaltyPoints200Ok.md
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMail200Ok.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailLabelsLabel.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailLabelsOk.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailLists200Ok.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailMailIdNotFound.md
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailMailIdOk.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailMailIdRecipient.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailRecipient.md
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMedals200Ok.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMedalsGraphic.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMining200Ok.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdNotFound.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdNotifications200Ok.md
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdNotificationsContacts200Ok.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOk.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOnlineOk.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOpportunities200Ok.md
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOrders200Ok.md
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOrdersHistory200Ok.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanets200Ok.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdContent.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdExtractorDetails.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdFactoryDetails.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdHead.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdLink.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdNotFound.md
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdOk.md
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdPin.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdRoute.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPortraitNotFound.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPortraitOk.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdRolesOk.md
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSearchOk.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdShipOk.md
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSkillqueue200Ok.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSkillsOk.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSkillsSkill.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdStandings200Ok.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdTitles200Ok.md
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdWalletJournal200Ok.md
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdWalletTransactions200Ok.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicBidsContractId200Ok.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicBidsContractIdForbidden.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicBidsContractIdNotFound.md
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicItemsContractId200Ok.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicItemsContractIdForbidden.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicItemsContractIdNotFound.md
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicRegionId200Ok.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetContractsPublicRegionIdNotFound.md
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationCorporationIdMiningExtractions200Ok.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationCorporationIdMiningObservers200Ok.md
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationCorporationIdMiningObserversObserverId200Ok.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdAlliancehistory200Ok.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdAssets200Ok.md
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBlueprints200Ok.md
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarks200Ok.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarksCoordinates.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarksFolders200Ok.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarksItem.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContacts200Ok.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContactsLabels200Ok.md
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContainersLogs200Ok.md
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContracts200Ok.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBids200Ok.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBidsNotFound.md
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItems200Ok.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsError520.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsNotFound.md
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdCustomsOffices200Ok.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdDivisionsHangarHangar.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdDivisionsOk.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdDivisionsWalletWallet.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFacilities200Ok.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFwStatsKills.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFwStatsOk.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFwStatsVictoryPoints.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdIconsNotFound.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdIconsOk.md
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdIndustryJobs200Ok.md
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdKillmailsRecent200Ok.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMedals200Ok.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMedalsIssued200Ok.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMembersTitles200Ok.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMembertracking200Ok.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdNotFound.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdOk.md
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdOrders200Ok.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdOrdersHistory200Ok.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdRoles200Ok.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdRolesHistory200Ok.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdShareholders200Ok.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStandings200Ok.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStarbases200Ok.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdFuel.md
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdOk.md
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStructures200Ok.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStructuresService.md
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdTitles200Ok.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdWallets200Ok.md
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionJournal200Ok.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionTransactions200Ok.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaAttributesAttributeIdNotFound.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaAttributesAttributeIdOk.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaAttribute.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaEffect.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdNotFound.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdOk.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaEffectsEffectIdModifier.md
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaEffectsEffectIdNotFound.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetDogmaEffectsEffectIdOk.md
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdMembers200Ok.md
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdMembersNotFound.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdNotFound.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdOk.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdWings200Ok.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdWingsNotFound.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdWingsSquad.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal1.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal1.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersKills.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek1.md
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersOk.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersVictoryPoints.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday1.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal1.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsKills.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek.md
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek1.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsOk.md
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsVictoryPoints.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday1.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsKills.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek1.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsOk.md
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsVictoryPoints.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsYesterdayYesterday.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsYesterdayYesterday1.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwStats200Ok.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwStatsKills.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwStatsVictoryPoints.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwSystems200Ok.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetFwWars200Ok.md
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetIncursions200Ok.md
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetIndustryFacilities200Ok.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetIndustrySystems200Ok.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetIndustrySystemsCostIndice.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetInsurancePrices200Ok.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetInsurancePricesLevel.md
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashAttacker.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashItem.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashItemsItem.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashOk.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashPosition.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashUnprocessableEntity.md
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashVictim.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetLoyaltyStoresCorporationIdOffers200Ok.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetLoyaltyStoresCorporationIdOffersNotFound.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetLoyaltyStoresCorporationIdOffersRequiredItem.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsGroupsMarketGroupIdNotFound.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsGroupsMarketGroupIdOk.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsPrices200Ok.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistory200Ok.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistoryError520.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistoryNotFound.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistoryUnprocessableEntity.md
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdOrders200Ok.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdOrdersNotFound.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdOrdersUnprocessableEntity.md
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetMarketsStructuresStructureId200Ok.md
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetOpportunitiesGroupsGroupIdOk.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetOpportunitiesTasksTaskIdOk.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetRouteOriginDestinationNotFound.md
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetSovereigntyCampaigns200Ok.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetSovereigntyCampaignsParticipant.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetSovereigntyMap200Ok.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetSovereigntyStructures200Ok.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetStatusOk.md
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseAncestries200Ok.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdNotFound.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdOk.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdPosition.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseBloodlines200Ok.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseCategoriesCategoryIdNotFound.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseCategoriesCategoryIdOk.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseConstellationsConstellationIdNotFound.md
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseConstellationsConstellationIdOk.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseConstellationsConstellationIdPosition.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseFactions200Ok.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseGraphicsGraphicIdNotFound.md
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseGraphicsGraphicIdOk.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseGroupsGroupIdNotFound.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseGroupsGroupIdOk.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseMoonsMoonIdNotFound.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseMoonsMoonIdOk.md
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseMoonsMoonIdPosition.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniversePlanetsPlanetIdNotFound.md
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniversePlanetsPlanetIdOk.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniversePlanetsPlanetIdPosition.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseRaces200Ok.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseRegionsRegionIdNotFound.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseRegionsRegionIdOk.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSchematicsSchematicIdNotFound.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSchematicsSchematicIdOk.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdDestination.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdNotFound.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdOk.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdPosition.md
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStarsStarIdOk.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStationsStationIdNotFound.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStationsStationIdOk.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStationsStationIdPosition.md
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStructuresStructureIdNotFound.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStructuresStructureIdOk.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseStructuresStructureIdPosition.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemJumps200Ok.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemKills200Ok.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdNotFound.md
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdOk.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdPlanet.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdPosition.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdDogmaAttribute.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdDogmaEffect.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdNotFound.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdOk.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdAggressor.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdAlly.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdDefender.md
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdKillmails200Ok.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdKillmailsUnprocessableEntity.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdOk.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdUnprocessableEntity.md
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/IncursionsApi.md
--rw-r--r--   0        0        0    43038 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/IndustryApi.md
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/InsuranceApi.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/InternalServerError.md
--rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/KillmailsApi.md
--rw-r--r--   0        0        0    16093 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/LocationApi.md
--rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/LoyaltyApi.md
--rw-r--r--   0        0        0    45241 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/MailApi.md
--rw-r--r--   0        0        0    55150 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/MarketApi.md
--rw-r--r--   0        0        0    22205 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/OpportunitiesApi.md
--rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PlanetaryInteractionApi.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersAffiliation200Ok.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdAssetsLocations200Ok.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdAssetsLocationsPosition.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdAssetsNames200Ok.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdContactsError520.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdFittingsCreated.md
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdFittingsFitting.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdFittingsItem.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailError520.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailLabelsLabel.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailMail.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailRecipient.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsLocations200Ok.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsNotFound.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsPosition.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsNames200Ok.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsNamesNotFound.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdMembersInvitation.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdMembersNotFound.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdMembersUnprocessableEntity.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsCreated.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsNotFound.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsCreated.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsNotFound.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUiOpenwindowNewmailNewMail.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUiOpenwindowNewmailUnprocessableEntity.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsAgent.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsAlliance.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsCharacter.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsConstellation.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsCorporation.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsFaction.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsInventoryType.md
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsOk.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsRegion.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsStation.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsSystem.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseNames200Ok.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PostUniverseNamesNotFound.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutCharactersCharacterIdCalendarEventIdResponse.md
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutCharactersCharacterIdMailMailIdContents.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdMembersMemberIdMovement.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdMembersMemberIdNotFound.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdMembersMemberIdUnprocessableEntity.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdNewSettings.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdNotFound.md
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNaming.md
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNotFound.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdWingsWingIdNaming.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdWingsWingIdNotFound.md
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/RoutesApi.md
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/SearchApi.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/ServiceUnavailable.md
--rw-r--r--   0        0        0    15883 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/SkillsApi.md
--rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/SovereigntyApi.md
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/StatusApi.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/Unauthorized.md
--rw-r--r--   0        0        0   128481 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/UniverseApi.md
--rw-r--r--   0        0        0    21635 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/UserInterfaceApi.md
--rw-r--r--   0        0        0    34300 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/WalletApi.md
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/docs/WarsApi.md
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/__init__.py
--rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/bad_request.py
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/delete_fleets_fleet_id_members_member_id_not_found.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/delete_fleets_fleet_id_squads_squad_id_not_found.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/delete_fleets_fleet_id_wings_wing_id_not_found.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/error_limited.py
--rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/forbidden.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/gateway_timeout.py
--rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_contacts200_ok.py
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_contacts_labels200_ok.py
--rw-r--r--   0        0        0    11452 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_icons_not_found.py
--rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_icons_ok.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_not_found.py
--rw-r--r--   0        0        0    13714 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_ok.py
--rw-r--r--   0        0        0    12927 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_agents_research200_ok.py
--rw-r--r--   0        0        0    17483 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_assets200_ok.py
--rw-r--r--   0        0        0    11461 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_assets_not_found.py
--rw-r--r--   0        0        0    13829 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_attributes_ok.py
--rw-r--r--   0        0        0    18552 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_blueprints200_ok.py
--rw-r--r--   0        0        0    14275 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks200_ok.py
--rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks_coordinates.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks_folders200_ok.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks_item.py
--rw-r--r--   0        0        0    12671 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar200_ok.py
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_attendees200_ok.py
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_attendees_not_found.py
--rw-r--r--   0        0        0    11496 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_not_found.py
--rw-r--r--   0        0        0    14135 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_ok.py
--rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_clones_home_location.py
--rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_clones_jump_clone.py
--rw-r--r--   0        0        0    13287 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_clones_ok.py
--rw-r--r--   0        0        0    13378 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contacts200_ok.py
--rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contacts_labels200_ok.py
--rw-r--r--   0        0        0    19129 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts200_ok.py
--rw-r--r--   0        0        0    12454 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_bids200_ok.py
--rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_bids_not_found.py
--rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_items200_ok.py
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_items_not_found.py
--rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_corporationhistory200_ok.py
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fatigue_ok.py
--rw-r--r--   0        0        0    13070 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fittings200_ok.py
--rw-r--r--   0        0        0    13665 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fittings_item.py
--rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fleet_not_found.py
--rw-r--r--   0        0        0    12760 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fleet_ok.py
--rw-r--r--   0        0        0    12465 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fw_stats_kills.py
--rw-r--r--   0        0        0    14311 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fw_stats_ok.py
--rw-r--r--   0        0        0    12341 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fw_stats_victory_points.py
--rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_industry_jobs200_ok.py
--rw-r--r--   0        0        0    11940 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_killmails_recent200_ok.py
--rw-r--r--   0        0        0    12135 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_location_ok.py
--rw-r--r--   0        0        0    11982 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_loyalty_points200_ok.py
--rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail200_ok.py
--rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_labels_label.py
--rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_labels_ok.py
--rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_lists200_ok.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_mail_id_not_found.py
--rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_mail_id_ok.py
--rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_mail_id_recipient.py
--rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_recipient.py
--rw-r--r--   0        0        0    14242 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_medals200_ok.py
--rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_medals_graphic.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mining200_ok.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_not_found.py
--rw-r--r--   0        0        0    26376 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_notifications200_ok.py
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_notifications_contacts200_ok.py
--rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_ok.py
--rw-r--r--   0        0        0    12388 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_online_ok.py
--rw-r--r--   0        0        0    11878 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_opportunities200_ok.py
--rw-r--r--   0        0        0    16413 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_orders200_ok.py
--rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_orders_history200_ok.py
--rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets200_ok.py
--rw-r--r--   0        0        0    11799 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_content.py
--rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_extractor_details.py
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_factory_details.py
--rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_head.py
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_link.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_not_found.py
--rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_ok.py
--rw-r--r--   0        0        0    15535 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_pin.py
--rw-r--r--   0        0        0    13252 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_route.py
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_portrait_not_found.py
--rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_portrait_ok.py
--rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_roles_ok.py
--rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_search_ok.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_ship_ok.py
--rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_skillqueue200_ok.py
--rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_skills_ok.py
--rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_skills_skill.py
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_standings200_ok.py
--rw-r--r--   0        0        0    11677 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_titles200_ok.py
--rw-r--r--   0        0        0    25772 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_wallet_journal200_ok.py
--rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_characters_character_id_wallet_transactions200_ok.py
--rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_bids_contract_id200_ok.py
--rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_bids_contract_id_forbidden.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_bids_contract_id_not_found.py
--rw-r--r--   0        0        0    14728 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_items_contract_id200_ok.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_items_contract_id_forbidden.py
--rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_items_contract_id_not_found.py
--rw-r--r--   0        0        0    16429 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_region_id200_ok.py
--rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_contracts_public_region_id_not_found.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporation_corporation_id_mining_extractions200_ok.py
--rw-r--r--   0        0        0    12715 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporation_corporation_id_mining_observers200_ok.py
--rw-r--r--   0        0        0    13062 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporation_corporation_id_mining_observers_observer_id200_ok.py
--rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_alliancehistory200_ok.py
--rw-r--r--   0        0        0    19003 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_assets200_ok.py
--rw-r--r--   0        0        0    19930 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_blueprints200_ok.py
--rw-r--r--   0        0        0    14343 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks200_ok.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks_coordinates.py
--rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks_folders200_ok.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks_item.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contacts200_ok.py
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contacts_labels200_ok.py
--rw-r--r--   0        0        0    20654 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_containers_logs200_ok.py
--rw-r--r--   0        0        0    19121 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts200_ok.py
--rw-r--r--   0        0        0    12466 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids200_ok.py
--rw-r--r--   0        0        0    11532 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids_not_found.py
--rw-r--r--   0        0        0    13534 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items200_ok.py
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_error520.py
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_not_found.py
--rw-r--r--   0        0        0    17531 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_customs_offices200_ok.py
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_divisions_hangar_hangar.py
--rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_divisions_ok.py
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_divisions_wallet_wallet.py
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_facilities200_ok.py
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_fw_stats_kills.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_fw_stats_ok.py
--rw-r--r--   0        0        0    12409 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_fw_stats_victory_points.py
--rw-r--r--   0        0        0    11470 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_icons_not_found.py
--rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_icons_ok.py
--rw-r--r--   0        0        0    19518 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_industry_jobs200_ok.py
--rw-r--r--   0        0        0    11952 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_killmails_recent200_ok.py
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_medals200_ok.py
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_medals_issued200_ok.py
--rw-r--r--   0        0        0    11941 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_members_titles200_ok.py
--rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_membertracking200_ok.py
--rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_not_found.py
--rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_ok.py
--rw-r--r--   0        0        0    16819 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_orders200_ok.py
--rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_orders_history200_ok.py
--rw-r--r--   0        0        0    33972 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_roles200_ok.py
--rw-r--r--   0        0        0    18571 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_roles_history200_ok.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_shareholders200_ok.py
--rw-r--r--   0        0        0    12233 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_standings200_ok.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_starbases200_ok.py
--rw-r--r--   0        0        0    11840 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_fuel.py
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_ok.py
--rw-r--r--   0        0        0    18352 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_structures200_ok.py
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_structures_service.py
--rw-r--r--   0        0        0    34063 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_titles200_ok.py
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_wallets200_ok.py
--rw-r--r--   0        0        0    26391 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_wallets_division_journal200_ok.py
--rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_wallets_division_transactions200_ok.py
--rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_attributes_attribute_id_not_found.py
--rw-r--r--   0        0        0    13774 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_attributes_attribute_id_ok.py
--rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py
--rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_effect.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_not_found.py
--rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_ok.py
--rw-r--r--   0        0        0    12821 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_effects_effect_id_modifier.py
--rw-r--r--   0        0        0    11448 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_effects_effect_id_not_found.py
--rw-r--r--   0        0        0    17527 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_dogma_effects_effect_id_ok.py
--rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_members200_ok.py
--rw-r--r--   0        0        0    11448 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_members_not_found.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_not_found.py
--rw-r--r--   0        0        0    12556 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_ok.py
--rw-r--r--   0        0        0    12251 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_wings200_ok.py
--rw-r--r--   0        0        0    11442 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_wings_not_found.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_wings_squad.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_active_total_active_total.py
--rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_active_total_active_total1.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_active_total_active_total.py
--rw-r--r--   0        0        0    11786 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_active_total_active_total1.py
--rw-r--r--   0        0        0    13971 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_kills.py
--rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_last_week_last_week.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_last_week_last_week1.py
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_ok.py
--rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_victory_points.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday.py
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday1.py
--rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total1.py
--rw-r--r--   0        0        0    14058 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_kills.py
--rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week.py
--rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week1.py
--rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_ok.py
--rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_victory_points.py
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday.py
--rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday1.py
--rw-r--r--   0        0        0    13726 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_kills.py
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_last_week_last_week.py
--rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_last_week_last_week1.py
--rw-r--r--   0        0        0    12251 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_ok.py
--rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_victory_points.py
--rw-r--r--   0        0        0    11709 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_yesterday_yesterday.py
--rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_yesterday_yesterday1.py
--rw-r--r--   0        0        0    13199 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_stats200_ok.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_stats_kills.py
--rw-r--r--   0        0        0    12172 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_stats_victory_points.py
--rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_systems200_ok.py
--rw-r--r--   0        0        0    11830 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_fw_wars200_ok.py
--rw-r--r--   0        0        0    14393 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_incursions200_ok.py
--rw-r--r--   0        0        0    13029 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_industry_facilities200_ok.py
--rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_industry_systems200_ok.py
--rw-r--r--   0        0        0    12350 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_industry_systems_cost_indice.py
--rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_insurance_prices200_ok.py
--rw-r--r--   0        0        0    11941 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_insurance_prices_level.py
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_attacker.py
--rw-r--r--   0        0        0    13500 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_item.py
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_items_item.py
--rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_ok.py
--rw-r--r--   0        0        0    11833 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_position.py
--rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_unprocessable_entity.py
--rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_victim.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_loyalty_stores_corporation_id_offers200_ok.py
--rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_loyalty_stores_corporation_id_offers_not_found.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_loyalty_stores_corporation_id_offers_required_item.py
--rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_groups_market_group_id_not_found.py
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_groups_market_group_id_ok.py
--rw-r--r--   0        0        0    12035 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_prices200_ok.py
--rw-r--r--   0        0        0    12872 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history200_ok.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history_error520.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history_not_found.py
--rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history_unprocessable_entity.py
--rw-r--r--   0        0        0    15004 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_region_id_orders200_ok.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_region_id_orders_not_found.py
--rw-r--r--   0        0        0    11506 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_region_id_orders_unprocessable_entity.py
--rw-r--r--   0        0        0    14702 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_markets_structures_structure_id200_ok.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_opportunities_groups_group_id_ok.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_opportunities_tasks_task_id_ok.py
--rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_route_origin_destination_not_found.py
--rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_sovereignty_campaigns200_ok.py
--rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_sovereignty_campaigns_participant.py
--rw-r--r--   0        0        0    12290 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_sovereignty_map200_ok.py
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_sovereignty_structures200_ok.py
--rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_status_ok.py
--rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_ancestries200_ok.py
--rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_not_found.py
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_ok.py
--rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_position.py
--rw-r--r--   0        0        0    14440 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_bloodlines200_ok.py
--rw-r--r--   0        0        0    11472 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_categories_category_id_not_found.py
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_categories_category_id_ok.py
--rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_constellations_constellation_id_not_found.py
--rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_constellations_constellation_id_ok.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_constellations_constellation_id_position.py
--rw-r--r--   0        0        0    14292 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_factions200_ok.py
--rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_graphics_graphic_id_not_found.py
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_graphics_graphic_id_ok.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_groups_group_id_not_found.py
--rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_groups_group_id_ok.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_moons_moon_id_not_found.py
--rw-r--r--   0        0        0    12576 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_moons_moon_id_ok.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_moons_moon_id_position.py
--rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_planets_planet_id_not_found.py
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_planets_planet_id_ok.py
--rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_planets_planet_id_position.py
--rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_races200_ok.py
--rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_regions_region_id_not_found.py
--rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_regions_region_id_ok.py
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_schematics_schematic_id_not_found.py
--rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_schematics_schematic_id_ok.py
--rw-r--r--   0        0        0    11963 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_destination.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_not_found.py
--rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_ok.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_position.py
--rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stars_star_id_ok.py
--rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stations_station_id_not_found.py
--rw-r--r--   0        0        0    16824 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stations_station_id_ok.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_stations_station_id_position.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_structures_structure_id_not_found.py
--rw-r--r--   0        0        0    13054 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_structures_structure_id_ok.py
--rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_structures_structure_id_position.py
--rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_system_jumps200_ok.py
--rw-r--r--   0        0        0    12520 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_system_kills200_ok.py
--rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_not_found.py
--rw-r--r--   0        0        0    14782 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_ok.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_planet.py
--rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_position.py
--rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_dogma_attribute.py
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_dogma_effect.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_not_found.py
--rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_ok.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_wars_war_id_aggressor.py
--rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_wars_war_id_ally.py
--rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_wars_war_id_defender.py
--rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_wars_war_id_killmails200_ok.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_wars_war_id_killmails_unprocessable_entity.py
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_wars_war_id_ok.py
--rw-r--r--   0        0        0    11470 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/get_wars_war_id_unprocessable_entity.py
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/internal_server_error.py
--rw-r--r--   0        0        0    12623 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_affiliation200_ok.py
--rw-r--r--   0        0        0    12241 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_assets_locations200_ok.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_assets_locations_position.py
--rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_assets_names200_ok.py
--rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_contacts_error520.py
--rw-r--r--   0        0        0    11578 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_fittings_created.py
--rw-r--r--   0        0        0    13010 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_fittings_fitting.py
--rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_fittings_item.py
--rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_error520.py
--rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_labels_label.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_mail.py
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_recipient.py
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_locations200_ok.py
--rw-r--r--   0        0        0    11511 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_locations_not_found.py
--rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_locations_position.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_names200_ok.py
--rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_names_not_found.py
--rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_members_invitation.py
--rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_members_not_found.py
--rw-r--r--   0        0        0    11476 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_members_unprocessable_entity.py
--rw-r--r--   0        0        0    11550 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_created.py
--rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_not_found.py
--rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_created.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_not_found.py
--rw-r--r--   0        0        0    13228 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_ui_openwindow_newmail_new_mail.py
--rw-r--r--   0        0        0    11503 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_ui_openwindow_newmail_unprocessable_entity.py
--rw-r--r--   0        0        0    11590 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_agent.py
--rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_alliance.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_character.py
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_constellation.py
--rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_corporation.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_faction.py
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_inventory_type.py
--rw-r--r--   0        0        0    16543 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_ok.py
--rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_region.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_station.py
--rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_ids_system.py
--rw-r--r--   0        0        0    12290 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_names200_ok.py
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/post_universe_names_not_found.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_characters_character_id_calendar_event_id_response.py
--rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_characters_character_id_mail_mail_id_contents.py
--rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_members_member_id_movement.py
--rw-r--r--   0        0        0    11472 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_members_member_id_not_found.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_members_member_id_unprocessable_entity.py
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_new_settings.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_not_found.py
--rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_squads_squad_id_naming.py
--rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_squads_squad_id_not_found.py
--rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_wings_wing_id_naming.py
--rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_wings_wing_id_not_found.py
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/service_unavailable.py
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/model/unauthorized.py
--rw-r--r--   0        0        0    37958 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_alliance_api.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_assets_api.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_bad_request.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_bookmarks_api.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_calendar_api.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_character_api.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_clones_api.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_contacts_api.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_contracts_api.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_corporation_api.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_delete_fleets_fleet_id_members_member_id_not_found.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_delete_fleets_fleet_id_squads_squad_id_not_found.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_delete_fleets_fleet_id_wings_wing_id_not_found.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_dogma_api.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_error_limited.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_faction_warfare_api.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_fittings_api.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_fleets_api.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_forbidden.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_gateway_timeout.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_contacts200_ok.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_contacts_labels200_ok.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_icons_not_found.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_icons_ok.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_not_found.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_ok.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_agents_research200_ok.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_assets200_ok.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_assets_not_found.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_attributes_ok.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_blueprints200_ok.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks200_ok.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks_coordinates.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks_folders200_ok.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks_item.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar200_ok.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees200_ok.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees_not_found.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_not_found.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_ok.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_clones_home_location.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_clones_jump_clone.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_clones_ok.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contacts200_ok.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contacts_labels200_ok.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts200_ok.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids200_ok.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids_not_found.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_items200_ok.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_items_not_found.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_corporationhistory200_ok.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fatigue_ok.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fittings200_ok.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fittings_item.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fleet_not_found.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fleet_ok.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fw_stats_kills.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fw_stats_ok.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fw_stats_victory_points.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_industry_jobs200_ok.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_killmails_recent200_ok.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_location_ok.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_loyalty_points200_ok.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail200_ok.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_labels_label.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_labels_ok.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_lists200_ok.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_mail_id_not_found.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_mail_id_ok.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_mail_id_recipient.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_recipient.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_medals200_ok.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_medals_graphic.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mining200_ok.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_not_found.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_notifications200_ok.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_notifications_contacts200_ok.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_ok.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_online_ok.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_opportunities200_ok.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_orders200_ok.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_orders_history200_ok.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets200_ok.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_content.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_extractor_details.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_factory_details.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_head.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_link.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_not_found.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_ok.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_pin.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_route.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_portrait_not_found.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_portrait_ok.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_roles_ok.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_search_ok.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_ship_ok.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_skillqueue200_ok.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_skills_ok.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_skills_skill.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_standings200_ok.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_titles200_ok.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_wallet_journal200_ok.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_wallet_transactions200_ok.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_bids_contract_id200_ok.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_bids_contract_id_forbidden.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_bids_contract_id_not_found.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_items_contract_id200_ok.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_items_contract_id_forbidden.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_items_contract_id_not_found.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_region_id200_ok.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_region_id_not_found.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporation_corporation_id_mining_extractions200_ok.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporation_corporation_id_mining_observers200_ok.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporation_corporation_id_mining_observers_observer_id200_ok.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_alliancehistory200_ok.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_assets200_ok.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_blueprints200_ok.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks200_ok.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks_coordinates.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks_folders200_ok.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks_item.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contacts200_ok.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contacts_labels200_ok.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_containers_logs200_ok.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts200_ok.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids200_ok.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids_not_found.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items200_ok.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_error520.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_not_found.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_customs_offices200_ok.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_divisions_hangar_hangar.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_divisions_ok.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_divisions_wallet_wallet.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_facilities200_ok.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_fw_stats_kills.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_fw_stats_ok.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_fw_stats_victory_points.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_icons_not_found.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_icons_ok.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_industry_jobs200_ok.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_killmails_recent200_ok.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_medals200_ok.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_medals_issued200_ok.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_members_titles200_ok.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_membertracking200_ok.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_not_found.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_ok.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_orders200_ok.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_orders_history200_ok.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_roles200_ok.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_roles_history200_ok.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_shareholders200_ok.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_standings200_ok.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_starbases200_ok.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_fuel.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_ok.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_structures200_ok.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_structures_service.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_titles200_ok.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_wallets200_ok.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_wallets_division_journal200_ok.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_wallets_division_transactions200_ok.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_attributes_attribute_id_not_found.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_attributes_attribute_id_ok.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_effect.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_not_found.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_ok.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_effects_effect_id_modifier.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_effects_effect_id_not_found.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_dogma_effects_effect_id_ok.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_members200_ok.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_members_not_found.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_not_found.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_ok.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_wings200_ok.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_wings_not_found.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_wings_squad.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_active_total_active_total.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_active_total_active_total1.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total1.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_kills.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week1.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_ok.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_victory_points.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday1.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total1.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_kills.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week1.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_ok.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_victory_points.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday1.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_kills.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_last_week_last_week.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_last_week_last_week1.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_ok.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_victory_points.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday1.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_stats200_ok.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_stats_kills.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_stats_victory_points.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_systems200_ok.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_fw_wars200_ok.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_incursions200_ok.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_industry_facilities200_ok.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_industry_systems200_ok.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_industry_systems_cost_indice.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_insurance_prices200_ok.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_insurance_prices_level.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_attacker.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_item.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_items_item.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_ok.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_position.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_unprocessable_entity.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_victim.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_loyalty_stores_corporation_id_offers200_ok.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_loyalty_stores_corporation_id_offers_not_found.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_loyalty_stores_corporation_id_offers_required_item.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_groups_market_group_id_not_found.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_groups_market_group_id_ok.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_prices200_ok.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history200_ok.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history_error520.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history_not_found.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history_unprocessable_entity.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_orders200_ok.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_orders_not_found.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_orders_unprocessable_entity.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_markets_structures_structure_id200_ok.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_opportunities_groups_group_id_ok.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_opportunities_tasks_task_id_ok.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_route_origin_destination_not_found.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_campaigns200_ok.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_campaigns_participant.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_map200_ok.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_structures200_ok.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_status_ok.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_ancestries200_ok.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_not_found.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_ok.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_position.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_bloodlines200_ok.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_categories_category_id_not_found.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_categories_category_id_ok.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_constellations_constellation_id_not_found.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_constellations_constellation_id_ok.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_constellations_constellation_id_position.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_factions200_ok.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_graphics_graphic_id_not_found.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_graphics_graphic_id_ok.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_groups_group_id_not_found.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_groups_group_id_ok.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_moons_moon_id_not_found.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_moons_moon_id_ok.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_moons_moon_id_position.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_planets_planet_id_not_found.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_planets_planet_id_ok.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_planets_planet_id_position.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_races200_ok.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_regions_region_id_not_found.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_regions_region_id_ok.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_schematics_schematic_id_not_found.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_schematics_schematic_id_ok.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_destination.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_not_found.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_ok.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_position.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stars_star_id_ok.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stations_station_id_not_found.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stations_station_id_ok.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_stations_station_id_position.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_structures_structure_id_not_found.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_structures_structure_id_ok.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_structures_structure_id_position.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_system_jumps200_ok.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_system_kills200_ok.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_not_found.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_ok.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_planet.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_position.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_dogma_attribute.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_dogma_effect.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_not_found.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_ok.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_aggressor.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_ally.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_defender.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_killmails200_ok.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_killmails_unprocessable_entity.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_ok.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_unprocessable_entity.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_incursions_api.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_industry_api.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_insurance_api.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_internal_server_error.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_killmails_api.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_location_api.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_loyalty_api.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_mail_api.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_market_api.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_opportunities_api.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_planetary_interaction_api.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_affiliation200_ok.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_assets_locations200_ok.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_assets_locations_position.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_assets_names200_ok.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_contacts_error520.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_fittings_created.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_fittings_fitting.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_fittings_item.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_error520.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_labels_label.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_mail.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_recipient.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_locations200_ok.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_locations_not_found.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_locations_position.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_names200_ok.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_names_not_found.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_members_invitation.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_members_not_found.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_members_unprocessable_entity.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_created.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_not_found.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_created.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_not_found.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_ui_openwindow_newmail_new_mail.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_ui_openwindow_newmail_unprocessable_entity.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_agent.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_alliance.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_character.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_constellation.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_corporation.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_faction.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_inventory_type.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_ok.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_region.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_station.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_system.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_names200_ok.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_post_universe_names_not_found.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_characters_character_id_calendar_event_id_response.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_characters_character_id_mail_mail_id_contents.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_members_member_id_movement.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_members_member_id_not_found.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_members_member_id_unprocessable_entity.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_new_settings.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_not_found.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_naming.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_not_found.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_naming.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_not_found.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_routes_api.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_search_api.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_service_unavailable.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_skills_api.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_sovereignty_api.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_status_api.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_unauthorized.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_universe_api.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_user_interface_api.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_wallet_api.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/esi_client/test/test_wars_api.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/README.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 esi_client-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/__init__.py
+-rw-r--r--   0        0        0    39119 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api_client.py
+-rw-r--r--   0        0        0    16447 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/configuration.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/exceptions.py
+-rw-r--r--   0        0        0    82553 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model_utils.py
+-rw-r--r--   0        0        0    14230 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/rest.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/__init__.py
+-rw-r--r--   0        0        0    26044 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/alliance_api.py
+-rw-r--r--   0        0        0    44642 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/assets_api.py
+-rw-r--r--   0        0        0    30304 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/bookmarks_api.py
+-rw-r--r--   0        0        0    30943 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/calendar_api.py
+-rw-r--r--   0        0        0    95070 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/character_api.py
+-rw-r--r--   0        0        0    14596 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/clones_api.py
+-rw-r--r--   0        0        0    66232 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/contacts_api.py
+-rw-r--r--   0        0        0    67661 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/contracts_api.py
+-rw-r--r--   0        0        0   156673 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/corporation_api.py
+-rw-r--r--   0        0        0    31563 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/dogma_api.py
+-rw-r--r--   0        0        0    49800 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/faction_warfare_api.py
+-rw-r--r--   0        0        0    21482 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/fittings_api.py
+-rw-r--r--   0        0        0    97465 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/fleets_api.py
+-rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/incursions_api.py
+-rw-r--r--   0        0        0    57957 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/industry_api.py
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/insurance_api.py
+-rw-r--r--   0        0        0    22976 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/killmails_api.py
+-rw-r--r--   0        0        0    21634 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/location_api.py
+-rw-r--r--   0        0        0    14814 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/loyalty_api.py
+-rw-r--r--   0        0        0    63735 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/mail_api.py
+-rw-r--r--   0        0        0    77534 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/market_api.py
+-rw-r--r--   0        0        0    33307 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/opportunities_api.py
+-rw-r--r--   0        0        0    29021 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/planetary_interaction_api.py
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/routes_api.py
+-rw-r--r--   0        0        0    11532 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/search_api.py
+-rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/skills_api.py
+-rw-r--r--   0        0        0    18391 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/sovereignty_api.py
+-rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/status_api.py
+-rw-r--r--   0        0        0   198686 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/universe_api.py
+-rw-r--r--   0        0        0    32604 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/user_interface_api.py
+-rw-r--r--   0        0        0    45436 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/wallet_api.py
+-rw-r--r--   0        0        0    19820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/api/wars_api.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/apis/__init__.py
+-rw-r--r--   0        0        0    16858 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/AllianceApi.md
+-rw-r--r--   0        0        0    31173 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/AssetsApi.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/BadRequest.md
+-rw-r--r--   0        0        0    22756 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/BookmarksApi.md
+-rw-r--r--   0        0        0    22607 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/CalendarApi.md
+-rw-r--r--   0        0        0    69568 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/CharacterApi.md
+-rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/ClonesApi.md
+-rw-r--r--   0        0        0    47082 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/ContactsApi.md
+-rw-r--r--   0        0        0    51239 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/ContractsApi.md
+-rw-r--r--   0        0        0   118362 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/CorporationApi.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/DeleteCharactersCharacterIdMailLabelsLabelIdUnprocessableEntity.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/DeleteFleetsFleetIdMembersMemberIdNotFound.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/DeleteFleetsFleetIdSquadsSquadIdNotFound.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/DeleteFleetsFleetIdWingsWingIdNotFound.md
+-rw-r--r--   0        0        0    20565 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/DogmaApi.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/ErrorLimited.md
+-rw-r--r--   0        0        0    34440 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/FactionWarfareApi.md
+-rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/FittingsApi.md
+-rw-r--r--   0        0        0    69064 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/FleetsApi.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/Forbidden.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GatewayTimeout.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdContacts200Ok.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdContactsLabels200Ok.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdIconsNotFound.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdIconsOk.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdNotFound.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdOk.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAgentsResearch200Ok.md
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAssets200Ok.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAssetsNotFound.md
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAttributesOk.md
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBlueprints200Ok.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarks200Ok.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarksCoordinates.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarksFolders200Ok.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarksItem.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendar200Ok.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendees200Ok.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendeesNotFound.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdNotFound.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdOk.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdClonesHomeLocation.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdClonesJumpClone.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdClonesOk.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContacts200Ok.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContactsLabels200Ok.md
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContracts200Ok.md
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdBids200Ok.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdBidsNotFound.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdItems200Ok.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdItemsNotFound.md
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCorporationhistory200Ok.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFatigueOk.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFittings200Ok.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFittingsItem.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFleetNotFound.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFleetOk.md
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFwStatsKills.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFwStatsOk.md
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFwStatsVictoryPoints.md
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdIndustryJobs200Ok.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdKillmailsRecent200Ok.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdLocationOk.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdLoyaltyPoints200Ok.md
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMail200Ok.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailLabelsLabel.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailLabelsOk.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailLists200Ok.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailMailIdNotFound.md
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailMailIdOk.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailMailIdRecipient.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailRecipient.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMedals200Ok.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMedalsGraphic.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMining200Ok.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdNotFound.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdNotifications200Ok.md
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdNotificationsContacts200Ok.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOk.md
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOnlineOk.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOpportunities200Ok.md
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOrders200Ok.md
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOrdersHistory200Ok.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanets200Ok.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdContent.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdExtractorDetails.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdFactoryDetails.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdHead.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdLink.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdNotFound.md
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdOk.md
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdPin.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdRoute.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPortraitNotFound.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPortraitOk.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdRolesOk.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSearchOk.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdShipOk.md
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSkillqueue200Ok.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSkillsOk.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSkillsSkill.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdStandings200Ok.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdTitles200Ok.md
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdWalletJournal200Ok.md
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdWalletTransactions200Ok.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicBidsContractId200Ok.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicBidsContractIdForbidden.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicBidsContractIdNotFound.md
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicItemsContractId200Ok.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicItemsContractIdForbidden.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicItemsContractIdNotFound.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicRegionId200Ok.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetContractsPublicRegionIdNotFound.md
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationCorporationIdMiningExtractions200Ok.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationCorporationIdMiningObservers200Ok.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationCorporationIdMiningObserversObserverId200Ok.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdAlliancehistory200Ok.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdAssets200Ok.md
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBlueprints200Ok.md
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarks200Ok.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarksCoordinates.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarksFolders200Ok.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarksItem.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContacts200Ok.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContactsLabels200Ok.md
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContainersLogs200Ok.md
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContracts200Ok.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBids200Ok.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBidsNotFound.md
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItems200Ok.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsError520.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsNotFound.md
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdCustomsOffices200Ok.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdDivisionsHangarHangar.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdDivisionsOk.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdDivisionsWalletWallet.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFacilities200Ok.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFwStatsKills.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFwStatsOk.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFwStatsVictoryPoints.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdIconsNotFound.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdIconsOk.md
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdIndustryJobs200Ok.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdKillmailsRecent200Ok.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMedals200Ok.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMedalsIssued200Ok.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMembersTitles200Ok.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMembertracking200Ok.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdNotFound.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdOk.md
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdOrders200Ok.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdOrdersHistory200Ok.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdRoles200Ok.md
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdRolesHistory200Ok.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdShareholders200Ok.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStandings200Ok.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStarbases200Ok.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdFuel.md
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdOk.md
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStructures200Ok.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStructuresService.md
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdTitles200Ok.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdWallets200Ok.md
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionJournal200Ok.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionTransactions200Ok.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaAttributesAttributeIdNotFound.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaAttributesAttributeIdOk.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaAttribute.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaEffect.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdNotFound.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdOk.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaEffectsEffectIdModifier.md
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaEffectsEffectIdNotFound.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetDogmaEffectsEffectIdOk.md
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdMembers200Ok.md
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdMembersNotFound.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdNotFound.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdOk.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdWings200Ok.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdWingsNotFound.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdWingsSquad.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal1.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal1.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersKills.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek1.md
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersOk.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersVictoryPoints.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday1.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal1.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsKills.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek1.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsOk.md
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsVictoryPoints.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday1.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsKills.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek1.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsOk.md
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsVictoryPoints.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsYesterdayYesterday.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsYesterdayYesterday1.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwStats200Ok.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwStatsKills.md
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwStatsVictoryPoints.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwSystems200Ok.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetFwWars200Ok.md
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetIncursions200Ok.md
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetIndustryFacilities200Ok.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetIndustrySystems200Ok.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetIndustrySystemsCostIndice.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetInsurancePrices200Ok.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetInsurancePricesLevel.md
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashAttacker.md
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashItem.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashItemsItem.md
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashOk.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashPosition.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashUnprocessableEntity.md
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashVictim.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetLoyaltyStoresCorporationIdOffers200Ok.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetLoyaltyStoresCorporationIdOffersNotFound.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetLoyaltyStoresCorporationIdOffersRequiredItem.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsGroupsMarketGroupIdNotFound.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsGroupsMarketGroupIdOk.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsPrices200Ok.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistory200Ok.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistoryError520.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistoryNotFound.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistoryUnprocessableEntity.md
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdOrders200Ok.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdOrdersNotFound.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdOrdersUnprocessableEntity.md
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetMarketsStructuresStructureId200Ok.md
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetOpportunitiesGroupsGroupIdOk.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetOpportunitiesTasksTaskIdOk.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetRouteOriginDestinationNotFound.md
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetSovereigntyCampaigns200Ok.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetSovereigntyCampaignsParticipant.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetSovereigntyMap200Ok.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetSovereigntyStructures200Ok.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetStatusOk.md
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseAncestries200Ok.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdNotFound.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdOk.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdPosition.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseBloodlines200Ok.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseCategoriesCategoryIdNotFound.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseCategoriesCategoryIdOk.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseConstellationsConstellationIdNotFound.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseConstellationsConstellationIdOk.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseConstellationsConstellationIdPosition.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseFactions200Ok.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseGraphicsGraphicIdNotFound.md
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseGraphicsGraphicIdOk.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseGroupsGroupIdNotFound.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseGroupsGroupIdOk.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseMoonsMoonIdNotFound.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseMoonsMoonIdOk.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseMoonsMoonIdPosition.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniversePlanetsPlanetIdNotFound.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniversePlanetsPlanetIdOk.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniversePlanetsPlanetIdPosition.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseRaces200Ok.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseRegionsRegionIdNotFound.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseRegionsRegionIdOk.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSchematicsSchematicIdNotFound.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSchematicsSchematicIdOk.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdDestination.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdNotFound.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdOk.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdPosition.md
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStarsStarIdOk.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStationsStationIdNotFound.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStationsStationIdOk.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStationsStationIdPosition.md
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStructuresStructureIdNotFound.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStructuresStructureIdOk.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseStructuresStructureIdPosition.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemJumps200Ok.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemKills200Ok.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdNotFound.md
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdOk.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdPlanet.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdPosition.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdDogmaAttribute.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdDogmaEffect.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdNotFound.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdOk.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdAggressor.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdAlly.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdDefender.md
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdKillmails200Ok.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdKillmailsUnprocessableEntity.md
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdOk.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdUnprocessableEntity.md
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/IncursionsApi.md
+-rw-r--r--   0        0        0    43038 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/IndustryApi.md
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/InsuranceApi.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/InternalServerError.md
+-rw-r--r--   0        0        0    16768 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/KillmailsApi.md
+-rw-r--r--   0        0        0    16093 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/LocationApi.md
+-rw-r--r--   0        0        0    10242 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/LoyaltyApi.md
+-rw-r--r--   0        0        0    45241 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/MailApi.md
+-rw-r--r--   0        0        0    55150 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/MarketApi.md
+-rw-r--r--   0        0        0    22205 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/OpportunitiesApi.md
+-rw-r--r--   0        0        0    21129 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PlanetaryInteractionApi.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersAffiliation200Ok.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdAssetsLocations200Ok.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdAssetsLocationsPosition.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdAssetsNames200Ok.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdContactsError520.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdFittingsCreated.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdFittingsFitting.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdFittingsItem.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailError520.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailLabelsLabel.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailMail.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailRecipient.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsLocations200Ok.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsNotFound.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsPosition.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsNames200Ok.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsNamesNotFound.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdMembersInvitation.md
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdMembersNotFound.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdMembersUnprocessableEntity.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsCreated.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsNotFound.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsCreated.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsNotFound.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUiOpenwindowNewmailNewMail.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUiOpenwindowNewmailUnprocessableEntity.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsAgent.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsAlliance.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsCharacter.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsConstellation.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsCorporation.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsFaction.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsInventoryType.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsOk.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsRegion.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsStation.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsSystem.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseNames200Ok.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PostUniverseNamesNotFound.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutCharactersCharacterIdCalendarEventIdResponse.md
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutCharactersCharacterIdMailMailIdContents.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdMembersMemberIdMovement.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdMembersMemberIdNotFound.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdMembersMemberIdUnprocessableEntity.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdNewSettings.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdNotFound.md
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNaming.md
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNotFound.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdWingsWingIdNaming.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdWingsWingIdNotFound.md
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/RoutesApi.md
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/SearchApi.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/ServiceUnavailable.md
+-rw-r--r--   0        0        0    15883 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/SkillsApi.md
+-rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/SovereigntyApi.md
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/StatusApi.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/Unauthorized.md
+-rw-r--r--   0        0        0   128481 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/UniverseApi.md
+-rw-r--r--   0        0        0    21635 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/UserInterfaceApi.md
+-rw-r--r--   0        0        0    34300 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/WalletApi.md
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/docs/WarsApi.md
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/__init__.py
+-rw-r--r--   0        0        0    11435 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/bad_request.py
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/delete_fleets_fleet_id_members_member_id_not_found.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/delete_fleets_fleet_id_squads_squad_id_not_found.py
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/delete_fleets_fleet_id_wings_wing_id_not_found.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/error_limited.py
+-rw-r--r--   0        0        0    11698 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/forbidden.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/gateway_timeout.py
+-rw-r--r--   0        0        0    12668 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_contacts200_ok.py
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_contacts_labels200_ok.py
+-rw-r--r--   0        0        0    11452 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_icons_not_found.py
+-rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_icons_ok.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_not_found.py
+-rw-r--r--   0        0        0    13714 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_ok.py
+-rw-r--r--   0        0        0    12927 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_agents_research200_ok.py
+-rw-r--r--   0        0        0    17483 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_assets200_ok.py
+-rw-r--r--   0        0        0    11461 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_assets_not_found.py
+-rw-r--r--   0        0        0    13829 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_attributes_ok.py
+-rw-r--r--   0        0        0    18552 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_blueprints200_ok.py
+-rw-r--r--   0        0        0    14275 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks200_ok.py
+-rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks_coordinates.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks_folders200_ok.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks_item.py
+-rw-r--r--   0        0        0    12671 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar200_ok.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_attendees200_ok.py
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_attendees_not_found.py
+-rw-r--r--   0        0        0    11496 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_not_found.py
+-rw-r--r--   0        0        0    14135 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_ok.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_clones_home_location.py
+-rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_clones_jump_clone.py
+-rw-r--r--   0        0        0    13287 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_clones_ok.py
+-rw-r--r--   0        0        0    13378 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contacts200_ok.py
+-rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contacts_labels200_ok.py
+-rw-r--r--   0        0        0    19129 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts200_ok.py
+-rw-r--r--   0        0        0    12454 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_bids200_ok.py
+-rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_bids_not_found.py
+-rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_items200_ok.py
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_items_not_found.py
+-rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_corporationhistory200_ok.py
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fatigue_ok.py
+-rw-r--r--   0        0        0    13070 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fittings200_ok.py
+-rw-r--r--   0        0        0    13665 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fittings_item.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fleet_not_found.py
+-rw-r--r--   0        0        0    12760 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fleet_ok.py
+-rw-r--r--   0        0        0    12465 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fw_stats_kills.py
+-rw-r--r--   0        0        0    14311 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fw_stats_ok.py
+-rw-r--r--   0        0        0    12341 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fw_stats_victory_points.py
+-rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_industry_jobs200_ok.py
+-rw-r--r--   0        0        0    11940 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_killmails_recent200_ok.py
+-rw-r--r--   0        0        0    12135 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_location_ok.py
+-rw-r--r--   0        0        0    11982 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_loyalty_points200_ok.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail200_ok.py
+-rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_labels_label.py
+-rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_labels_ok.py
+-rw-r--r--   0        0        0    11835 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_lists200_ok.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_mail_id_not_found.py
+-rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_mail_id_ok.py
+-rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_mail_id_recipient.py
+-rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_recipient.py
+-rw-r--r--   0        0        0    14242 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_medals200_ok.py
+-rw-r--r--   0        0        0    12186 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_medals_graphic.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mining200_ok.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_not_found.py
+-rw-r--r--   0        0        0    26376 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_notifications200_ok.py
+-rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_notifications_contacts200_ok.py
+-rw-r--r--   0        0        0    14640 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_ok.py
+-rw-r--r--   0        0        0    12388 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_online_ok.py
+-rw-r--r--   0        0        0    11878 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_opportunities200_ok.py
+-rw-r--r--   0        0        0    16413 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_orders200_ok.py
+-rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_orders_history200_ok.py
+-rw-r--r--   0        0        0    13876 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets200_ok.py
+-rw-r--r--   0        0        0    11799 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_content.py
+-rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_extractor_details.py
+-rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_factory_details.py
+-rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_head.py
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_link.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_not_found.py
+-rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_ok.py
+-rw-r--r--   0        0        0    15535 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_pin.py
+-rw-r--r--   0        0        0    13252 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_route.py
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_portrait_not_found.py
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_portrait_ok.py
+-rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_roles_ok.py
+-rw-r--r--   0        0        0    14656 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_search_ok.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_ship_ok.py
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_skillqueue200_ok.py
+-rw-r--r--   0        0        0    12504 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_skills_ok.py
+-rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_skills_skill.py
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_standings200_ok.py
+-rw-r--r--   0        0        0    11677 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_titles200_ok.py
+-rw-r--r--   0        0        0    25772 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_wallet_journal200_ok.py
+-rw-r--r--   0        0        0    14228 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_characters_character_id_wallet_transactions200_ok.py
+-rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_bids_contract_id200_ok.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_bids_contract_id_forbidden.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_bids_contract_id_not_found.py
+-rw-r--r--   0        0        0    14728 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_items_contract_id200_ok.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_items_contract_id_forbidden.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_items_contract_id_not_found.py
+-rw-r--r--   0        0        0    16429 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_region_id200_ok.py
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_contracts_public_region_id_not_found.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporation_corporation_id_mining_extractions200_ok.py
+-rw-r--r--   0        0        0    12715 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporation_corporation_id_mining_observers200_ok.py
+-rw-r--r--   0        0        0    13062 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporation_corporation_id_mining_observers_observer_id200_ok.py
+-rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_alliancehistory200_ok.py
+-rw-r--r--   0        0        0    19003 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_assets200_ok.py
+-rw-r--r--   0        0        0    19930 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_blueprints200_ok.py
+-rw-r--r--   0        0        0    14343 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks200_ok.py
+-rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks_coordinates.py
+-rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks_folders200_ok.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks_item.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contacts200_ok.py
+-rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contacts_labels200_ok.py
+-rw-r--r--   0        0        0    20654 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_containers_logs200_ok.py
+-rw-r--r--   0        0        0    19121 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts200_ok.py
+-rw-r--r--   0        0        0    12466 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids200_ok.py
+-rw-r--r--   0        0        0    11532 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids_not_found.py
+-rw-r--r--   0        0        0    13534 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items200_ok.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_error520.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_not_found.py
+-rw-r--r--   0        0        0    17531 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_customs_offices200_ok.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_divisions_hangar_hangar.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_divisions_ok.py
+-rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_divisions_wallet_wallet.py
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_facilities200_ok.py
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_fw_stats_kills.py
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_fw_stats_ok.py
+-rw-r--r--   0        0        0    12409 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_fw_stats_victory_points.py
+-rw-r--r--   0        0        0    11470 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_icons_not_found.py
+-rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_icons_ok.py
+-rw-r--r--   0        0        0    19518 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_industry_jobs200_ok.py
+-rw-r--r--   0        0        0    11952 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_killmails_recent200_ok.py
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_medals200_ok.py
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_medals_issued200_ok.py
+-rw-r--r--   0        0        0    11941 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_members_titles200_ok.py
+-rw-r--r--   0        0        0    13159 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_membertracking200_ok.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_not_found.py
+-rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_ok.py
+-rw-r--r--   0        0        0    16819 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_orders200_ok.py
+-rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_orders_history200_ok.py
+-rw-r--r--   0        0        0    33972 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_roles200_ok.py
+-rw-r--r--   0        0        0    18571 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_roles_history200_ok.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_shareholders200_ok.py
+-rw-r--r--   0        0        0    12233 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_standings200_ok.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_starbases200_ok.py
+-rw-r--r--   0        0        0    11840 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_fuel.py
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_ok.py
+-rw-r--r--   0        0        0    18352 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_structures200_ok.py
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_structures_service.py
+-rw-r--r--   0        0        0    34063 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_titles200_ok.py
+-rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_wallets200_ok.py
+-rw-r--r--   0        0        0    26391 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_wallets_division_journal200_ok.py
+-rw-r--r--   0        0        0    14017 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_wallets_division_transactions200_ok.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_attributes_attribute_id_not_found.py
+-rw-r--r--   0        0        0    13774 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_attributes_attribute_id_ok.py
+-rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py
+-rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_effect.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_not_found.py
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_ok.py
+-rw-r--r--   0        0        0    12821 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_effects_effect_id_modifier.py
+-rw-r--r--   0        0        0    11448 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_effects_effect_id_not_found.py
+-rw-r--r--   0        0        0    17527 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_dogma_effects_effect_id_ok.py
+-rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_members200_ok.py
+-rw-r--r--   0        0        0    11448 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_members_not_found.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_not_found.py
+-rw-r--r--   0        0        0    12556 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_ok.py
+-rw-r--r--   0        0        0    12251 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_wings200_ok.py
+-rw-r--r--   0        0        0    11442 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_wings_not_found.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_wings_squad.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_active_total_active_total.py
+-rw-r--r--   0        0        0    11742 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_active_total_active_total1.py
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_active_total_active_total.py
+-rw-r--r--   0        0        0    11786 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_active_total_active_total1.py
+-rw-r--r--   0        0        0    13971 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_kills.py
+-rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_last_week_last_week.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_last_week_last_week1.py
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_ok.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_victory_points.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday.py
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday1.py
+-rw-r--r--   0        0        0    11785 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total1.py
+-rw-r--r--   0        0        0    14058 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_kills.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week.py
+-rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week1.py
+-rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_ok.py
+-rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_victory_points.py
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday.py
+-rw-r--r--   0        0        0    11794 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday1.py
+-rw-r--r--   0        0        0    13726 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_kills.py
+-rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_last_week_last_week.py
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_last_week_last_week1.py
+-rw-r--r--   0        0        0    12251 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_ok.py
+-rw-r--r--   0        0        0    13825 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_victory_points.py
+-rw-r--r--   0        0        0    11709 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_yesterday_yesterday.py
+-rw-r--r--   0        0        0    11730 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_yesterday_yesterday1.py
+-rw-r--r--   0        0        0    13199 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_stats200_ok.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_stats_kills.py
+-rw-r--r--   0        0        0    12172 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_stats_victory_points.py
+-rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_systems200_ok.py
+-rw-r--r--   0        0        0    11830 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_fw_wars200_ok.py
+-rw-r--r--   0        0        0    14393 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_incursions200_ok.py
+-rw-r--r--   0        0        0    13029 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_industry_facilities200_ok.py
+-rw-r--r--   0        0        0    12294 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_industry_systems200_ok.py
+-rw-r--r--   0        0        0    12350 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_industry_systems_cost_indice.py
+-rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_insurance_prices200_ok.py
+-rw-r--r--   0        0        0    11941 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_insurance_prices_level.py
+-rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_attacker.py
+-rw-r--r--   0        0        0    13500 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_item.py
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_items_item.py
+-rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_ok.py
+-rw-r--r--   0        0        0    11833 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_position.py
+-rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_unprocessable_entity.py
+-rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_victim.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_loyalty_stores_corporation_id_offers200_ok.py
+-rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_loyalty_stores_corporation_id_offers_not_found.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_loyalty_stores_corporation_id_offers_required_item.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_groups_market_group_id_not_found.py
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_groups_market_group_id_ok.py
+-rw-r--r--   0        0        0    12035 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_prices200_ok.py
+-rw-r--r--   0        0        0    12872 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history200_ok.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history_error520.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history_not_found.py
+-rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history_unprocessable_entity.py
+-rw-r--r--   0        0        0    15004 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_region_id_orders200_ok.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_region_id_orders_not_found.py
+-rw-r--r--   0        0        0    11506 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_region_id_orders_unprocessable_entity.py
+-rw-r--r--   0        0        0    14702 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_markets_structures_structure_id200_ok.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_opportunities_groups_group_id_ok.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_opportunities_tasks_task_id_ok.py
+-rw-r--r--   0        0        0    11454 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_route_origin_destination_not_found.py
+-rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_sovereignty_campaigns200_ok.py
+-rw-r--r--   0        0        0    11806 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_sovereignty_campaigns_participant.py
+-rw-r--r--   0        0        0    12290 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_sovereignty_map200_ok.py
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_sovereignty_structures200_ok.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_status_ok.py
+-rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_ancestries200_ok.py
+-rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_not_found.py
+-rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_ok.py
+-rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_position.py
+-rw-r--r--   0        0        0    14440 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_bloodlines200_ok.py
+-rw-r--r--   0        0        0    11472 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_categories_category_id_not_found.py
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_categories_category_id_ok.py
+-rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_constellations_constellation_id_not_found.py
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_constellations_constellation_id_ok.py
+-rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_constellations_constellation_id_position.py
+-rw-r--r--   0        0        0    14292 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_factions200_ok.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_graphics_graphic_id_not_found.py
+-rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_graphics_graphic_id_ok.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_groups_group_id_not_found.py
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_groups_group_id_ok.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_moons_moon_id_not_found.py
+-rw-r--r--   0        0        0    12576 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_moons_moon_id_ok.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_moons_moon_id_position.py
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_planets_planet_id_not_found.py
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_planets_planet_id_ok.py
+-rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_planets_planet_id_position.py
+-rw-r--r--   0        0        0    12366 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_races200_ok.py
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_regions_region_id_not_found.py
+-rw-r--r--   0        0        0    12417 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_regions_region_id_ok.py
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_schematics_schematic_id_not_found.py
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_schematics_schematic_id_ok.py
+-rw-r--r--   0        0        0    11963 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_destination.py
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_not_found.py
+-rw-r--r--   0        0        0    13577 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_ok.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_position.py
+-rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stars_star_id_ok.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stations_station_id_not_found.py
+-rw-r--r--   0        0        0    16824 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stations_station_id_ok.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_stations_station_id_position.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_structures_structure_id_not_found.py
+-rw-r--r--   0        0        0    13054 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_structures_structure_id_ok.py
+-rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_structures_structure_id_position.py
+-rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_system_jumps200_ok.py
+-rw-r--r--   0        0        0    12520 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_system_kills200_ok.py
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_not_found.py
+-rw-r--r--   0        0        0    14782 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_ok.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_planet.py
+-rw-r--r--   0        0        0    11809 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_position.py
+-rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_dogma_attribute.py
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_dogma_effect.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_not_found.py
+-rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_ok.py
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_wars_war_id_aggressor.py
+-rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_wars_war_id_ally.py
+-rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_wars_war_id_defender.py
+-rw-r--r--   0        0        0    11886 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_wars_war_id_killmails200_ok.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_wars_war_id_killmails_unprocessable_entity.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_wars_war_id_ok.py
+-rw-r--r--   0        0        0    11470 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/get_wars_war_id_unprocessable_entity.py
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/internal_server_error.py
+-rw-r--r--   0        0        0    12623 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_affiliation200_ok.py
+-rw-r--r--   0        0        0    12241 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_assets_locations200_ok.py
+-rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_assets_locations_position.py
+-rw-r--r--   0        0        0    11756 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_assets_names200_ok.py
+-rw-r--r--   0        0        0    11478 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_contacts_error520.py
+-rw-r--r--   0        0        0    11578 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_fittings_created.py
+-rw-r--r--   0        0        0    13010 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_fittings_fitting.py
+-rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_fittings_item.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_error520.py
+-rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_labels_label.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_mail.py
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_recipient.py
+-rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_locations200_ok.py
+-rw-r--r--   0        0        0    11511 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_locations_not_found.py
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_locations_position.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_names200_ok.py
+-rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_names_not_found.py
+-rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_members_invitation.py
+-rw-r--r--   0        0        0    11451 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_members_not_found.py
+-rw-r--r--   0        0        0    11476 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_members_unprocessable_entity.py
+-rw-r--r--   0        0        0    11550 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_created.py
+-rw-r--r--   0        0        0    11445 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_not_found.py
+-rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_created.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_not_found.py
+-rw-r--r--   0        0        0    13228 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_ui_openwindow_newmail_new_mail.py
+-rw-r--r--   0        0        0    11503 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_ui_openwindow_newmail_unprocessable_entity.py
+-rw-r--r--   0        0        0    11590 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_agent.py
+-rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_alliance.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_character.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_constellation.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_corporation.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_faction.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_inventory_type.py
+-rw-r--r--   0        0        0    16543 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_ok.py
+-rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_region.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_station.py
+-rw-r--r--   0        0        0    11593 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_ids_system.py
+-rw-r--r--   0        0        0    12290 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_names200_ok.py
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/post_universe_names_not_found.py
+-rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_characters_character_id_calendar_event_id_response.py
+-rw-r--r--   0        0        0    11906 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_characters_character_id_mail_mail_id_contents.py
+-rw-r--r--   0        0        0    13113 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_members_member_id_movement.py
+-rw-r--r--   0        0        0    11472 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_members_member_id_not_found.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_members_member_id_unprocessable_entity.py
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_new_settings.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_not_found.py
+-rw-r--r--   0        0        0    11545 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_squads_squad_id_naming.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_squads_squad_id_not_found.py
+-rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_wings_wing_id_naming.py
+-rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_wings_wing_id_not_found.py
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/service_unavailable.py
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/model/unauthorized.py
+-rw-r--r--   0        0        0    37958 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_alliance_api.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_assets_api.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_bad_request.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_bookmarks_api.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_calendar_api.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_character_api.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_clones_api.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_contacts_api.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_contracts_api.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_corporation_api.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_delete_fleets_fleet_id_members_member_id_not_found.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_delete_fleets_fleet_id_squads_squad_id_not_found.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_delete_fleets_fleet_id_wings_wing_id_not_found.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_dogma_api.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_error_limited.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_faction_warfare_api.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_fittings_api.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_fleets_api.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_forbidden.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_gateway_timeout.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_contacts200_ok.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_contacts_labels200_ok.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_icons_not_found.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_icons_ok.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_not_found.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_ok.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_agents_research200_ok.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_assets200_ok.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_assets_not_found.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_attributes_ok.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_blueprints200_ok.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks200_ok.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks_coordinates.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks_folders200_ok.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks_item.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar200_ok.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees200_ok.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees_not_found.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_not_found.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_ok.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_clones_home_location.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_clones_jump_clone.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_clones_ok.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contacts200_ok.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contacts_labels200_ok.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts200_ok.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids200_ok.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids_not_found.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_items200_ok.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_items_not_found.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_corporationhistory200_ok.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fatigue_ok.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fittings200_ok.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fittings_item.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fleet_not_found.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fleet_ok.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fw_stats_kills.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fw_stats_ok.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fw_stats_victory_points.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_industry_jobs200_ok.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_killmails_recent200_ok.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_location_ok.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_loyalty_points200_ok.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail200_ok.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_labels_label.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_labels_ok.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_lists200_ok.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_mail_id_not_found.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_mail_id_ok.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_mail_id_recipient.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_recipient.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_medals200_ok.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_medals_graphic.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mining200_ok.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_not_found.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_notifications200_ok.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_notifications_contacts200_ok.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_ok.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_online_ok.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_opportunities200_ok.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_orders200_ok.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_orders_history200_ok.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets200_ok.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_content.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_extractor_details.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_factory_details.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_head.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_link.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_not_found.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_ok.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_pin.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_route.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_portrait_not_found.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_portrait_ok.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_roles_ok.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_search_ok.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_ship_ok.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_skillqueue200_ok.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_skills_ok.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_skills_skill.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_standings200_ok.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_titles200_ok.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_wallet_journal200_ok.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_wallet_transactions200_ok.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_bids_contract_id200_ok.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_bids_contract_id_forbidden.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_bids_contract_id_not_found.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_items_contract_id200_ok.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_items_contract_id_forbidden.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_items_contract_id_not_found.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_region_id200_ok.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_region_id_not_found.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporation_corporation_id_mining_extractions200_ok.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporation_corporation_id_mining_observers200_ok.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporation_corporation_id_mining_observers_observer_id200_ok.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_alliancehistory200_ok.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_assets200_ok.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_blueprints200_ok.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks200_ok.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks_coordinates.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks_folders200_ok.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks_item.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contacts200_ok.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contacts_labels200_ok.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_containers_logs200_ok.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts200_ok.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids200_ok.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids_not_found.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items200_ok.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_error520.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_not_found.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_customs_offices200_ok.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_divisions_hangar_hangar.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_divisions_ok.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_divisions_wallet_wallet.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_facilities200_ok.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_fw_stats_kills.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_fw_stats_ok.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_fw_stats_victory_points.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_icons_not_found.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_icons_ok.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_industry_jobs200_ok.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_killmails_recent200_ok.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_medals200_ok.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_medals_issued200_ok.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_members_titles200_ok.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_membertracking200_ok.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_not_found.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_ok.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_orders200_ok.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_orders_history200_ok.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_roles200_ok.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_roles_history200_ok.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_shareholders200_ok.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_standings200_ok.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_starbases200_ok.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_fuel.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_ok.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_structures200_ok.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_structures_service.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_titles200_ok.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_wallets200_ok.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_wallets_division_journal200_ok.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_wallets_division_transactions200_ok.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_attributes_attribute_id_not_found.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_attributes_attribute_id_ok.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_effect.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_not_found.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_ok.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_effects_effect_id_modifier.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_effects_effect_id_not_found.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_dogma_effects_effect_id_ok.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_members200_ok.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_members_not_found.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_not_found.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_ok.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_wings200_ok.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_wings_not_found.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_wings_squad.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_active_total_active_total.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_active_total_active_total1.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total1.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_kills.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week1.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_ok.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_victory_points.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday1.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total1.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_kills.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week1.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_ok.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_victory_points.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday1.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_kills.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_last_week_last_week.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_last_week_last_week1.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_ok.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_victory_points.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday1.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_stats200_ok.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_stats_kills.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_stats_victory_points.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_systems200_ok.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_fw_wars200_ok.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_incursions200_ok.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_industry_facilities200_ok.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_industry_systems200_ok.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_industry_systems_cost_indice.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_insurance_prices200_ok.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_insurance_prices_level.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_attacker.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_item.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_items_item.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_ok.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_position.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_unprocessable_entity.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_victim.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_loyalty_stores_corporation_id_offers200_ok.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_loyalty_stores_corporation_id_offers_not_found.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_loyalty_stores_corporation_id_offers_required_item.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_groups_market_group_id_not_found.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_groups_market_group_id_ok.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_prices200_ok.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history200_ok.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history_error520.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history_not_found.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history_unprocessable_entity.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_orders200_ok.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_orders_not_found.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_orders_unprocessable_entity.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_markets_structures_structure_id200_ok.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_opportunities_groups_group_id_ok.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_opportunities_tasks_task_id_ok.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_route_origin_destination_not_found.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_campaigns200_ok.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_campaigns_participant.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_map200_ok.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_structures200_ok.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_status_ok.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_ancestries200_ok.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_not_found.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_ok.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_position.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_bloodlines200_ok.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_categories_category_id_not_found.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_categories_category_id_ok.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_constellations_constellation_id_not_found.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_constellations_constellation_id_ok.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_constellations_constellation_id_position.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_factions200_ok.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_graphics_graphic_id_not_found.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_graphics_graphic_id_ok.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_groups_group_id_not_found.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_groups_group_id_ok.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_moons_moon_id_not_found.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_moons_moon_id_ok.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_moons_moon_id_position.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_planets_planet_id_not_found.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_planets_planet_id_ok.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_planets_planet_id_position.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_races200_ok.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_regions_region_id_not_found.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_regions_region_id_ok.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_schematics_schematic_id_not_found.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_schematics_schematic_id_ok.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_destination.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_not_found.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_ok.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_position.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stars_star_id_ok.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stations_station_id_not_found.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stations_station_id_ok.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_stations_station_id_position.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_structures_structure_id_not_found.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_structures_structure_id_ok.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_structures_structure_id_position.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_system_jumps200_ok.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_system_kills200_ok.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_not_found.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_ok.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_planet.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_position.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_dogma_attribute.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_dogma_effect.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_not_found.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_ok.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_aggressor.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_ally.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_defender.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_killmails200_ok.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_killmails_unprocessable_entity.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_ok.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_unprocessable_entity.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_incursions_api.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_industry_api.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_insurance_api.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_internal_server_error.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_killmails_api.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_location_api.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_loyalty_api.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_mail_api.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_market_api.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_opportunities_api.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_planetary_interaction_api.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_affiliation200_ok.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_assets_locations200_ok.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_assets_locations_position.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_assets_names200_ok.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_contacts_error520.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_fittings_created.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_fittings_fitting.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_fittings_item.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_error520.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_labels_label.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_mail.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_recipient.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_locations200_ok.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_locations_not_found.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_locations_position.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_names200_ok.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_names_not_found.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_members_invitation.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_members_not_found.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_members_unprocessable_entity.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_created.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_not_found.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_created.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_not_found.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_ui_openwindow_newmail_new_mail.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_ui_openwindow_newmail_unprocessable_entity.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_agent.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_alliance.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_character.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_constellation.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_corporation.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_faction.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_inventory_type.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_ok.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_region.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_station.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_system.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_names200_ok.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_post_universe_names_not_found.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_characters_character_id_calendar_event_id_response.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_characters_character_id_mail_mail_id_contents.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_members_member_id_movement.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_members_member_id_not_found.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_members_member_id_unprocessable_entity.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_new_settings.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_not_found.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_naming.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_not_found.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_naming.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_not_found.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_routes_api.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_search_api.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_service_unavailable.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_skills_api.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_sovereignty_api.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_status_api.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_unauthorized.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_universe_api.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_user_interface_api.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_wallet_api.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/esi_client/test/test_wars_api.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/README.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 esi_client-0.1.0a2/PKG-INFO
```

### Comparing `esi_client-0.1.0a1/esi_client/__init__.py` & `esi_client-0.1.0a2/esi_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     An OpenAPI for EVE Online  # noqa: E501
 
     The version of the OpenAPI document: 1.17
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.1.0a1"
+__version__ = "0.1.0a2"
 
 # import ApiClient
 from esi_client.api_client import ApiClient
 
 # import Configuration
 from esi_client.configuration import Configuration
```

### Comparing `esi_client-0.1.0a1/esi_client/api_client.py` & `esi_client-0.1.0a2/esi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.0a1/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.0a2/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `esi_client-0.1.0a1/esi_client/configuration.py` & `esi_client-0.1.0a2/esi_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.17\n"\
-               "SDK Package Version: 0.1.0a1".\
+               "SDK Package Version: 0.1.0a2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `esi_client-0.1.0a1/esi_client/exceptions.py` & `esi_client-0.1.0a2/esi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model_utils.py` & `esi_client-0.1.0a2/esi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/rest.py` & `esi_client-0.1.0a2/esi_client/rest.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/alliance_api.py` & `esi_client-0.1.0a2/esi_client/api/alliance_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/assets_api.py` & `esi_client-0.1.0a2/esi_client/api/assets_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/bookmarks_api.py` & `esi_client-0.1.0a2/esi_client/api/bookmarks_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/calendar_api.py` & `esi_client-0.1.0a2/esi_client/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/character_api.py` & `esi_client-0.1.0a2/esi_client/api/character_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/clones_api.py` & `esi_client-0.1.0a2/esi_client/api/clones_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/contacts_api.py` & `esi_client-0.1.0a2/esi_client/api/contacts_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/contracts_api.py` & `esi_client-0.1.0a2/esi_client/api/contracts_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/corporation_api.py` & `esi_client-0.1.0a2/esi_client/api/corporation_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/dogma_api.py` & `esi_client-0.1.0a2/esi_client/api/dogma_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/faction_warfare_api.py` & `esi_client-0.1.0a2/esi_client/api/faction_warfare_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/fittings_api.py` & `esi_client-0.1.0a2/esi_client/api/fittings_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/fleets_api.py` & `esi_client-0.1.0a2/esi_client/api/fleets_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/incursions_api.py` & `esi_client-0.1.0a2/esi_client/api/incursions_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/industry_api.py` & `esi_client-0.1.0a2/esi_client/api/industry_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/insurance_api.py` & `esi_client-0.1.0a2/esi_client/api/insurance_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/killmails_api.py` & `esi_client-0.1.0a2/esi_client/api/killmails_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/location_api.py` & `esi_client-0.1.0a2/esi_client/api/location_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/loyalty_api.py` & `esi_client-0.1.0a2/esi_client/api/loyalty_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/mail_api.py` & `esi_client-0.1.0a2/esi_client/api/mail_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/market_api.py` & `esi_client-0.1.0a2/esi_client/api/market_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/opportunities_api.py` & `esi_client-0.1.0a2/esi_client/api/opportunities_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/planetary_interaction_api.py` & `esi_client-0.1.0a2/esi_client/api/planetary_interaction_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/routes_api.py` & `esi_client-0.1.0a2/esi_client/api/routes_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/search_api.py` & `esi_client-0.1.0a2/esi_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/skills_api.py` & `esi_client-0.1.0a2/esi_client/api/skills_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/sovereignty_api.py` & `esi_client-0.1.0a2/esi_client/api/sovereignty_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/status_api.py` & `esi_client-0.1.0a2/esi_client/api/status_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/universe_api.py` & `esi_client-0.1.0a2/esi_client/api/universe_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/user_interface_api.py` & `esi_client-0.1.0a2/esi_client/api/user_interface_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/wallet_api.py` & `esi_client-0.1.0a2/esi_client/api/wallet_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/api/wars_api.py` & `esi_client-0.1.0a2/esi_client/api/wars_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/apis/__init__.py` & `esi_client-0.1.0a2/esi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/AllianceApi.md` & `esi_client-0.1.0a2/esi_client/docs/AllianceApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/AssetsApi.md` & `esi_client-0.1.0a2/esi_client/docs/AssetsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/BadRequest.md` & `esi_client-0.1.0a2/esi_client/docs/BadRequest.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/BookmarksApi.md` & `esi_client-0.1.0a2/esi_client/docs/BookmarksApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/CalendarApi.md` & `esi_client-0.1.0a2/esi_client/docs/CalendarApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/CharacterApi.md` & `esi_client-0.1.0a2/esi_client/docs/CharacterApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/ClonesApi.md` & `esi_client-0.1.0a2/esi_client/docs/ClonesApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/ContactsApi.md` & `esi_client-0.1.0a2/esi_client/docs/ContactsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/ContractsApi.md` & `esi_client-0.1.0a2/esi_client/docs/ContractsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/CorporationApi.md` & `esi_client-0.1.0a2/esi_client/docs/CorporationApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/DeleteCharactersCharacterIdMailLabelsLabelIdUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/DeleteCharactersCharacterIdMailLabelsLabelIdUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/DeleteFleetsFleetIdMembersMemberIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/DeleteFleetsFleetIdMembersMemberIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/DeleteFleetsFleetIdSquadsSquadIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/DeleteFleetsFleetIdSquadsSquadIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/DeleteFleetsFleetIdWingsWingIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/DeleteFleetsFleetIdWingsWingIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/DogmaApi.md` & `esi_client-0.1.0a2/esi_client/docs/DogmaApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/ErrorLimited.md` & `esi_client-0.1.0a2/esi_client/docs/ErrorLimited.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/FactionWarfareApi.md` & `esi_client-0.1.0a2/esi_client/docs/FactionWarfareApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/FittingsApi.md` & `esi_client-0.1.0a2/esi_client/docs/FittingsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/FleetsApi.md` & `esi_client-0.1.0a2/esi_client/docs/FleetsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/Forbidden.md` & `esi_client-0.1.0a2/esi_client/docs/Forbidden.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GatewayTimeout.md` & `esi_client-0.1.0a2/esi_client/docs/GatewayTimeout.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdContacts200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdContacts200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdContactsLabels200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdContactsLabels200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdIconsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdIconsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdIconsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdIconsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetAlliancesAllianceIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetAlliancesAllianceIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAgentsResearch200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAgentsResearch200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAssets200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAssets200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAssetsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAssetsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdAttributesOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdAttributesOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBlueprints200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBlueprints200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarks200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarks200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarksCoordinates.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarksCoordinates.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarksFolders200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarksFolders200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdBookmarksItem.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdBookmarksItem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendar200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendar200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendees200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendees200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendeesNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdAttendeesNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCalendarEventIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCalendarEventIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdClonesHomeLocation.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdClonesHomeLocation.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdClonesJumpClone.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdClonesJumpClone.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdClonesOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdClonesOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContacts200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContacts200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContactsLabels200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContactsLabels200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContracts200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContracts200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdBids200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdBids200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdBidsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdBidsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdItems200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdItems200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdContractsContractIdItemsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdContractsContractIdItemsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdCorporationhistory200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdCorporationhistory200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFatigueOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFatigueOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFittings200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFittings200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFittingsItem.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFittingsItem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFleetNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFleetNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFleetOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFleetOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFwStatsKills.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFwStatsKills.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFwStatsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFwStatsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdFwStatsVictoryPoints.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdFwStatsVictoryPoints.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdIndustryJobs200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdIndustryJobs200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdKillmailsRecent200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdKillmailsRecent200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdLocationOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdLocationOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdLoyaltyPoints200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdLoyaltyPoints200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMail200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMail200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailLabelsLabel.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailLabelsLabel.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailLabelsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailLabelsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailLists200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailLists200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailMailIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailMailIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailMailIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailMailIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailMailIdRecipient.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailMailIdRecipient.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMailRecipient.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMailRecipient.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMedals200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMedals200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMedalsGraphic.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMedalsGraphic.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdMining200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdMining200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdNotifications200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdNotifications200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdNotificationsContacts200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdNotificationsContacts200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOnlineOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOnlineOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOpportunities200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOpportunities200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOrders200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOrders200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdOrdersHistory200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdOrdersHistory200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanets200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanets200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdContent.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdContent.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdExtractorDetails.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdExtractorDetails.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdFactoryDetails.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdFactoryDetails.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdHead.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdHead.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdLink.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdLink.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdPin.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdPin.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdRoute.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPlanetsPlanetIdRoute.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPortraitNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPortraitNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdPortraitOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdPortraitOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdRolesOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdRolesOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSearchOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSearchOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdShipOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdShipOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSkillqueue200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSkillqueue200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSkillsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSkillsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdSkillsSkill.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdSkillsSkill.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdStandings200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdStandings200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdTitles200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdTitles200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdWalletJournal200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdWalletJournal200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCharactersCharacterIdWalletTransactions200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCharactersCharacterIdWalletTransactions200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicBidsContractId200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicBidsContractId200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicBidsContractIdForbidden.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicBidsContractIdForbidden.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicBidsContractIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicBidsContractIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicItemsContractId200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicItemsContractId200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicItemsContractIdForbidden.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicItemsContractIdForbidden.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicItemsContractIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicItemsContractIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicRegionId200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicRegionId200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetContractsPublicRegionIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetContractsPublicRegionIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationCorporationIdMiningExtractions200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationCorporationIdMiningExtractions200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationCorporationIdMiningObservers200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationCorporationIdMiningObservers200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationCorporationIdMiningObserversObserverId200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationCorporationIdMiningObserversObserverId200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdAlliancehistory200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdAlliancehistory200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdAssets200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdAssets200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBlueprints200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBlueprints200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarks200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarks200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarksCoordinates.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarksCoordinates.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarksFolders200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarksFolders200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdBookmarksItem.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdBookmarksItem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContacts200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContacts200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContactsLabels200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContactsLabels200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContainersLogs200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContainersLogs200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContracts200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContracts200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBids200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBids200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBidsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdBidsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItems200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItems200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsError520.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsError520.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdContractsContractIdItemsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdCustomsOffices200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdCustomsOffices200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdDivisionsHangarHangar.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdDivisionsHangarHangar.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdDivisionsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdDivisionsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdDivisionsWalletWallet.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdDivisionsWalletWallet.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFacilities200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFacilities200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFwStatsKills.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFwStatsKills.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFwStatsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFwStatsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdFwStatsVictoryPoints.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdFwStatsVictoryPoints.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdIconsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdIconsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdIconsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdIconsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdIndustryJobs200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdIndustryJobs200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdKillmailsRecent200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdKillmailsRecent200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMedals200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMedals200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMedalsIssued200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMedalsIssued200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMembersTitles200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMembersTitles200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdMembertracking200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdMembertracking200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdOrders200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdOrders200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdOrdersHistory200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdOrdersHistory200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdRoles200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdRoles200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdRolesHistory200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdRolesHistory200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdShareholders200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdShareholders200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStandings200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStandings200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStarbases200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStarbases200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdFuel.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdFuel.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStarbasesStarbaseIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStructures200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStructures200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdStructuresService.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdStructuresService.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdTitles200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdTitles200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdWallets200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdWallets200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionJournal200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionJournal200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionTransactions200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetCorporationsCorporationIdWalletsDivisionTransactions200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaAttributesAttributeIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaAttributesAttributeIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaAttributesAttributeIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaAttributesAttributeIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaAttribute.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaAttribute.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaEffect.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdDogmaEffect.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaDynamicItemsTypeIdItemIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaEffectsEffectIdModifier.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaEffectsEffectIdModifier.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaEffectsEffectIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaEffectsEffectIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetDogmaEffectsEffectIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetDogmaEffectsEffectIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdMembers200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdMembers200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdMembersNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdMembersNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdWings200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdWings200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdWingsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdWingsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFleetsFleetIdWingsSquad.md` & `esi_client-0.1.0a2/esi_client/docs/GetFleetsFleetIdWingsSquad.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsActiveTotalActiveTotal1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersActiveTotalActiveTotal1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersKills.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersKills.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersLastWeekLastWeek1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersVictoryPoints.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersVictoryPoints.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCharactersYesterdayYesterday1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsActiveTotalActiveTotal1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsKills.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsKills.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsLastWeekLastWeek1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsVictoryPoints.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsVictoryPoints.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsCorporationsYesterdayYesterday1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsKills.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsKills.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsLastWeekLastWeek1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsVictoryPoints.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsVictoryPoints.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsYesterdayYesterday.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsYesterdayYesterday.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwLeaderboardsYesterdayYesterday1.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwLeaderboardsYesterdayYesterday1.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwStats200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwStats200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwStatsKills.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwStatsKills.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwStatsVictoryPoints.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwStatsVictoryPoints.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwSystems200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwSystems200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetFwWars200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetFwWars200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetIncursions200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetIncursions200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetIndustryFacilities200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetIndustryFacilities200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetIndustrySystems200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetIndustrySystems200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetIndustrySystemsCostIndice.md` & `esi_client-0.1.0a2/esi_client/docs/GetIndustrySystemsCostIndice.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetInsurancePrices200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetInsurancePrices200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetInsurancePricesLevel.md` & `esi_client-0.1.0a2/esi_client/docs/GetInsurancePricesLevel.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashAttacker.md` & `esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashAttacker.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashItem.md` & `esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashItem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashItemsItem.md` & `esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashItemsItem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetKillmailsKillmailIdKillmailHashVictim.md` & `esi_client-0.1.0a2/esi_client/docs/GetKillmailsKillmailIdKillmailHashVictim.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetLoyaltyStoresCorporationIdOffers200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetLoyaltyStoresCorporationIdOffers200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetLoyaltyStoresCorporationIdOffersNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetLoyaltyStoresCorporationIdOffersNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetLoyaltyStoresCorporationIdOffersRequiredItem.md` & `esi_client-0.1.0a2/esi_client/docs/GetLoyaltyStoresCorporationIdOffersRequiredItem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsGroupsMarketGroupIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsGroupsMarketGroupIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsGroupsMarketGroupIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsGroupsMarketGroupIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsPrices200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsPrices200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistory200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistory200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistoryError520.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistoryError520.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistoryNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistoryNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdHistoryUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdHistoryUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdOrders200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdOrders200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdOrdersNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdOrdersNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsRegionIdOrdersUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsRegionIdOrdersUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetMarketsStructuresStructureId200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetMarketsStructuresStructureId200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetOpportunitiesGroupsGroupIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetOpportunitiesGroupsGroupIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetOpportunitiesTasksTaskIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetOpportunitiesTasksTaskIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetRouteOriginDestinationNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetRouteOriginDestinationNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetSovereigntyCampaigns200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetSovereigntyCampaigns200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetSovereigntyCampaignsParticipant.md` & `esi_client-0.1.0a2/esi_client/docs/GetSovereigntyCampaignsParticipant.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetSovereigntyMap200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetSovereigntyMap200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetSovereigntyStructures200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetSovereigntyStructures200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetStatusOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetStatusOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseAncestries200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseAncestries200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseAsteroidBeltsAsteroidBeltIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseBloodlines200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseBloodlines200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseCategoriesCategoryIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseCategoriesCategoryIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseCategoriesCategoryIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseCategoriesCategoryIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseConstellationsConstellationIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseConstellationsConstellationIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseConstellationsConstellationIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseConstellationsConstellationIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseConstellationsConstellationIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseConstellationsConstellationIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseFactions200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseFactions200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseGraphicsGraphicIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseGraphicsGraphicIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseGraphicsGraphicIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseGraphicsGraphicIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseGroupsGroupIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseGroupsGroupIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseGroupsGroupIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseGroupsGroupIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseMoonsMoonIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseMoonsMoonIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseMoonsMoonIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseMoonsMoonIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseMoonsMoonIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseMoonsMoonIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniversePlanetsPlanetIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniversePlanetsPlanetIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniversePlanetsPlanetIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniversePlanetsPlanetIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniversePlanetsPlanetIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniversePlanetsPlanetIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseRaces200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseRaces200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseRegionsRegionIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseRegionsRegionIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseRegionsRegionIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseRegionsRegionIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSchematicsSchematicIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSchematicsSchematicIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSchematicsSchematicIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSchematicsSchematicIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdDestination.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdDestination.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStargatesStargateIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStargatesStargateIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStarsStarIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStarsStarIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStationsStationIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStationsStationIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStationsStationIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStationsStationIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStationsStationIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStationsStationIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStructuresStructureIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStructuresStructureIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStructuresStructureIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStructuresStructureIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseStructuresStructureIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseStructuresStructureIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemJumps200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemJumps200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemKills200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemKills200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdPlanet.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdPlanet.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseSystemsSystemIdPosition.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseSystemsSystemIdPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdDogmaAttribute.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdDogmaAttribute.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdDogmaEffect.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdDogmaEffect.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetUniverseTypesTypeIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetUniverseTypesTypeIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdAggressor.md` & `esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdAggressor.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdAlly.md` & `esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdAlly.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdDefender.md` & `esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdDefender.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdKillmails200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdKillmails200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdKillmailsUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdKillmailsUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdOk.md` & `esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/GetWarsWarIdUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/GetWarsWarIdUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/IncursionsApi.md` & `esi_client-0.1.0a2/esi_client/docs/IncursionsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/IndustryApi.md` & `esi_client-0.1.0a2/esi_client/docs/IndustryApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/InsuranceApi.md` & `esi_client-0.1.0a2/esi_client/docs/InsuranceApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/InternalServerError.md` & `esi_client-0.1.0a2/esi_client/docs/InternalServerError.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/KillmailsApi.md` & `esi_client-0.1.0a2/esi_client/docs/KillmailsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/LocationApi.md` & `esi_client-0.1.0a2/esi_client/docs/LocationApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/LoyaltyApi.md` & `esi_client-0.1.0a2/esi_client/docs/LoyaltyApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/MailApi.md` & `esi_client-0.1.0a2/esi_client/docs/MailApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/MarketApi.md` & `esi_client-0.1.0a2/esi_client/docs/MarketApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/OpportunitiesApi.md` & `esi_client-0.1.0a2/esi_client/docs/OpportunitiesApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PlanetaryInteractionApi.md` & `esi_client-0.1.0a2/esi_client/docs/PlanetaryInteractionApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersAffiliation200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersAffiliation200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdAssetsLocations200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdAssetsLocations200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdAssetsLocationsPosition.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdAssetsLocationsPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdAssetsNames200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdAssetsNames200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdContactsError520.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdContactsError520.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdFittingsCreated.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdFittingsCreated.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdFittingsFitting.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdFittingsFitting.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdFittingsItem.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdFittingsItem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailError520.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailError520.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailLabelsLabel.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailLabelsLabel.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailMail.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailMail.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCharactersCharacterIdMailRecipient.md` & `esi_client-0.1.0a2/esi_client/docs/PostCharactersCharacterIdMailRecipient.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsLocations200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsLocations200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsPosition.md` & `esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsLocationsPosition.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsNames200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsNames200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostCorporationsCorporationIdAssetsNamesNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PostCorporationsCorporationIdAssetsNamesNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdMembersInvitation.md` & `esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdMembersInvitation.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdMembersNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdMembersNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdMembersUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdMembersUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsCreated.md` & `esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsCreated.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsCreated.md` & `esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsCreated.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PostFleetsFleetIdWingsWingIdSquadsNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUiOpenwindowNewmailNewMail.md` & `esi_client-0.1.0a2/esi_client/docs/PostUiOpenwindowNewmailNewMail.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUiOpenwindowNewmailUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/PostUiOpenwindowNewmailUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsAgent.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsAgent.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsAlliance.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsAlliance.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsCharacter.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsCharacter.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsConstellation.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsConstellation.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsCorporation.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsCorporation.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsFaction.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsFaction.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsInventoryType.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsInventoryType.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsOk.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsOk.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsRegion.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsRegion.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsStation.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsStation.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseIdsSystem.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseIdsSystem.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseNames200Ok.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseNames200Ok.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PostUniverseNamesNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PostUniverseNamesNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutCharactersCharacterIdCalendarEventIdResponse.md` & `esi_client-0.1.0a2/esi_client/docs/PutCharactersCharacterIdCalendarEventIdResponse.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutCharactersCharacterIdMailMailIdContents.md` & `esi_client-0.1.0a2/esi_client/docs/PutCharactersCharacterIdMailMailIdContents.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdMembersMemberIdMovement.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdMembersMemberIdMovement.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdMembersMemberIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdMembersMemberIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdMembersMemberIdUnprocessableEntity.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdMembersMemberIdUnprocessableEntity.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdNewSettings.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdNewSettings.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNaming.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNaming.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdSquadsSquadIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdWingsWingIdNaming.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdWingsWingIdNaming.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/PutFleetsFleetIdWingsWingIdNotFound.md` & `esi_client-0.1.0a2/esi_client/docs/PutFleetsFleetIdWingsWingIdNotFound.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/RoutesApi.md` & `esi_client-0.1.0a2/esi_client/docs/RoutesApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/SearchApi.md` & `esi_client-0.1.0a2/esi_client/docs/SearchApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/ServiceUnavailable.md` & `esi_client-0.1.0a2/esi_client/docs/ServiceUnavailable.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/SkillsApi.md` & `esi_client-0.1.0a2/esi_client/docs/SkillsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/SovereigntyApi.md` & `esi_client-0.1.0a2/esi_client/docs/SovereigntyApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/StatusApi.md` & `esi_client-0.1.0a2/esi_client/docs/StatusApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/Unauthorized.md` & `esi_client-0.1.0a2/esi_client/docs/Unauthorized.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/UniverseApi.md` & `esi_client-0.1.0a2/esi_client/docs/UniverseApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/UserInterfaceApi.md` & `esi_client-0.1.0a2/esi_client/docs/UserInterfaceApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/WalletApi.md` & `esi_client-0.1.0a2/esi_client/docs/WalletApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/docs/WarsApi.md` & `esi_client-0.1.0a2/esi_client/docs/WarsApi.md`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/bad_request.py` & `esi_client-0.1.0a2/esi_client/model/bad_request.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/delete_fleets_fleet_id_members_member_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/delete_fleets_fleet_id_members_member_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/delete_fleets_fleet_id_squads_squad_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/delete_fleets_fleet_id_squads_squad_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/delete_fleets_fleet_id_wings_wing_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/delete_fleets_fleet_id_wings_wing_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/error_limited.py` & `esi_client-0.1.0a2/esi_client/model/error_limited.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/forbidden.py` & `esi_client-0.1.0a2/esi_client/model/forbidden.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/gateway_timeout.py` & `esi_client-0.1.0a2/esi_client/model/gateway_timeout.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_contacts_labels200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_contacts_labels200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_icons_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_icons_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_icons_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_icons_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_alliances_alliance_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_alliances_alliance_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_agents_research200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_agents_research200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_assets200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_assets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_assets_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_assets_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_attributes_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_attributes_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_blueprints200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_blueprints200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks_coordinates.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks_coordinates.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks_folders200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks_folders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_bookmarks_item.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_bookmarks_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_attendees200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_attendees200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_attendees_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_attendees_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_calendar_event_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_calendar_event_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_clones_home_location.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_clones_home_location.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_clones_jump_clone.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_clones_jump_clone.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_clones_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_clones_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contacts_labels200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contacts_labels200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_bids200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_bids200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_bids_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_bids_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_items200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_items200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_contracts_contract_id_items_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_contracts_contract_id_items_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_corporationhistory200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_corporationhistory200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fatigue_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fatigue_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fittings200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fittings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fittings_item.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fittings_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fleet_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fleet_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fleet_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fleet_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fw_stats_kills.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fw_stats_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fw_stats_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fw_stats_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_fw_stats_victory_points.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_fw_stats_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_industry_jobs200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_industry_jobs200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_killmails_recent200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_killmails_recent200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_location_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_location_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_loyalty_points200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_loyalty_points200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_labels_label.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_labels_label.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_labels_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_labels_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_lists200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_lists200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_mail_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_mail_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_mail_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_mail_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_mail_id_recipient.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_mail_id_recipient.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mail_recipient.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mail_recipient.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_medals200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_medals200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_medals_graphic.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_medals_graphic.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_mining200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_mining200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_notifications200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_notifications200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_notifications_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_notifications_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_online_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_online_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_opportunities200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_opportunities200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_orders200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_orders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_orders_history200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_orders_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_content.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_content.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_extractor_details.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_extractor_details.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_factory_details.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_factory_details.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_head.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_head.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_link.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_link.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_pin.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_pin.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_planets_planet_id_route.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_planets_planet_id_route.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_portrait_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_portrait_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_portrait_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_portrait_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_roles_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_roles_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_search_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_search_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_ship_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_ship_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_skillqueue200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_skillqueue200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_skills_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_skills_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_skills_skill.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_skills_skill.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_standings200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_standings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_titles200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_titles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_wallet_journal200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_wallet_journal200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_characters_character_id_wallet_transactions200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_characters_character_id_wallet_transactions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_bids_contract_id200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_bids_contract_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_bids_contract_id_forbidden.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_bids_contract_id_forbidden.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_bids_contract_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_bids_contract_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_items_contract_id200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_items_contract_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_items_contract_id_forbidden.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_items_contract_id_forbidden.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_items_contract_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_items_contract_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_region_id200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_region_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_contracts_public_region_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_contracts_public_region_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporation_corporation_id_mining_extractions200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporation_corporation_id_mining_extractions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporation_corporation_id_mining_observers200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporation_corporation_id_mining_observers200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporation_corporation_id_mining_observers_observer_id200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporation_corporation_id_mining_observers_observer_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_alliancehistory200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_alliancehistory200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_assets200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_assets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_blueprints200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_blueprints200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks_coordinates.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks_coordinates.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks_folders200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks_folders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_bookmarks_item.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_bookmarks_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contacts_labels200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contacts_labels200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_containers_logs200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_containers_logs200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_bids_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_error520.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_contracts_contract_id_items_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_customs_offices200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_customs_offices200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_divisions_hangar_hangar.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_divisions_hangar_hangar.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_divisions_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_divisions_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_divisions_wallet_wallet.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_divisions_wallet_wallet.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_facilities200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_facilities200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_fw_stats_kills.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_fw_stats_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_fw_stats_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_fw_stats_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_fw_stats_victory_points.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_fw_stats_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_icons_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_icons_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_icons_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_icons_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_industry_jobs200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_industry_jobs200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_killmails_recent200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_killmails_recent200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_medals200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_medals200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_medals_issued200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_medals_issued200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_members_titles200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_members_titles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_membertracking200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_membertracking200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_orders200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_orders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_orders_history200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_orders_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_roles200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_roles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_roles_history200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_roles_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_shareholders200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_shareholders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_standings200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_standings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_starbases200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_starbases200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_fuel.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_fuel.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_starbases_starbase_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_structures200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_structures200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_structures_service.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_structures_service.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_titles200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_titles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_wallets200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_wallets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_wallets_division_journal200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_wallets_division_journal200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_corporations_corporation_id_wallets_division_transactions200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_corporations_corporation_id_wallets_division_transactions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_attributes_attribute_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_attributes_attribute_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_attributes_attribute_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_attributes_attribute_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_effect.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_dogma_effect.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_dynamic_items_type_id_item_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_dynamic_items_type_id_item_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_effects_effect_id_modifier.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_effects_effect_id_modifier.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_effects_effect_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_effects_effect_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_dogma_effects_effect_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_dogma_effects_effect_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_members200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_members200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_members_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_members_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_wings200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_wings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_wings_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_wings_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fleets_fleet_id_wings_squad.py` & `esi_client-0.1.0a2/esi_client/model/get_fleets_fleet_id_wings_squad.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_active_total_active_total.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_active_total_active_total.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_active_total_active_total1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_active_total_active_total1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_active_total_active_total.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_active_total_active_total.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_active_total_active_total1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_active_total_active_total1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_kills.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_last_week_last_week.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_last_week_last_week.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_last_week_last_week1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_last_week_last_week1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_victory_points.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_characters_yesterday_yesterday1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_active_total_active_total1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_kills.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_last_week_last_week1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_victory_points.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_corporations_yesterday_yesterday1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_kills.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_last_week_last_week.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_last_week_last_week.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_last_week_last_week1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_last_week_last_week1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_victory_points.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_yesterday_yesterday.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_yesterday_yesterday.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_leaderboards_yesterday_yesterday1.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_leaderboards_yesterday_yesterday1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_stats200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_stats200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_stats_kills.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_stats_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_stats_victory_points.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_stats_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_systems200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_systems200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_fw_wars200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_fw_wars200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_incursions200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_incursions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_industry_facilities200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_industry_facilities200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_industry_systems200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_industry_systems200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_industry_systems_cost_indice.py` & `esi_client-0.1.0a2/esi_client/model/get_industry_systems_cost_indice.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_insurance_prices200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_insurance_prices200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_insurance_prices_level.py` & `esi_client-0.1.0a2/esi_client/model/get_insurance_prices_level.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_attacker.py` & `esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_attacker.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_item.py` & `esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_items_item.py` & `esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_items_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_position.py` & `esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_killmails_killmail_id_killmail_hash_victim.py` & `esi_client-0.1.0a2/esi_client/model/get_killmails_killmail_id_killmail_hash_victim.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_loyalty_stores_corporation_id_offers200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_loyalty_stores_corporation_id_offers200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_loyalty_stores_corporation_id_offers_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_loyalty_stores_corporation_id_offers_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_loyalty_stores_corporation_id_offers_required_item.py` & `esi_client-0.1.0a2/esi_client/model/get_loyalty_stores_corporation_id_offers_required_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_groups_market_group_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_groups_market_group_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_groups_market_group_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_groups_market_group_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_prices200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_prices200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history_error520.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_region_id_history_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_region_id_history_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_region_id_orders200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_region_id_orders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_region_id_orders_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_region_id_orders_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_region_id_orders_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_region_id_orders_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_markets_structures_structure_id200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_markets_structures_structure_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_opportunities_groups_group_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_opportunities_groups_group_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_opportunities_tasks_task_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_opportunities_tasks_task_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_route_origin_destination_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_route_origin_destination_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_sovereignty_campaigns200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_sovereignty_campaigns200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_sovereignty_campaigns_participant.py` & `esi_client-0.1.0a2/esi_client/model/get_sovereignty_campaigns_participant.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_sovereignty_map200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_sovereignty_map200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_sovereignty_structures200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_sovereignty_structures200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_status_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_status_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_ancestries200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_ancestries200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_asteroid_belts_asteroid_belt_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_bloodlines200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_bloodlines200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_categories_category_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_categories_category_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_categories_category_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_categories_category_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_constellations_constellation_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_constellations_constellation_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_constellations_constellation_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_constellations_constellation_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_constellations_constellation_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_constellations_constellation_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_factions200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_factions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_graphics_graphic_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_graphics_graphic_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_graphics_graphic_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_graphics_graphic_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_groups_group_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_groups_group_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_groups_group_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_groups_group_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_moons_moon_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_moons_moon_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_moons_moon_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_moons_moon_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_moons_moon_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_moons_moon_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_planets_planet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_planets_planet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_planets_planet_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_planets_planet_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_planets_planet_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_planets_planet_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_races200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_races200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_regions_region_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_regions_region_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_regions_region_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_regions_region_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_schematics_schematic_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_schematics_schematic_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_schematics_schematic_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_schematics_schematic_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_destination.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_destination.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stargates_stargate_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stargates_stargate_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stars_star_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stars_star_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stations_station_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stations_station_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stations_station_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stations_station_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_stations_station_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_stations_station_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_structures_structure_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_structures_structure_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_structures_structure_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_structures_structure_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_structures_structure_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_structures_structure_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_system_jumps200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_system_jumps200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_system_kills200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_system_kills200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_planet.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_planet.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_systems_system_id_position.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_systems_system_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_dogma_attribute.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_dogma_attribute.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_dogma_effect.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_dogma_effect.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_universe_types_type_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_universe_types_type_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_wars_war_id_aggressor.py` & `esi_client-0.1.0a2/esi_client/model/get_wars_war_id_aggressor.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_wars_war_id_ally.py` & `esi_client-0.1.0a2/esi_client/model/get_wars_war_id_ally.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_wars_war_id_defender.py` & `esi_client-0.1.0a2/esi_client/model/get_wars_war_id_defender.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_wars_war_id_killmails200_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_wars_war_id_killmails200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_wars_war_id_killmails_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/get_wars_war_id_killmails_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_wars_war_id_ok.py` & `esi_client-0.1.0a2/esi_client/model/get_wars_war_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/get_wars_war_id_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/get_wars_war_id_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/internal_server_error.py` & `esi_client-0.1.0a2/esi_client/model/internal_server_error.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_affiliation200_ok.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_affiliation200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_assets_locations200_ok.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_assets_locations200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_assets_locations_position.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_assets_locations_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_assets_names200_ok.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_assets_names200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_contacts_error520.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_contacts_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_fittings_created.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_fittings_created.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_fittings_fitting.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_fittings_fitting.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_fittings_item.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_fittings_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_error520.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_labels_label.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_labels_label.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_mail.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_mail.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_characters_character_id_mail_recipient.py` & `esi_client-0.1.0a2/esi_client/model/post_characters_character_id_mail_recipient.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_locations200_ok.py` & `esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_locations200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_locations_not_found.py` & `esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_locations_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_locations_position.py` & `esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_locations_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_names200_ok.py` & `esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_names200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_corporations_corporation_id_assets_names_not_found.py` & `esi_client-0.1.0a2/esi_client/model/post_corporations_corporation_id_assets_names_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_members_invitation.py` & `esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_members_invitation.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_members_not_found.py` & `esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_members_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_members_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_members_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_created.py` & `esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_created.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_not_found.py` & `esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_created.py` & `esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_created.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_not_found.py` & `esi_client-0.1.0a2/esi_client/model/post_fleets_fleet_id_wings_wing_id_squads_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_ui_openwindow_newmail_new_mail.py` & `esi_client-0.1.0a2/esi_client/model/post_ui_openwindow_newmail_new_mail.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_ui_openwindow_newmail_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/post_ui_openwindow_newmail_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_agent.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_agent.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_alliance.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_alliance.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_character.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_character.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_constellation.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_constellation.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_corporation.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_corporation.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_faction.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_faction.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_inventory_type.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_inventory_type.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_ok.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_region.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_region.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_station.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_station.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_ids_system.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_ids_system.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_names200_ok.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_names200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/post_universe_names_not_found.py` & `esi_client-0.1.0a2/esi_client/model/post_universe_names_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_characters_character_id_calendar_event_id_response.py` & `esi_client-0.1.0a2/esi_client/model/put_characters_character_id_calendar_event_id_response.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_characters_character_id_mail_mail_id_contents.py` & `esi_client-0.1.0a2/esi_client/model/put_characters_character_id_mail_mail_id_contents.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_members_member_id_movement.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_members_member_id_movement.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_members_member_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_members_member_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_members_member_id_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_members_member_id_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_new_settings.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_new_settings.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_squads_squad_id_naming.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_squads_squad_id_naming.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_squads_squad_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_squads_squad_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_wings_wing_id_naming.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_wings_wing_id_naming.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/put_fleets_fleet_id_wings_wing_id_not_found.py` & `esi_client-0.1.0a2/esi_client/model/put_fleets_fleet_id_wings_wing_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/service_unavailable.py` & `esi_client-0.1.0a2/esi_client/model/service_unavailable.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/model/unauthorized.py` & `esi_client-0.1.0a2/esi_client/model/unauthorized.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/models/__init__.py` & `esi_client-0.1.0a2/esi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_alliance_api.py` & `esi_client-0.1.0a2/esi_client/test/test_alliance_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_assets_api.py` & `esi_client-0.1.0a2/esi_client/test/test_assets_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_bad_request.py` & `esi_client-0.1.0a2/esi_client/test/test_bad_request.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_bookmarks_api.py` & `esi_client-0.1.0a2/esi_client/test/test_bookmarks_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_calendar_api.py` & `esi_client-0.1.0a2/esi_client/test/test_calendar_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_character_api.py` & `esi_client-0.1.0a2/esi_client/test/test_character_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_clones_api.py` & `esi_client-0.1.0a2/esi_client/test/test_clones_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_contacts_api.py` & `esi_client-0.1.0a2/esi_client/test/test_contacts_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_contracts_api.py` & `esi_client-0.1.0a2/esi_client/test/test_contracts_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_corporation_api.py` & `esi_client-0.1.0a2/esi_client/test/test_corporation_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_delete_characters_character_id_mail_labels_label_id_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_delete_fleets_fleet_id_members_member_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_delete_fleets_fleet_id_members_member_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_delete_fleets_fleet_id_squads_squad_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_delete_fleets_fleet_id_squads_squad_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_delete_fleets_fleet_id_wings_wing_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_delete_fleets_fleet_id_wings_wing_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_dogma_api.py` & `esi_client-0.1.0a2/esi_client/test/test_dogma_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_error_limited.py` & `esi_client-0.1.0a2/esi_client/test/test_error_limited.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_faction_warfare_api.py` & `esi_client-0.1.0a2/esi_client/test/test_faction_warfare_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_fittings_api.py` & `esi_client-0.1.0a2/esi_client/test/test_fittings_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_fleets_api.py` & `esi_client-0.1.0a2/esi_client/test/test_fleets_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_forbidden.py` & `esi_client-0.1.0a2/esi_client/test/test_forbidden.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_gateway_timeout.py` & `esi_client-0.1.0a2/esi_client/test/test_gateway_timeout.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_contacts_labels200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_contacts_labels200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_icons_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_icons_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_icons_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_icons_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_alliances_alliance_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_alliances_alliance_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_agents_research200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_agents_research200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_assets200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_assets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_assets_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_assets_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_attributes_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_attributes_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_blueprints200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_blueprints200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks_coordinates.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks_coordinates.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks_folders200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks_folders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_bookmarks_item.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_bookmarks_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_attendees_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_calendar_event_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_calendar_event_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_clones_home_location.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_clones_home_location.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_clones_jump_clone.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_clones_jump_clone.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_clones_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_clones_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contacts_labels200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contacts_labels200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_bids_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_items200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_items200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_contracts_contract_id_items_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_contracts_contract_id_items_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_corporationhistory200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_corporationhistory200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fatigue_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fatigue_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fittings200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fittings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fittings_item.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fittings_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fleet_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fleet_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fleet_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fleet_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fw_stats_kills.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fw_stats_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fw_stats_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fw_stats_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_fw_stats_victory_points.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_fw_stats_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_industry_jobs200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_industry_jobs200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_killmails_recent200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_killmails_recent200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_location_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_location_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_loyalty_points200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_loyalty_points200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_labels_label.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_labels_label.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_labels_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_labels_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_lists200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_lists200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_mail_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_mail_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_mail_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_mail_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_mail_id_recipient.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_mail_id_recipient.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mail_recipient.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mail_recipient.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_medals200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_medals200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_medals_graphic.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_medals_graphic.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_mining200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_mining200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_notifications200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_notifications200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_notifications_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_notifications_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_online_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_online_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_opportunities200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_opportunities200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_orders200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_orders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_orders_history200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_orders_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_content.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_content.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_extractor_details.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_extractor_details.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_factory_details.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_factory_details.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_head.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_head.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_link.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_link.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_pin.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_pin.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_planets_planet_id_route.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_planets_planet_id_route.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_portrait_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_portrait_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_portrait_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_portrait_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_roles_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_roles_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_search_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_search_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_ship_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_ship_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_skillqueue200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_skillqueue200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_skills_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_skills_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_skills_skill.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_skills_skill.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_standings200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_standings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_titles200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_titles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_wallet_journal200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_wallet_journal200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_characters_character_id_wallet_transactions200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_characters_character_id_wallet_transactions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_bids_contract_id200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_bids_contract_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_bids_contract_id_forbidden.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_bids_contract_id_forbidden.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_bids_contract_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_bids_contract_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_items_contract_id200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_items_contract_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_items_contract_id_forbidden.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_items_contract_id_forbidden.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_items_contract_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_items_contract_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_region_id200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_region_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_contracts_public_region_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_contracts_public_region_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporation_corporation_id_mining_extractions200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporation_corporation_id_mining_extractions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporation_corporation_id_mining_observers200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporation_corporation_id_mining_observers200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporation_corporation_id_mining_observers_observer_id200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporation_corporation_id_mining_observers_observer_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_alliancehistory200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_alliancehistory200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_assets200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_assets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_blueprints200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_blueprints200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks_coordinates.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks_coordinates.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks_folders200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks_folders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_bookmarks_item.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_bookmarks_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contacts200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contacts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contacts_labels200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contacts_labels200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_containers_logs200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_containers_logs200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_bids_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_error520.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_contracts_contract_id_items_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_customs_offices200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_customs_offices200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_divisions_hangar_hangar.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_divisions_hangar_hangar.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_divisions_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_divisions_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_divisions_wallet_wallet.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_divisions_wallet_wallet.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_facilities200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_facilities200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_fw_stats_kills.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_fw_stats_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_fw_stats_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_fw_stats_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_fw_stats_victory_points.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_fw_stats_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_icons_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_icons_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_icons_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_icons_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_industry_jobs200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_industry_jobs200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_killmails_recent200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_killmails_recent200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_medals200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_medals200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_medals_issued200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_medals_issued200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_members_titles200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_members_titles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_membertracking200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_membertracking200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_orders200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_orders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_orders_history200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_orders_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_roles200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_roles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_roles_history200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_roles_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_shareholders200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_shareholders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_standings200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_standings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_starbases200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_starbases200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_fuel.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_fuel.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_starbases_starbase_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_structures200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_structures200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_structures_service.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_structures_service.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_titles200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_titles200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_wallets200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_wallets200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_wallets_division_journal200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_wallets_division_journal200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_corporations_corporation_id_wallets_division_transactions200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_corporations_corporation_id_wallets_division_transactions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_attributes_attribute_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_attributes_attribute_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_attributes_attribute_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_attributes_attribute_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_attribute.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_effect.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_dogma_effect.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_dynamic_items_type_id_item_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_effects_effect_id_modifier.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_effects_effect_id_modifier.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_effects_effect_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_effects_effect_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_dogma_effects_effect_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_dogma_effects_effect_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_members200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_members200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_members_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_members_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_wings200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_wings200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_wings_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_wings_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fleets_fleet_id_wings_squad.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fleets_fleet_id_wings_squad.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_active_total_active_total.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_active_total_active_total.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_active_total_active_total1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_active_total_active_total1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_active_total_active_total1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_kills.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_last_week_last_week1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_victory_points.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_characters_yesterday_yesterday1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_active_total_active_total1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_kills.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_last_week_last_week1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_victory_points.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_corporations_yesterday_yesterday1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_kills.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_last_week_last_week.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_last_week_last_week.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_last_week_last_week1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_last_week_last_week1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_victory_points.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday1.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_leaderboards_yesterday_yesterday1.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_stats200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_stats200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_stats_kills.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_stats_kills.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_stats_victory_points.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_stats_victory_points.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_systems200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_systems200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_fw_wars200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_fw_wars200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_incursions200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_incursions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_industry_facilities200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_industry_facilities200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_industry_systems200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_industry_systems200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_industry_systems_cost_indice.py` & `esi_client-0.1.0a2/esi_client/test/test_get_industry_systems_cost_indice.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_insurance_prices200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_insurance_prices200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_insurance_prices_level.py` & `esi_client-0.1.0a2/esi_client/test/test_get_insurance_prices_level.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_attacker.py` & `esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_attacker.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_item.py` & `esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_items_item.py` & `esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_items_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_killmails_killmail_id_killmail_hash_victim.py` & `esi_client-0.1.0a2/esi_client/test/test_get_killmails_killmail_id_killmail_hash_victim.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_loyalty_stores_corporation_id_offers200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_loyalty_stores_corporation_id_offers200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_loyalty_stores_corporation_id_offers_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_loyalty_stores_corporation_id_offers_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_loyalty_stores_corporation_id_offers_required_item.py` & `esi_client-0.1.0a2/esi_client/test/test_get_loyalty_stores_corporation_id_offers_required_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_groups_market_group_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_groups_market_group_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_groups_market_group_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_groups_market_group_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_prices200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_prices200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history_error520.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_history_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_history_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_orders200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_orders200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_orders_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_orders_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_region_id_orders_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_region_id_orders_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_markets_structures_structure_id200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_markets_structures_structure_id200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_opportunities_groups_group_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_opportunities_groups_group_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_opportunities_tasks_task_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_opportunities_tasks_task_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_route_origin_destination_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_route_origin_destination_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_campaigns200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_campaigns200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_campaigns_participant.py` & `esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_campaigns_participant.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_map200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_map200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_sovereignty_structures200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_sovereignty_structures200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_status_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_status_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_ancestries200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_ancestries200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_asteroid_belts_asteroid_belt_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_bloodlines200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_bloodlines200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_categories_category_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_categories_category_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_categories_category_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_categories_category_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_constellations_constellation_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_constellations_constellation_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_constellations_constellation_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_constellations_constellation_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_constellations_constellation_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_constellations_constellation_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_factions200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_factions200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_graphics_graphic_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_graphics_graphic_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_graphics_graphic_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_graphics_graphic_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_groups_group_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_groups_group_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_groups_group_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_groups_group_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_moons_moon_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_moons_moon_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_moons_moon_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_moons_moon_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_moons_moon_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_moons_moon_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_planets_planet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_planets_planet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_planets_planet_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_planets_planet_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_planets_planet_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_planets_planet_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_races200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_races200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_regions_region_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_regions_region_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_regions_region_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_regions_region_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_schematics_schematic_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_schematics_schematic_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_schematics_schematic_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_schematics_schematic_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_destination.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_destination.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stargates_stargate_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stargates_stargate_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stars_star_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stars_star_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stations_station_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stations_station_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stations_station_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stations_station_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_stations_station_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_stations_station_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_structures_structure_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_structures_structure_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_structures_structure_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_structures_structure_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_structures_structure_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_structures_structure_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_system_jumps200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_system_jumps200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_system_kills200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_system_kills200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_planet.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_planet.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_systems_system_id_position.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_systems_system_id_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_dogma_attribute.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_dogma_attribute.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_dogma_effect.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_dogma_effect.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_universe_types_type_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_universe_types_type_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_aggressor.py` & `esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_aggressor.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_ally.py` & `esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_ally.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_defender.py` & `esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_defender.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_killmails200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_killmails200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_killmails_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_killmails_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_get_wars_war_id_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_get_wars_war_id_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_incursions_api.py` & `esi_client-0.1.0a2/esi_client/test/test_incursions_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_industry_api.py` & `esi_client-0.1.0a2/esi_client/test/test_industry_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_insurance_api.py` & `esi_client-0.1.0a2/esi_client/test/test_insurance_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_internal_server_error.py` & `esi_client-0.1.0a2/esi_client/test/test_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_killmails_api.py` & `esi_client-0.1.0a2/esi_client/test/test_killmails_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_location_api.py` & `esi_client-0.1.0a2/esi_client/test/test_location_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_loyalty_api.py` & `esi_client-0.1.0a2/esi_client/test/test_loyalty_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_mail_api.py` & `esi_client-0.1.0a2/esi_client/test/test_mail_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_market_api.py` & `esi_client-0.1.0a2/esi_client/test/test_market_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_opportunities_api.py` & `esi_client-0.1.0a2/esi_client/test/test_opportunities_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_planetary_interaction_api.py` & `esi_client-0.1.0a2/esi_client/test/test_planetary_interaction_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_affiliation200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_affiliation200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_assets_locations200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_assets_locations200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_assets_locations_position.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_assets_locations_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_assets_names200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_assets_names200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_contacts_error520.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_contacts_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_fittings_created.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_fittings_created.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_fittings_fitting.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_fittings_fitting.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_fittings_item.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_fittings_item.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_error520.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_error520.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_labels_label.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_labels_label.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_mail.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_mail.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_characters_character_id_mail_recipient.py` & `esi_client-0.1.0a2/esi_client/test/test_post_characters_character_id_mail_recipient.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_locations200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_locations200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_locations_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_locations_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_locations_position.py` & `esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_locations_position.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_names200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_names200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_corporations_corporation_id_assets_names_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_post_corporations_corporation_id_assets_names_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_members_invitation.py` & `esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_members_invitation.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_members_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_members_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_members_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_members_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_created.py` & `esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_created.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_created.py` & `esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_created.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_post_fleets_fleet_id_wings_wing_id_squads_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_ui_openwindow_newmail_new_mail.py` & `esi_client-0.1.0a2/esi_client/test/test_post_ui_openwindow_newmail_new_mail.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_ui_openwindow_newmail_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_post_ui_openwindow_newmail_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_agent.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_agent.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_alliance.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_alliance.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_character.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_character.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_constellation.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_constellation.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_corporation.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_corporation.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_faction.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_faction.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_inventory_type.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_inventory_type.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_region.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_region.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_station.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_station.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_ids_system.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_ids_system.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_names200_ok.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_names200_ok.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_post_universe_names_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_post_universe_names_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_characters_character_id_calendar_event_id_response.py` & `esi_client-0.1.0a2/esi_client/test/test_put_characters_character_id_calendar_event_id_response.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_characters_character_id_mail_mail_id_contents.py` & `esi_client-0.1.0a2/esi_client/test/test_put_characters_character_id_mail_mail_id_contents.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_members_member_id_movement.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_members_member_id_movement.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_members_member_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_members_member_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_members_member_id_unprocessable_entity.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_members_member_id_unprocessable_entity.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_new_settings.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_new_settings.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_naming.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_naming.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_squads_squad_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_naming.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_naming.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_not_found.py` & `esi_client-0.1.0a2/esi_client/test/test_put_fleets_fleet_id_wings_wing_id_not_found.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_routes_api.py` & `esi_client-0.1.0a2/esi_client/test/test_routes_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_search_api.py` & `esi_client-0.1.0a2/esi_client/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_service_unavailable.py` & `esi_client-0.1.0a2/esi_client/test/test_service_unavailable.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_skills_api.py` & `esi_client-0.1.0a2/esi_client/test/test_skills_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_sovereignty_api.py` & `esi_client-0.1.0a2/esi_client/test/test_sovereignty_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_status_api.py` & `esi_client-0.1.0a2/esi_client/test/test_status_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_unauthorized.py` & `esi_client-0.1.0a2/esi_client/test/test_unauthorized.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_universe_api.py` & `esi_client-0.1.0a2/esi_client/test/test_universe_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_user_interface_api.py` & `esi_client-0.1.0a2/esi_client/test/test_user_interface_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_wallet_api.py` & `esi_client-0.1.0a2/esi_client/test/test_wallet_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/esi_client/test/test_wars_api.py` & `esi_client-0.1.0a2/esi_client/test/test_wars_api.py`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/LICENSE` & `esi_client-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/README.md` & `esi_client-0.1.0a2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # esi-client
 
 A Python client for accessing the complete Eve Online ESI API.
 
 [![release](https://img.shields.io/pypi/v/esi-client?label=release)](https://pypi.org/project/esi-client/)
 [![python](https://img.shields.io/pypi/pyversions/esi-client)](https://pypi.org/project/esi-client/)
-[![ESI](https://img.shields.io/badge/ESI-1.17-orange)](https://esi.evetech.net/ui/)
+[![openapi](https://img.shields.io/badge/openapigen-6.6.0_SNAPSHOT-blue)](https://esi.evetech.net/ui/)
+[![ESI](https://img.shields.io/badge/ESI-1.17-blue)](https://esi.evetech.net/ui/)
 [![pipeline status](https://gitlab.com/ErikKalkoken/esi-client-generator/badges/main/pipeline.svg)](https://gitlab.com/ErikKalkoken/esi-client-generator/-/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/esi-client/-/blob/master/LICENSE)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
+## Contents
+
+- [Overview](#overview)
+- [Installation](#installation)
+- [Usage](#usage)
+
 ## Overview
 
 This package is a library that provides a Python client for accessing the public 3rd party API of EVE Online, which is more commonly known as "ESI" (EVE Swagger Interface).
 
 The client is automatically generated from ESI's specification with the [Open API generator](https://openapi-generator.tech/).
 
 This approach offers many benefits in comparison to other ESI libraries:
 
 - Complete and correct coverage of all endpoints
 - Automatic serialization and mapping to Python data types
 - Python classes for all data models
-- Full type annotations
+- Type annotations, i.e. enabling auto complete for API methods
 - No delay at startup for building the client
 - Robust and proven API client
 - Fast turnaround on API updates
 
 ## Installation
 
 You can install the current this library directly from PyPI:
@@ -111,22 +118,40 @@
     api_instance = CharacterApi(api_client)
     api_response = api_instance.get_characters_character_id_medals(
         character_id=93330670
     )
     ...
 ```
 
-### Token as parameter
+#### Token as parameter
 
 Another way of providing your access token is as parameter when making the call to the endpoint:
 
 ```python
 from esi_client.api.character_api import CharacterApi
 
 api_instance = CharacterApi(api_client)
 api_response = api_instance.get_characters_character_id_medals(
     character_id=93330670, token="ACCESS-TOKEN"
 )
-... 
+```
+
+### Getting HTTP information for a response
+
+In some cases you also need to get the HTTP information for a response. e.g. if a endpoint supports paging the information about how many pages there are is in the HTTP header.
+
+To get the HTTP information you need to pass the argument `_return_http_data_only=False` when calling the API method. The API method will then return a tuple consisting of:
+
+- data
+- HTTP status code
+- HTTP response headers
+
+Here is an example:
+
+```python
+from esi_client.api.universe_api import UniverseApi
+
+api = UniverseApi()
+data, status_code, header = api.get_universe_types(_return_http_data_only=False)
 ```
 
 The source code for these examples can also be found in project's `examples` folder.
```

### Comparing `esi_client-0.1.0a1/pyproject.toml` & `esi_client-0.1.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esi_client-0.1.0a1/PKG-INFO` & `esi_client-0.1.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-client
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A Python client for accessing the complete Eve Online ESI API.
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/esi-client-generator
 Maintainer-email: Erik Kalkoken <kalkoken87@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Erik Kalkoken
         
@@ -49,31 +49,38 @@
 
 # esi-client
 
 A Python client for accessing the complete Eve Online ESI API.
 
 [![release](https://img.shields.io/pypi/v/esi-client?label=release)](https://pypi.org/project/esi-client/)
 [![python](https://img.shields.io/pypi/pyversions/esi-client)](https://pypi.org/project/esi-client/)
-[![ESI](https://img.shields.io/badge/ESI-1.17-orange)](https://esi.evetech.net/ui/)
+[![openapi](https://img.shields.io/badge/openapigen-6.6.0_SNAPSHOT-blue)](https://esi.evetech.net/ui/)
+[![ESI](https://img.shields.io/badge/ESI-1.17-blue)](https://esi.evetech.net/ui/)
 [![pipeline status](https://gitlab.com/ErikKalkoken/esi-client-generator/badges/main/pipeline.svg)](https://gitlab.com/ErikKalkoken/esi-client-generator/-/commits/main)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/esi-client/-/blob/master/LICENSE)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
+## Contents
+
+- [Overview](#overview)
+- [Installation](#installation)
+- [Usage](#usage)
+
 ## Overview
 
 This package is a library that provides a Python client for accessing the public 3rd party API of EVE Online, which is more commonly known as "ESI" (EVE Swagger Interface).
 
 The client is automatically generated from ESI's specification with the [Open API generator](https://openapi-generator.tech/).
 
 This approach offers many benefits in comparison to other ESI libraries:
 
 - Complete and correct coverage of all endpoints
 - Automatic serialization and mapping to Python data types
 - Python classes for all data models
-- Full type annotations
+- Type annotations, i.e. enabling auto complete for API methods
 - No delay at startup for building the client
 - Robust and proven API client
 - Fast turnaround on API updates
 
 ## Installation
 
 You can install the current this library directly from PyPI:
@@ -160,22 +167,40 @@
     api_instance = CharacterApi(api_client)
     api_response = api_instance.get_characters_character_id_medals(
         character_id=93330670
     )
     ...
 ```
 
-### Token as parameter
+#### Token as parameter
 
 Another way of providing your access token is as parameter when making the call to the endpoint:
 
 ```python
 from esi_client.api.character_api import CharacterApi
 
 api_instance = CharacterApi(api_client)
 api_response = api_instance.get_characters_character_id_medals(
     character_id=93330670, token="ACCESS-TOKEN"
 )
-... 
+```
+
+### Getting HTTP information for a response
+
+In some cases you also need to get the HTTP information for a response. e.g. if a endpoint supports paging the information about how many pages there are is in the HTTP header.
+
+To get the HTTP information you need to pass the argument `_return_http_data_only=False` when calling the API method. The API method will then return a tuple consisting of:
+
+- data
+- HTTP status code
+- HTTP response headers
+
+Here is an example:
+
+```python
+from esi_client.api.universe_api import UniverseApi
+
+api = UniverseApi()
+data, status_code, header = api.get_universe_types(_return_http_data_only=False)
 ```
 
 The source code for these examples can also be found in project's `examples` folder.
```

