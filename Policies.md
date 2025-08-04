[
	
	//Expansion 
    {
        "name": "Expansion",
        "era": "Classical era",
        "priorities": {
            "Neutral": 0,
            "Cultural": 0,
            "Diplomatic": 0,
            "Domination": 20,
            "Scientific": 10,
	    "Religious": 0
        },
        "uniques": [
                "Comment [+25% Strength vs Barbarians and City-States units]", "[+25]% Strength <vs [Barbarian] units> <hidden from users>", 
		"[+25]% Strength <vs [City-States]> <hidden from users>",
		 "Adopt [City Militia]", 					"Unavailable",
			"[+25]% weight to this choice for AI decisions"
        ],
        "policies": [
            {
                "name": "City Militia",
                "uniques": [
                    "[-50]% maintenance costs <for [Military] units> <in [City center] tiles>", "[+2 Happiness, +1 Production] [in all cities with a garrison]"
                ],
                "row": 1,
                "column": 3
            },
            {
                "name": "Colonialism",
                "uniques": [
                    "[+1] population [in all cities]",
                    "[+1 Happiness] [in all cities]",
                    "Gain a free [Governor's Mansion] [in this city] <upon founding a city>",
                    "Free [Worker] appears <upon founding a city>",
			"Gain a free [Harbor] [in this city] <upon founding a city> <on foreign continents>",
                ],
                "requires": ["City Militia"],
                "row": 2,
                "column": 2
            },
            {
                "name": "Autarky",
                "uniques": [
                    "Quantity of strategic resources produced by the empire +[50]%",
                    "[+2 Food] [in all cities connected to capital]"
                ],
                "requires": ["City Militia"],
                "row": 2,
                "column": 4
            },
            {
                "name": "Relations",
                "uniques": [
                    "May buy [Diplomat] units for [500] [Faith] [in all cities in which the majority religion is a major religion] at an increasing price ([500]) <starting from the [Medieval era]>"
		],
                "requires": ["Autarky"],
                "row": 3,
                "column": 2
            },
            {
                "name": "State Logistics",
                "uniques": [
                    "[-25]% maintenance on road & railroads", "Improves movement speed on roads"
                ],
                "requires": ["Colonialism"],
                "row": 3,
                "column": 4
            },
            {
                "name": "Expansion Complete",
                "uniques": [
                 "[-25]% Culture cost of natural border growth [in all cities connected to capital]", "[-25]% Gold cost of acquiring tiles [in all cities connected to capital]"
                ]
	    }
	]
    },
    {
        "name": "Humor",
        "era": "Industrial era",
        "priorities": {
            "Neutral": 10,
            "Cultural": 0,
            "Diplomatic": 0,
            "Domination": 10,
            "Scientific": 0
        },
        "uniques": [
            "[+1 Happiness] per [2] population [in all cities]",
		 "Adopt [Comedic Journalism]", 
					"Unavailable",
			"Free Social Policy <if no other Civilization has adopted this>", // Early Adopter (usually provided to the first two civs)
        ],
        "policies": [
            {
                "name": "Comedic Journalism",
                "uniques": [
                    "[+2 Happiness] from every [Broadcast Tower]"
                ],
                "row": 1,
                "column": 1
            },
            {
                "name": "Gelotology",
                "uniques": [
                    "[+1 Happiness] from every [Medical Lab]","[+1 Happiness] from every [Hospital]"
                ],
                "row": 1,
                "column": 3
            },
            {
                "name": "Kabarett",
                "uniques": [
                    "[+2 Culture, +1 Happiness] from every [Amphitheater]","[+2 Culture, +1 Happiness] from every [Theatre]"
                ],
                "requires": ["Comedic Journalism","Gelotology"],
                "row": 2,
                "column": 3
            },
            {
                "name": "Political Cartoon",
                "uniques": [
                    "[+1 Happiness] from all [Culture] buildings <when below [-10] [Happiness]>"
                ],
                "requires": ["Comedic Journalism","Gelotology"],
                "row": 2,
                "column": 5
            },
            {
                "name": "Political Satire",
                "uniques": [
                    "[+1 Happiness] per every [8] [Culture]"
                ],
                "requires": ["Political Cartoon"],
                "row": 3,
                "column": 5
            },
            {
                "name": "Humor Complete",
                "uniques": [
                    "[+2 Happiness, +1 Culture] per [2] population [in all cities]"
                ]
            }
        ]
    },
    {
        "name": "Voluntarism",
        "era": "Industrial era",
        "priorities": {
            "Neutral": 10,
            "Cultural": 0,
            "Diplomatic": 0,
            "Domination": 10,
            "Scientific": 0
        },
        "uniques": [
            "[+2 Production, +2 Food] per [2] population [in capital]",
		 "Adopt [Black Bloc]",
					"Unavailable",
			"Free Social Policy <if no other Civilization has adopted this>", // Early Adopter (usually provided to the first two civs)
        ],
        "policies": [
            {
                "name": "Anarchism",
                "uniques": [
                    "[-50]% unhappiness from the number of cities"
                ],
                "row": 1,
                "column": 1
            },
            {
                "name": "Black Bloc",
                "uniques": [
                    "No movement cost to pillage"
                ],
                "row": 1,
                "column": 3
            },
            {
                "name": "Insurgent Army",
                "uniques": [
                    "[+15]% Strength <for [All] units> <when fighting in [Friendly Land] tiles>"
                ],
                "row": 1,
                "column": 5
            },
            {
                "name": "Mutual Aid",
                "uniques": [
                    "Allied City-States provide [Gold] equal to [+30]% of what they produce for themselves","Allied City-States provide [Food] equal to [+40]% of what they produce for themselves"
                ],
                "requires": ["Anarchism","Black Bloc","Insurgent Army"],
                "row": 2,
                "column": 3
            },
            {
                "name": "Self-Organization",
                "uniques": [
                    "[+15]% [Production] [in all cities]"
                ],
                "requires": ["Mutual Aid"],
                "row": 3,
                "column": 3
            },
            {
                "name": "Voluntarism Complete",
                "uniques": [
                    "[+3 Production, +3 Food] per [2] population [in all cities]"
                ]
            }
        ]
    }
]
