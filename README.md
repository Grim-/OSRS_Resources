# OSRS_Resources
A selection of resources I have either parsed or found relating to OSRS Fan site development.

I will be uploading the code used to parse the information at a later time so others can update at any time.



OSRS_GE_ITEM_DETAILS: Contains all items parsed from OSRS GE Catalogue in seperate aplhabetical files and all in one (all_in_one.json) the price data won't be very useful but I wanted to offer it exactly as I parsed it.

{
	"icon":"http://services.runescape.com/m=itemdb_oldschool/1510570893006_obj_sprite.gif?id=890",
	"icon_large":"http://services.runescape.com/m=itemdb_oldschool/1510570893006_obj_big.gif?id=890",
	"id":890,
	"type":"Default",
	"typeIcon":"http://www.runescape.com/img/categories/Default",
	"name":"Adamant arrow",
	"description":"Arrows with adamant heads.",
	"current":{
	  "trend":"neutral",
		"price":57
		},
	"today":{
	  "trend":"neutral",
		"price":0
		},
	"members":"false"
}


OSRS_ITEM_STATS: Contains every item on http://oldschoolrunescape.wikia.com/wiki/Category:Slot_tables parsed into a json with item name for each item.

    {
        "item-name": "Adamant arrow",
        "stats": {
            "stab-attack": "0",
            "slash-attack": "0",
            "crush-attack": "0",
            "magic-attack": "0",
            "ranged-attack": "0",
            "stab-defence": "0",
            "slash-defence": "0",
            "crush-defence": "0",
            "magic-defence": "0",
            "ranged-defence": "0",
            "strength-bonus": "0",
            "prayer-bonus": "0",
            "ranged-strength": "+31",
            "magic-strength": ""
        },
        "id": "890",
        "tradeable": true
    }


OSRS_ITEM_STATS_MERGED_WITH_GE_DATA: Contains all items parsed from OSRS GE Catalogue and http://oldschoolrunescape.wikia.com/wiki/Category:Slot_tables, for each slot merged together with the useless item price data removed.

a typical item object contained here looks like

    {
        "id": 890,
        "name": "Adamant arrow",
        "description": "Arrows with adamant heads.",
        "stats": {
            "stab-attack": "0",
            "slash-attack": "0",
            "crush-attack": "0",
            "magic-attack": "0",
            "ranged-attack": "0",
            "stab-defence": "0",
            "slash-defence": "0",
            "crush-defence": "0",
            "magic-defence": "0",
            "ranged-defence": "0",
            "strength-bonus": "0",
            "prayer-bonus": "0",
            "ranged-strength": "+31",
            "magic-strength": ""
        },
        "members": "false",
        "tradeable": true
    }

ALL_TRADEABLE_OSRS_ITEM_IMAGES: Contains every picture for items on the OSRS_GE_ITEM_DETAILS pictures are named as [id].png

ALL_OSRS_OBJECTS+ITEMS_WITH_PARTIAL_PICTURES: Contains every picture for items on the OSRS_GE_ITEM_DETAILS pictures are named as [id].png, also included are pictures for a good portion of item pictures (even interactables, doors etc) - this is not complete and isn't likely to be updated.