``` md-bundle-minify.js

var importModuleByKey = [

  {
    object: jsonion_db,
   '{keyPath}': [ '{includeFilePath}' ]
  },

]

```


```json integrated.json
{
  "__description": "Register of built-in Types and their synonyms and expression sequences (right-hand)",
  "__types": ["Type", "Synonym", "Abbreviation", "Reference", "Operator"],
  "__apply": ["/\s/", "__strDecode"],
  
  "P <= TangibleProcess": {

    "Abbreviation": ["Abbrev", "Abbr"],
    "Aggregation": "null",

    "Create": "null",
      "Read": "null",
    "Update": "null",
    "Delete": "null",
    "Select": ["Filter", "Pick"],
      "Join": ["Merge"],
    "Insert": "null",

    "Difference": ["Diff", "~", "%0% ~~ %1%", "~=", "~=="],
    "Patch": ["%0% (%1%)-> %2%", "%0% -(%1%)> %2%"],
    
    "Stem": "Stem %0% -> %1%",
    
    "functionIndexKeyStore": "[%0%](https://wikipedia.org/en/%1%)",
    "Initialization": "Init",
    "Input": "I",
    "Output": "O",
    "PointOfValidation": ["API", "Mirror", "Package", "Module", "Component", "Function"],
    
    "Index": ["toIndex", "i"],

    "MapTo": ["Remap", "Map", "%0% -> %1%"],
    "Reference": ["Ref", "\"%0%\" => \"%1%\"", "\'%0%\' => \'%1%\'"],

    "Pending": "null",

    "Query": "null",
    "Mutate": "null",

    "StringVariable": ["\{Var\}", "{%}", "{{%}}", "${%}"],

    "Trie": ["%0% { %1%"],

    "Validation": "null"
  },

  "__caseInsensitive": {
    "jsonion": "null",
    "md": ["Markdown", "CommonMark"],
    "regex": ["RegExp", "/%/"],
    "v32svgn": "null",
    "validation": ["valida.jsonion", "valida", "validate"],
  },

  "__footing": [
    "including String and Numeric types, as commonly redefined in schema validation"
  ],
  "__syntax": "JavaScript ES6"
}

```


```js manifest-gestrz.js
//
//  //  //
// /*

 # jsonion stem ( data collections × augmentations )

 … A package to explain and resolve database operations & actions with. Written on a mission to produce a readable DB manifest file ...

[a x b] /\/


import { onionStem } from './db-augment/'  // db.a
import { evaluateArgs, Abbr } from 'jsonion/util'

import bindActionTpl from 'jsonion/actionPreset'
    // Assign resolving functions to data state */


var Resolver = function( args = {}, dataRoot = onionStem ){

  var err, inputSchema = {  // Type validation
    augment: [ 'array' ], actions: [ 'array' ]
  },
  Abbreviate: [
  " a => A, m => M, z => Z ", // … list head, foot & mixins
  " augment => augm ",
  " actions => actn ",
  " relational => rel "
  ];

  return ( err = evaluateArgs( inputSchema, args ))
 ? inputSchema 
 : Abbr({
    
    augment: list( args.augment, dataRoot ),
    actions: list( args.actions, Pckg, Offline, ...y ),
    relational: ` #id, #node_id, #table_id `

  }, Abbreviate /* Up to speed */ )
}      // ˇ \\

```


```jsonion.tx2gql schema.txt


      //    //    //    // Beware

     //   _.* => 1|.*  // Mashup

    //   __  => _     // Partials

   //    //    //    // Consideration


