## Expose variable names as defined in scripts (in console)
Explicit notations on script startup … in-browser console ; server console

```js onion [tags, listed]

import lib, { TrieType } from jsonion

var etc = new TrieType({

	sun { flower { oil 		: { 0: $ }}},
	flax { seed { s 		: { 0: $ }}},
	olive { oil 			: { 0: $ }},
	linseed					: { 0: $ },
	lentils					: { 0: $ },
	buckwheat { flour		: { 0: $ },
	wheatflour				: { 0: $ },
	chickpeas				: { 0: $ },


}, lib.flags.i)

lib.toConsole(...etc)

```

--- ---———

```jsonion                 /* … document-wide */

                                       /* ´´´
                                       ´´´ */
     //           bbvb.             
 */// A vagrant representation jizzlock  //
    //                                  //     


  /*
*/ jsonion_db = {  // … into the cross-origins
 //

  _: {  /*   Operations RAM   */ },
  i: { /* Index of key paths */ 0: {}, 1: {} },
  ctx: {}, ctxProxy: {}, db: {}, dbProxy: {},

  init(hydrate){
    hydrate.forEach( (mapKey, object) => {} )
  }
},

/* ´´´  "Augmented Data, GraphQL & React/Redux"
´´´ */ 
    route = (objTrie, action, params, resolver) 
  => { return resolver( action, params, obTrie )
},

```

```js types.agents.js

export const agentTypes = {
 user: {}
 entity: {}
}

```

```js db.users.js
/*

 # Package: 'jsonion-users'
 - Augments any database of users, thus keeping track of user records across multiple services
 - Pseudonyms in users' credentials are expected to mask real identity; thus decryption key subparts are shared as a secret knot (= DB rel.) tying in public accounts (to reveal with certainty at a later point in own name & by assembling private key from multiple parties)

 */

import { 
  Integer, String, HashId, Timestamp,
  Names, Email, PostAddress
} from './Types/'

import { index, relation AS rel } from './Types/db'
import { eventSource } from './db.eventsource'
import { language } from './db.languages'
import { Actions } from './actions'

export const user = { users: index.collection`

#{{id}} #{{userId}} #{{firstName}} #{{surname}} ##{{pseudonym}} ##{{email}}

`, // … Index of users' data will contain first-tier and second-tier values only upon a query is delivered.

 
__oneOf: [
  id: { type: Integer, ...unique },
  userId: { type: HashId, ...unique },
],

 pseudonym: { type: String, synonym: ['username', 'account handle'] },

__contacts: { _: {
  firstName: [Names, 2],
  surname: [Names],
  email: [Email],
  address: [PostAddress]
 }, synonyms: ['contact details', 'personal info', 'whereabouts'] 
},

 languages: { _: language, ...rel.id },
 
 // … should create an Iterator
 ...[Actions({ autoValue: "{{ TIMESTAMP_NOW }}" }, 'create', 'edit', 'close', 'remove', [Timestamp])],
 ...[Actions('delete', { callback: eventSource })]
}

```

```js db.circle.js

import jsonion from './...' // … 

// Circles -- groups of people with common interest

jsonion.circle = {

// List of users and circles
   member: ["user", "commoner"], 
   languages: {}
// … which members of a group use to communicate with -- with insights mapped, possibly to a GraphQL/React templates (from aggregate metrics and statistical indexes and derived coefficients)

}

//
/* Entity -- a circle of people who delegate agency
 … to actors on a role to enact common visions, with peers
*/

jsonion.entity = {
  // Raising awareness of own conduct ... undefined
}

```