export default const collections = () => {
   var collection = {}

/*

 # Gesture-Reflection module definitions
   with jsonion
*/


/*

## Needs
 - Tree structure of definitions, rooted in basic needs 
 ( in overlapping with "wishes", "urges", "desires", "demands" )

   */

collection.need = {}


/*

## Resorces
 - Tree structure of resource definitions

   */

collection.resource = {}
collection.resource_type = {}
collection.resource_unit = {}


collections.resource = { // Link up above collections
  'schema': {
    resource_type: ['./link-to/schema.json#internalRef', Rec.rel],
    resource_unit: ['./link-to/simplSchema.js#exportedVar', Rec.rel]
  },

  ...collection.resource, // <- repeat main resource

// # Add related data structures:
  ...collection.resource_unit,
  ...collection.resource_type

}




/*

## Gestures
 - Symbols of patterns, emerging from recurring (inter)actions and behaviours

   */

collection.gesture = { // Templates, personalized to a specific occasion
}



/*

## Leaps
 - A gesture becomes a leap when habits change
 
   Q: When does a 'leap' fit in node_stem, as a 'milestone' or a 'pointer' in content evolution flow?

   */



/*

 # Collection: Values
 - Words which are meaningful upon truthfully reflecting shared, interpersonal experiences

   */

collection.value = { // Tree structure of value keywords
}

collection.value_observable = { // Metrics for measuring a certain effort / impact, tied to values
};                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          


collections.value_model_contract = {} /* Defined contracts
  
  # For example:

  - when a condition is met, words used by a given person / entity are ...
    replaced with a predefined correction
    or open for editing anew

*/




/*

  # Collections: What we need, what we can offer, what we value (appreciate)

*/

collections.agency_need = { 
// List of needs (all-time ; recurring higher)
// ... described in text or with tags (referenced by ID)
}
collections.agency_resource = { // Pool of disclosed resources
// Governed by entities (a group of people & circles) with defined agency
}; 
collections.agency_value = { // Values we care of (enacted and appreciated), narrowing in on preferred ways of doing
}; 
                                      
 

/*

  # Collection: Gestures
  - Desired scenarios - descriptions of recurring patterns (activities and flowing resources)

*/

collections.agency_gesture = {}
collections.agency_gesture_resource = { // Typical / average flow of resources
}
collections.agency_gesture_transaction = { // Contains a set of transactions 
};



/*

  # Collection: Transactions
  - Occurence of a gesture or its variant - a transaction
  - Flow of ... among giving and receiving entities (meta data about an act of sharing)

*/

collections.agency_transaction = {}

// Resources and energies, which flowed while sharing
collections.agency_transaction_resource = {}

// Needs, fulfilled with this gesture
collections.agency_transaction_need = {}

// Reflected, enacted values (describing intangibles)
collections.agency_transaction_value = {}


# Resource
jsonion { path } / Resource

 - name
 - type
 - description
 - energy
 - matter
 - unfinished

…/	Resource_Component
	- resource_id
 - referenced_resource_id



## Media resource
jsonion { path } / Media



## Gesture
jsonion { path } / Gesture-s

 - title
 - description
 - time
 - location
 ( create, publish, update | close, archive, unlist, delete )

…/ { Stem }(Gesture)

  …/ From
  	- gesture_id
  	- entity_id 
   ( submit | confirm | close, delete )

  …/	To
   - gesture_id
	  - entity_id
   - confirmed
  	- confirmed_time

  …/ Resource
  	- resource_id



## Leap
{ path } / Leap-s

 - title
 - description
 - time_added
( add, update )

…/ Gesture
 - title
 - description



## Reflection
{ path } / Reflection-s

 - subject
 - story
 - time

…/ Value
	- reflection_id
 - entity_id
 - value_id
 - color_hex

…/ Context
	- reflection_id
	- value_id
	- entity_id
	- context_id

…/ Leap
		- reflection_id
		- entity_id
		- value_id
		- relative_value_id
		- ratio

…/ Involved
	- reflection_id
	- entity_id
 - confirmed

…/ Trusted
 - reflection_id
 - entity_id
	- trusted

```


```js Facebook.jsonion
{
'.{propertyName} #': { // … looking for Facebook 'status_updates'
	 This: "post",
__allOf: [], // … is this the dataset we're looking for?
__oneOf: [],
	 map: ['timestamp', 'full_name', 'action', 'post', 'event_name', 'place_name'],

 '.title': {
    Remove: true, // … task executed after jsIons react, while finally mapping to JSON tree

		 // jsIons transform data state (where RegExp condition !false)
	  '/(.*) shared an event./': { 
	     As: ['full_name'],
	    'post.action': 'event_shared'
 	  },
 	 '/(.*) was attending (.*) at (.*)./': {
	     As: ['full_name', 'event_name', 'place_name'],
	    'post.action': 'event_attending'
	   }
  }
},
/*

Like dissoluted ions... The encoded parsing rules enter and react with substances kept in a medium's data structure; so to harness and map modified contents into a resulting JSON data tree.

*/
}

```

## 'V32SVGn' … instead of multiple HTML documents in another wrap

One can't simply spur up a coherent archive (made of distinctive components), when bodies which consist of the same matter will smudge in a deep dish -- lasagna will remain a lasagna; and so would topics contained on embedded websites' pages submerge the wrapping HTML body... But surely we would want to smile in gratitude (that's right, to a forgotten chef who forced an all-around vegan rule to all of the courses).


## Shorthand syntax of 'jsonion'

A shorthand syntax to modify with a JSON dataset structure. A meaningful tool to learn with how to work around parsing processes.


```js
/*


## Resolving unique paths among a variety of data types
   ie. ".status_updates # => fbPosts"


 ` . ` List item identifier: precedes an encoded string (of defined types)


 ` # ` List item(s), identified by a designated index key

   - Consequent list item number (index for efficiency)
   - Contained key value -- easily matched
   ( eg. hashtag, encoded timestamp, identifier key value, namespace key value )


 ` => ` Remap directive (clone data, or create an alias)

   A mapping key (literal) could make available the type of items, nested in an array, in a schematized database collection.


 ` {{ L.function }}: {{ R.3 }} ` Key-value variable template (a special case)

   - Right-hand variable contains a string, number, a function or an object (possibly an internal reference)
   - Left key handle will accept any one of the above types; restrictions and/or transformations will apply in case of a returned object with an exceeding depth



   "… on …"[ion]  ·  [on]"… in …"([o])  ·  [on]"… io …"[n]
    # jsOnIon, jsOnion, jsonIon, JSonIon, JSONIon, SONion
   // /  //   //   //   */

             /* 
            / `\
           ´    ``
     Sort      
   of                peeling
  a                      loop …
     
   \           
    `         .          /
              #         ´



A teal fringe roof, in shade a car,
all's black and ... receives a note

Aloof from frowning winds,
nothing's what it seems

In a passage full of dreams,
entire reef fleets open drinks


  */
```

I'm here to help you. Goodbye