```js actionPreset.js
//  //  //  //  /*

              import actions__en from './actionDict'
     import { redux, json, sql } from './render.actions'
  import { standalone, jsonion } from './render.augmentations'
        import { d_b, parseActions, std } from 'jsonion'

    /\/
   // \
  // ...

 ##  Map actions to data schema

/\/ export default preset; */
    var { caseInsensitive, partialMatch, optional } = std

//  //  //  //  //  //  //  //

var preset = (source = {app:{}, pckg:{}, api:{}, offline:{}}, tpl = {   

  '{0}': [ 'collection', 'object', 'table', caseInsensitive ],
'{key}': { '{0}':{'Name': $}, partialMatch.left },

﻿__augment: [
    standalone`{augmentation}`, // … 
    jsonion.embed`{ keyPath }.{ augmentation }`,
    jsonion.sql.embed`{ tablePath }_{ augmentation }`
  ],
  id: [ 'id', 'Id', jsonion`{key}Id`,
    sql`{key}_id`, jsonion`{key} # .[Ii]d`,
    jsonion`{key}.[Ii]d`, '...relation' ]
  relation: { __match:{__index:{ __gte: 1 }}},
  user:[ 
    json`{enacted}By`, sql`{enacted}_by` 
  ],
  entity: [
    json`{enacted}As`, sql`{enacted}_as` 
  ],
  agentType: [
    json`{enacting}{AgentType}`,  sql`{enacting}_{agentType}`, 
    json`{enacted}By{AgentType}`, sql`{enacted}_by_{agentType}`, 
  ],
  timestamp: [ {'/[Tt]/':{ime:{stamp:$}}}, json`{action}At`,
    json`{enacted}At`, json`{key}Time`, json`{action}Time`
    sql`{key}_time`, sql`{action}_time`, sql`time_{enacted}`,
    sql`{action}_at`, sql`{enacted}_at` ],
__try: { timestamp: [ '/.*[Dd]ate.*/', /.*[Tt]ime.*/ ] },
__call: [ redux.allCaps`{action}_{tablePath}` ],
     // {type}: [ custom definitions ] … #{shortKey} sort, filter 

}, // /\
  /*..*/    dictionaryTrie = actions__en    //
)   =>   {
 
  var actionList = {
    template: tpl,
    language: dictionary.languageCode['ISO 639-1'],
    dictionary: dictionaryTrie, // Unload memory while parsing ...
    ...source
  }

  //
 //  Compile and merge with "jsonion" database process
// ( a prepocessing method, reusable at runtime )

  var merge = function (

//  Main input: calculate "difference" and "merge"
      actionSource, dictionaryTrie, tpl,

//  Main object to merge into
      actionList,

//  Multilingual Trie suffix parser
      resolveSuffix = resolveSuffix__en,

//  Core process handle (optionally)
      ctxKey = null, // accessKey = {} // … if needed, besides

  ){
    
    var { map, index, diff } = 
      parseActions( actionList, resolveSuffix ){

    return d_b.coreProcessMerge( ctxKey, {
     'key': map,
     'key.tpl': d_b.tpl,
     '__index': { 'key': index }
    })
  },

  actionList.__merge = merge;

  return actionList 
}


  //
 // \
/* ...parsingFunction procedure
  ( a multilingual feature )

   ```verb-tense // … what's expected in outcome array

  1 infinitive
  2 past simple

 >> …  await resolveSuffix <<
     ( language dependent )

  3 present-continuous

   ``` => {1}: [ ()=>{}, {3}, >> ... << , {2} ]

*/  function resolveSuffix__en( wordList ){

}
```

```js db.stem.js
/* 

 # Schema of a recent data state block
 … a uniform way of accessing a data node's context through time

 - JSON objects, consistent across data sources & store implementations (in-memory Key-Value stores & message queues, NoSQL databases)

 - Compatibility with SQL is planned as an effort for efficiency: sliced views for serving a variety of aspects; relational data model is aligned with indexing; generating tables for augmented collections at peak demand

*/

import { Text, Integer } from './Types/'
import { 
  validationSchema, withHolochain, withEthereum 
} from './db.valida.js'
import { Actions } from './actions'	// … mirroring a part of data node -- 'eventsWithState' (to generate fields) || 'events'

/* 

   A list of actions that write and modify state of data (node's context)... Rules of access to data are defined in scope of application? 

*/
// To-do: Translate schema into JSON schema type (March - May, 2017)

var nodeStem = {

 id: { type: String, unique: true }, // Data node ID; Unique for each data node?

 ...augment('sql', 'json').({
  key: "no
 }),

 // Current branch (multiple content versions and translations may be contained)
 branch_id: Integer,
 branch_timestamp: Integer,

 // Current published state
 state_id: Integer,  
 state_timestamp: Integer,

 ...actions('create', 'update', 'publish'),
 ...actions('close', 'remove'),
 ...actions('unpublish', 'delete'),

 ...validators().on(Holochain, Twitter)

}

/* 	
	Type 'rhizome': data node's state of mapped relations within plurality of co-evolving contents
*/
/*
import {rhizome_related_node, rhizome_by_type,
		contained_relation_types, agent_relation_types, external_relation_types,
		translate_request} from 'schema';
*/
// Type 'multilingual': enables storing content in multiple languages, by adding translations to rhizome

// import {state, state_translate_request} from 'schema';
// import {draft, draft_translate_request} from 'schema';

```

```js db.review.js

// Type 'reflections': enables commenting contents, giving ability to attach reflected realities during evolving

const reflection = { // Modelling augmentation in early 2017

	sql: { 
		node_id: String,
		branch_id: Integer
	},
	
	state_id: Integer,
	
	eventsWithFields: [actions.platform.create, actions.platform.remove, actions.platform.mutate],

	events: [actions.platform.delete]
};

// Type 'references': enables referencing contents (attachments)

const reference = {

	sql: { 
		node_id: String,
		branch_id: Integer
	},
	
	state_id: Integer,
		  
	pointer_field: String,
	pointer_fulltext: Integer,

	eventsWithFields: [actions.platform.create, actions.platform.remove],

	events: [actions.platform.delete]
};

// Type 'reports': enables reporting inappropriate contents, falsifying invalid data - both in accord with specific circles

const report = {

	eventsWithFields: [actions.platform.create, actions.platform.resolve, actions.platform.close, actions.platform.remove],

	events: [actions.platform.delete]
};

// with any augmented collection (why just so)
// parse pointers to data
// parse markup syntax

```

```js db.eventsource.js

// Stems: {coll} / eventSource
//
// An event occurs one too many times ...
// 

var augment, inputSchema, matchSchema = {}

stem = {
  name: 'eventSource',
}

matchSchema.type = {
 __unique: true,
 __oneOf: [
  'node_id', 'event_id'
 ]
}

var inputSchema = {

__standalone: {
    _: 'string',
    match: ['object', 'ASC']
  },

    collection: 'string',
    timestamp: [ Integer, 11 ],
//  augmented: ['string', 'array'],
    action:    ['string', 'array'],
    user_id:   [ Integer, 'string' ],
    entity_id: [ Integer, 'string' ],

  __checksum: {
      md5: {},
      sha256: {
       '{{ chainType }}': '{{ hash }}'
      },
    },
  __defaultKeys: ['sha256']
}

// findNamespace: ''

```

```js db.augment.js

/*

 # Logic of `jsonion` database schema definitions
 … harvesting the granularity of SQL data relations model (enabling further indexing and refactoring)

 */// Should export possible actions, relevant to what and when (in cosequence)


var initDB // on first load (window || node.js) ; else

var createCollection // write schema to LocalStorage, .json file (export schema; store file), SQL

var indexRelation // Trie type index, SQL add index key

var find, filter // select

```

```js schema.primitives.js

Import { String, Array, Text, Integer as Int } from "./stdTypes"
Export { fieldDiff, fieldDiffList, fieldValue }

const fieldDiff = { // Difference since previous state
  field: String,
  diff: String, 
  n: Int // Steps of change, where applicable
};

const fieldDiffList = { // List of modifications
  field: String,
  diffList: [
    { diff: String, levensthein: Int }
  ]
};

const fieldValue = { // Field and value schema (SQL naming)
  field: String,
  value: [Int, Float, String, Text]
};
```

```js text2json/layout/OrderedList

// Working on parsing in 2019

documentParsingFlow = [
 'receiveContext',  // … dataset's ctx (automated)
 'receivePropsFrom', // … properties & attributes
	'receiveObjectsFrom', // … merge in or transform
 'createArrayOfObjects',
   'objectsRecreateByDelimiters',
  	'js',
	 	'id__createTemporaryId', '*__temporary',
	  '*',
 'toContext', // … automated
 'toDatabaseTasks',
 'pending'
],

abbreviate = function( array, abbrTrie = {}, abbr = {} ){
   array.forEach( (str) => {
     abbrTrie = intoTrie( str, abbrTrie )
     abbr[( getLeafPath( str, abbrTrie ))] = str
   }
 },
 
var { createArrayOfObjects, receiveObjectsFromParser, objectsRecreateByDelimiters, receivePropsFromParser, addToContext, js, id__createTemporaryId, __temporary, __notLast, toContext, toDatabasetasks, pending } 
= abbreviate( documentParsingFlow )

const parsingProcess = {

 serviceStart: [
  'initCoreRunner',
  'registerStdTypes', // … to escape he oblivion

  'getParserList',
  'fnIndex__Wikipedia', // … reusable components
 ],

 initSequence: [
  'receiveProps',   // keyPath, parserList, 
  'receiveObjects', // ctxAdapter or dbAdapter, …
  'parseConfig',
  'parseRemappingSchema',
  'parsePath',
  'initParsers',
 ],

 initParsers: [ // … invoking sequences for expressions & layout blocks (complex encoding & text)
  'receiveProps',
  'initBlocks',
  'initKeywords',
  'initExpressions',
  'intoTrie', // expressionFn to tokenize with
 ],

 parseDirectory: [
  'findConfig',
  'updateContext',
  'parseFiles',
  'setDatabaseTasks',
  'setPending'
 ],


 // Processing information in normalized datasets
 parseCollection: [ // … JSON database output, SVG, RDF
  'sourceParamsToContext',
  'parseDoc'
 ],

 parseFile: [ // … not expecting XML and JS markup
  'parseDoc',
  'filenameToContext',
  'parseContext'
 ],

 parseDoc: documentParsingFlow,

 // Ad-hoc instructions from expressionFn in Trie
	invokeSeq: [
		'intoTrie',
 ],
 
// There's a little more to it, though.
 
```

```js OrderedList.js

import React from 'react'
import _ from 'lodash'

import { // Logical operators — now building a necessary set (with usecases)
	Scenario, MatchOneOf as OneOf, 
	ExpressionChain as Chain, Trie,
	ExpressionNativeJS as Expr,
	Scoop } from '../logic'

import { Line as NL, Headline as H, Paragraph as P } from './' // Layout blocks

import { escapeExpression as e } from '../util' // function unexistent here yet [!!!]

/*
const exampleContent: "

	# Überschrift (aha!)

	Here is etwas
	1. Erste
	2. Zweite
	3. …

"
*/


export default function orderedList (props) {

	//
	// Content blocks in which this expression can appear
	//(even when not explicitly declared)
	//
	
	this.compatible = { 
		in: { // Needless to declare: "Document.*"
			text2json: ["Section", "Paragraph"],
			parserName: [""],
			parserName_2: [""]
		},
		contains: {
			parserName: ["Expressions", "Blocks"]
		},
		with: { // Both wrapped "in" or "contains"
			parserName: ["Expr", "Block"]
		},
		not: {
			parserName: ["Expr", "Block"]
		}
	}
	// … Is extensible (before considering fnIndex__Wikipedia)
	if(_.isObject(props.in))
		compatible.in = _.merge(compatible.in, props.in)


	this.symbols = {}


	this.NumberedItem = {
		expr: "numberedItem",
		compatible: {
			in: { ...compatible },
			contains: { ...compatible },
			ruleOut: { ...compatible }
		},
		symbols: {
			opening: {
				"[0-9]+\.\s": ["md", "text2json"],
				"[0-9]+\s{0,1}\)\s+": ["text2json"],
				"[0-9]+\s+": ["text2json"]
			}
		},
		match: (input, el, db) => {


			// Does the previous list item somehow share the same block?
			//
			// Conditions must be met (descending by priority — higher priority first):
			// — at least two items with an ascending order of numbers exist at same indentation
			// — no elements with a lower depth from tree root exist in between two items
			//	(ie.: left in tree ~ with a smaller indentation)
			var previousListItem


			// 1) run a query (when expression doesn't issue temporary tokens)
			previousListItem = db
				.get('tokens')
				.queryTx({	// … 
					expr: el.expr,
					parser: null,
					with: compatible,
					// When retrieving token data …
					ref: 123,				// — shares one of the same containers
					treeDepth_current: 123, // — is on the same level as previous token
					treeDepth_search: 3,		// — will traverse tree of tokens N levels
					// Sorting results
					sort: "desc",
					limit: 1,
					recent: 1 // shorthand for the above two parameters
				})
				.value()

			// 2) or check cache (when expression)
			previousListItem = db
				.get('tokens.cache')
				.find({ expr: el.expr, blocks: '!!!' }) // … matching IDs
				.recent(1)
				.value()


			end = (previousListItem) ? previousListItem.index : 1
			for (i = input.first ; i <= end ; i++){

				if( matchingExpression ){

					end++

					db.get('parser.runtime').setBufferLen(this.expr) // [!!!] Pass expression/block token ID
				}
			}

			db.get('parser.runtime').resetBufferLen(this.expr) // [!!!] Pass expression/block token ID


			return { i }

		},
		trie: {  }
	}
	// … Is extensible
	if(_.isObject(props.NumberedItem.symbols))
		NumberedItem.symbols = extendSymbols(NumberedItem.symbols, props.symbols)


	return (

		<OrderedList componentLang="en">

			<Scoop>

				<H />
				<P />

				<OneOf resolve="auto">
					<Scenario>
						<Expr with="{this.NumberedItem}">
							{children}
{ /*

	Expressions which are repeated should	not overload the 
	Trie parser structure	with recurrence. Rather, they should be	
	separately listed in a non-parsable category.

								<Scenario>
									{children}
								</Scenario>
								<Scenario>
									{children}
								</Scenario>
*/ }
						</Expr>
					</Scenario>

					<Scenario>
						<Expr with="{this.AlphabeticalItem}">
							{children}
						</Expr>
					</Scenario>
				</OneOf>

			</Scoop>

		</OrderedList>
	)
}

```

```js fn.expressions.js

export {
  exprWrap, extendGen,
  generateTokenId

  // stdExpr, noSuffix, withSuffix (some RegExp types)
}

// Understand expressions, deterministic first off (NSFW)?
/*

## Expression function wrapper validates "arguments" and resolves subtypes

*/  //  //  //

const exprWrap = ( exprFn, argList = [
 /* Sets of arguments: runtime, subtype (& internal) */
] ) => {


	 var wrap = { /* … will await a call in memory */ },
  inputSchema = null, err = null

  if ( !argList.length ){ // Check to save some memory
    var { 
     invokeSeq, inputSchema, configInternal 
    } = exprFn() // … an introductory greeting call
  }


  //
  // Expression validation layer

  const runValid = function( 
   fn = exprFn, argList = argList, schema = inputSchema 
  ){

    if( !schema )
      var inputSchema = exprFn('inputSchema')

    // Check inputs
    return ( err = evaluateArgs(inputSchema, argList) )
    ? fn( argList ) 
    : err
  }


  //
  // Wrapping up ...
  //

  wrap = (runtimeArgs = null, subtypeArgs = null) => {

    var argList = ( runtimeArgs || subtypeArgs ) 
      ? mergeArrays( runtimeArgs, subtypeArgs)
      : null

    if ( !inputSchema )
      var inputSchema = exprFn('inputSchema')

    return runValid( exprFn, argList, schema ) };


  wrap.defineType = ( typeName, typeArgs ) => {

    if ( !inputSchema )
      var { 
       invokeSeq, inputSchema, configInternal 
      } = exprFn({ 'greetWith': argList })

    var wrapType = function( runtimeArgs = null ){
    
      var argList = ( runtimeArgs )
        ? mergeArrays( runtimeArgs, typeArgs )
        : typeArgs

      return runValid( exprFn, argList, inputSchema )
    }

    wrapType.config = configInternal,
    wrapType.invokeSeq = invokeSeq

    return wrapType
  }

  //
  // … Any differences here and there?
  // ( .config and .invokeSeq )
  //

  if (inputSchema) {
    wrap.config = configInternal
    wrap.invokeSeq = invokeSeq
  }


  return wrap;
} // … consider storing within wraps the "db.tokens" references, and greeting's object's "checksum" values (for comparison)


//
// # Invoking a variety of types by arguments
// … storing and accessing subtypes of one expression
//
// ie. expressionType(), expression Type["subtype"]
//

```

```js fn.index.js

__indexParams = { // …
  lastInsert: ['{t}', '{i}'],
  trie: {
 /*  Optimized fast-access index
   … a derivate of query patterns (of frequent and relevant steps in loop) */
  },
 '{sortedBy}': {  // … inMemory cache (once)
    store: { data: false, captions: false, refs: true },
    count: '{n}',

    totalRanges: {
     0: ['{a_}', '{b_}', '{a__utf8}', '{z__utf8}']
    },
    rangeByKeyIndex: {
     0: [
        [ '{a_}', '{b_}', '{a__utf8}', '{b__utf8}', '{i}', '{n}', '{indexObj__next}', '{indexObj__prev}' ] ],
    ],

    expireAfter: -1,
    insertedKeys: [    // … unprocessed inserted row numbers
      { t: null, i: null, key: null },
    ],
    stepPolynomial: [  // … keyword density at traversed areas
      { '{routeMatch}': ['{a__utf8}', '{b__utf8}', '{i}', '{n}',
        '{lastQueryAt}', '{queryFrequency}', '{avgMatchRatio}'] },
    ],
    lastQueryAt: '{timestamp}',
  },
  priority: { highest: 1, lowest: 4, 
    deprioritizeUntil: 2, offloadAt: 3
  },
  methodsWikipedia: { '{functionPath}': '{Wikipedia__URL}' },
},


indexLoops = function( onionPath, // 

  sortedBy = {
  '{timestamp.update}': 'DESC'
  },
  rangeParams = {
    offset: 0, limit: 30,
  '{timestamp.update}': { a_: 0, b_: char(2^64) }
  },

  returnType = {
    data: false,
    captions: false,
    ref: true
  },
  persistentIndex = {
    expire: 7*24*3600,
    priority: { high: 1, low: 4, offload: 3 },
    maxLen: 5000,
    minLen: 1000
  }

){

  var next = ( typeof onionPath.next === 'object' )
              ? onionPath.next : null
/*
  [
    {indexObj}, {i}, {order},
    {offset}, {limit},
    {returnType__obj},

    {sortingKey}, ({rangeParams__obj}), {order}, … ;

    {keyPath}, {persistentIndex_expire},
    {priority_a}, {priority_b}
  ]
 */
```

```jsonion.tx2gql schema.txt


      //    //    //    // Beware

     //   _.* => 1|.*  // Mashup

    //   __  => _     // Partials

   //    //    //    // Consideration


export default const collections = () => {
   var collection = {}

//
// ////    //*
 # Gesture-Reflection module definitions
//     /// with jsonion x ( node-rhizome )
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

```json ion

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

```gql d_b.stem.gql

query viewDataRoot( findBy: [StemPath], 
__id: Int, __keyPath: String, __blockId: Int ): [RootDataNode]

type RootDataNode { ${cached} ${dataStore} ${JSON} ${XML} } # oneOf

query viewStems( findBy: [StemPath],
 __id: Int, __keyPath: String, __blockId: Int ): [StemAugmented]

type StemAugmented {
 ${stem}
 ${augmentations}
 __included: Annotations, __y: [T]
}

fragment augmentations {
 ${eventSource} ${translateRequest}
 ${event} ${reflections} ${highlights}
 ${leap} ${gesture} ${values}
 ${tree} ${rhizome} ${related}
 ${circles} ${permissions}
 ${mirrors} ${blockchain} ${dht}
}

input StemPath { ${stemPath} }

fragment stemPath {

 # [BranchTag] × [StateActual] × [ChainHash]
   stemId: String

 # Determined main branch stemId (hash)
   main: String

 ${internalPath}
 ${sourceServiceParams}

   language: [LangCode]          # ISO 936-1
   branch: [BranchTag]   # Branch identifiers (alphabetical list)
}

fragment stem { ${stemPath}

 # Branch Head: Current state of data, as published (multilingual)
   state: [StateActual]

 # Audit Trail: Modifications to data node state (History & Draft)
   chain: [StateChain]
}

type Annotations {

 # Complete data nodes
   nodeList: [StemAugmented]   

 # Partial data node views
   captions: [StemCaption]
   rootData: [RootDataNode]  # … unaugmented view

 # Internal references (with 'jsonion')
 __refs:     [StemRel]         

 # Links to external mirrors
   mirror:   [MirrorNode]

 # Links to external services
   linked:   [SourceNode]
}

query nodeChain( languageCode: String, machineTranslation: Boolean,

 # Pagination offset start
   stemId: String,

 # Pagination: Returned items count
   limit: Int, count: Int, next: Int, n: Int, prev: Int,

 # Is there an external source listed?
   source: Boolean, url: Boolean, domain: String,

 # Is there a source of data validation and backup?
   mirror: Boolean
   blockchain: Boolean
   dht: Boolean

   findBy: [StemPath]

): [StateChain]
```

```js integrated.json
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
    
    "Fork": "Fork %0% -> %1%",
    "Stem": "Stem %0% -> %1%",
    
    "functionIndexKeyStore": "[%0%](https://wikipedia.org/en/%1%)",
    "Initialization": "Init",
    "Input": "I",
    "Output": "O",
    "PointOfValidation": ["API", "Mirror", "Package", "Module", "Component", "Function"],
    
    "Index": ["toIndex", "i"],

    "MapTo": ["Remap", "Map", "%0% -> %1%"],
    "Reference": ["Ref", '\"%0%\" => \"%1%\"', "\'%0%\' => \'%1%\'"],

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
