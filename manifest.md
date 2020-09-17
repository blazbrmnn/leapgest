---


---

<h2 id="expose-variable-names-as-defined-in-scripts-in-console">Expose variable names as defined in scripts (in console)</h2>
<p>Explicit notations on script startup … in-browser console ; server console</p>
<pre class=" language-js"><code class="prism  language-js">
<span class="token keyword">import</span> lib<span class="token punctuation">,</span> <span class="token punctuation">{</span> TrieType <span class="token punctuation">}</span> <span class="token keyword">from</span> jsonion

<span class="token keyword">var</span> etc <span class="token operator">=</span> <span class="token keyword">new</span> <span class="token class-name">TrieType</span><span class="token punctuation">(</span><span class="token punctuation">{</span>

	sun <span class="token punctuation">{</span> flower <span class="token punctuation">{</span> oil 		<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">,</span>
	flax <span class="token punctuation">{</span> seed <span class="token punctuation">{</span> s 		<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">,</span>
	olive <span class="token punctuation">{</span> oil 			<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">,</span>
	linseed					<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">,</span>
	lentils					<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">,</span>
	buckwheat <span class="token punctuation">{</span> flour		<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">,</span>
	wheatflour				<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">,</span>
	chickpeas				<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token number">0</span><span class="token punctuation">:</span> $ <span class="token punctuation">}</span><span class="token punctuation">,</span>


<span class="token punctuation">}</span><span class="token punctuation">,</span> lib<span class="token punctuation">.</span>flags<span class="token punctuation">.</span>i<span class="token punctuation">)</span>

lib<span class="token punctuation">.</span><span class="token function">toConsole</span><span class="token punctuation">(</span><span class="token operator">...</span>etc<span class="token punctuation">)</span>

</code></pre>
<p>— ---———</p>
<pre class=" language-jsonion"><code class="prism  language-jsonion">
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
    hydrate.forEach( (mapKey, object) =&gt; {} )
  }
},

/* ´´´  "Augmented Data, GraphQL &amp; React/Redux"
´´´ */ 
    route = (objTrie, action, params, resolver) 
  =&gt; { return resolver( action, params, obTrie )
},

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token keyword">export</span> <span class="token keyword">const</span> agentTypes <span class="token operator">=</span> <span class="token punctuation">{</span>
 user<span class="token punctuation">:</span> <span class="token punctuation">{</span><span class="token punctuation">}</span>
 entity<span class="token punctuation">:</span> <span class="token punctuation">{</span><span class="token punctuation">}</span>
<span class="token punctuation">}</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js"><span class="token comment">/*

 # Package: 'jsonion-users'
 - Augments any database of users, thus keeping track of user records across multiple services
 - Pseudonyms in users' credentials are expected to mask real identity; thus decryption key subparts are shared as a secret knot (= DB rel.) tying in public accounts (to reveal with certainty at a later point in own name &amp; by assembling private key from multiple parties)

 */</span>

<span class="token keyword">import</span> <span class="token punctuation">{</span> 
  Integer<span class="token punctuation">,</span> String<span class="token punctuation">,</span> HashId<span class="token punctuation">,</span> Timestamp<span class="token punctuation">,</span>
  Names<span class="token punctuation">,</span> Email<span class="token punctuation">,</span> PostAddress
<span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./Types/'</span>

<span class="token keyword">import</span> <span class="token punctuation">{</span> index<span class="token punctuation">,</span> relation AS rel <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./Types/db'</span>
<span class="token keyword">import</span> <span class="token punctuation">{</span> eventSource <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./db.eventsource'</span>
<span class="token keyword">import</span> <span class="token punctuation">{</span> language <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./db.languages'</span>
<span class="token keyword">import</span> <span class="token punctuation">{</span> Actions <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./actions'</span>

<span class="token keyword">export</span> <span class="token keyword">const</span> user <span class="token operator">=</span> <span class="token punctuation">{</span> users<span class="token punctuation">:</span> index<span class="token punctuation">.</span>collection<span class="token template-string"><span class="token string">`

#{{id}} #{{userId}} #{{firstName}} #{{surname}} ##{{pseudonym}} ##{{email}}

`</span></span><span class="token punctuation">,</span> <span class="token comment">// … Index of users' data will contain first-tier and second-tier values only upon a query is delivered.</span>

 
__oneOf<span class="token punctuation">:</span> <span class="token punctuation">[</span>
  id<span class="token punctuation">:</span> <span class="token punctuation">{</span> type<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span> <span class="token operator">...</span>unique <span class="token punctuation">}</span><span class="token punctuation">,</span>
  userId<span class="token punctuation">:</span> <span class="token punctuation">{</span> type<span class="token punctuation">:</span> HashId<span class="token punctuation">,</span> <span class="token operator">...</span>unique <span class="token punctuation">}</span><span class="token punctuation">,</span>
<span class="token punctuation">]</span><span class="token punctuation">,</span>

 pseudonym<span class="token punctuation">:</span> <span class="token punctuation">{</span> type<span class="token punctuation">:</span> String<span class="token punctuation">,</span> synonym<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'username'</span><span class="token punctuation">,</span> <span class="token string">'account handle'</span><span class="token punctuation">]</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>

__contacts<span class="token punctuation">:</span> <span class="token punctuation">{</span> _<span class="token punctuation">:</span> <span class="token punctuation">{</span>
  firstName<span class="token punctuation">:</span> <span class="token punctuation">[</span>Names<span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
  surname<span class="token punctuation">:</span> <span class="token punctuation">[</span>Names<span class="token punctuation">]</span><span class="token punctuation">,</span>
  email<span class="token punctuation">:</span> <span class="token punctuation">[</span>Email<span class="token punctuation">]</span><span class="token punctuation">,</span>
  address<span class="token punctuation">:</span> <span class="token punctuation">[</span>PostAddress<span class="token punctuation">]</span>
 <span class="token punctuation">}</span><span class="token punctuation">,</span> synonyms<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'contact details'</span><span class="token punctuation">,</span> <span class="token string">'personal info'</span><span class="token punctuation">,</span> <span class="token string">'whereabouts'</span><span class="token punctuation">]</span> 
<span class="token punctuation">}</span><span class="token punctuation">,</span>

 languages<span class="token punctuation">:</span> <span class="token punctuation">{</span> _<span class="token punctuation">:</span> language<span class="token punctuation">,</span> <span class="token operator">...</span>rel<span class="token punctuation">.</span>id <span class="token punctuation">}</span><span class="token punctuation">,</span>
 
 <span class="token comment">// … should create an Iterator</span>
 <span class="token operator">...</span><span class="token punctuation">[</span><span class="token function">Actions</span><span class="token punctuation">(</span><span class="token punctuation">{</span> autoValue<span class="token punctuation">:</span> <span class="token string">"{{ TIMESTAMP_NOW }}"</span> <span class="token punctuation">}</span><span class="token punctuation">,</span> <span class="token string">'create'</span><span class="token punctuation">,</span> <span class="token string">'edit'</span><span class="token punctuation">,</span> <span class="token string">'close'</span><span class="token punctuation">,</span> <span class="token string">'remove'</span><span class="token punctuation">,</span> <span class="token punctuation">[</span>Timestamp<span class="token punctuation">]</span><span class="token punctuation">)</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
 <span class="token operator">...</span><span class="token punctuation">[</span><span class="token function">Actions</span><span class="token punctuation">(</span><span class="token string">'delete'</span><span class="token punctuation">,</span> <span class="token punctuation">{</span> callback<span class="token punctuation">:</span> eventSource <span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">]</span>
<span class="token punctuation">}</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token keyword">import</span> jsonion <span class="token keyword">from</span> <span class="token string">'./...'</span> <span class="token comment">// … </span>

<span class="token comment">// Circles -- groups of people with common interest</span>

jsonion<span class="token punctuation">.</span>circle <span class="token operator">=</span> <span class="token punctuation">{</span>

<span class="token comment">// List of users and circles</span>
   member<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"user"</span><span class="token punctuation">,</span> <span class="token string">"commoner"</span><span class="token punctuation">]</span><span class="token punctuation">,</span> 
   languages<span class="token punctuation">:</span> <span class="token punctuation">{</span><span class="token punctuation">}</span>
<span class="token comment">// … which members of a group use to communicate with -- with insights mapped, possibly to a GraphQL/React templates (from aggregate metrics and statistical indexes and derived coefficients)</span>

<span class="token punctuation">}</span>

<span class="token comment">//</span>
<span class="token comment">/* Entity -- a circle of people who delegate agency
 … to actors on a role to enact common visions, with peers
*/</span>

jsonion<span class="token punctuation">.</span>entity <span class="token operator">=</span> <span class="token punctuation">{</span>
  <span class="token comment">// Raising awareness of own conduct ... undefined</span>
<span class="token punctuation">}</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js"><span class="token comment">//  //  //  //  </span><span class="token comment">/*

              import actions__en from './actionDict'
     import { redux, json, sql } from './render.actions'
  import { standalone, jsonion } from './render.augmentations'
        import { d_b, parseActions, std } from 'jsonion'

    /\/
   // \
  // ...

 ##  Map actions to data schema

/\/ export default preset; */</span>
    <span class="token keyword">var</span> <span class="token punctuation">{</span> caseInsensitive<span class="token punctuation">,</span> partialMatch<span class="token punctuation">,</span> optional <span class="token punctuation">}</span> <span class="token operator">=</span> std

<span class="token comment">//  //  //  //  //  //  //  //</span>

<span class="token keyword">var</span> preset <span class="token operator">=</span> <span class="token punctuation">(</span>source <span class="token operator">=</span> <span class="token punctuation">{</span>app<span class="token punctuation">:</span><span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">,</span> pckg<span class="token punctuation">:</span><span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">,</span> api<span class="token punctuation">:</span><span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">,</span> offline<span class="token punctuation">:</span><span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">,</span> tpl <span class="token operator">=</span> <span class="token punctuation">{</span>   

  <span class="token string">'{0}'</span><span class="token punctuation">:</span> <span class="token punctuation">[</span> <span class="token string">'collection'</span><span class="token punctuation">,</span> <span class="token string">'object'</span><span class="token punctuation">,</span> <span class="token string">'table'</span><span class="token punctuation">,</span> caseInsensitive <span class="token punctuation">]</span><span class="token punctuation">,</span>
<span class="token string">'{key}'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token string">'{0}'</span><span class="token punctuation">:</span><span class="token punctuation">{</span><span class="token string">'Name'</span><span class="token punctuation">:</span> $<span class="token punctuation">}</span><span class="token punctuation">,</span> partialMatch<span class="token punctuation">.</span>left <span class="token punctuation">}</span><span class="token punctuation">,</span>

﻿__augment<span class="token punctuation">:</span> <span class="token punctuation">[</span>
    standalone<span class="token template-string"><span class="token string">`{augmentation}`</span></span><span class="token punctuation">,</span> <span class="token comment">// … </span>
    jsonion<span class="token punctuation">.</span>embed<span class="token template-string"><span class="token string">`{ keyPath }.{ augmentation }`</span></span><span class="token punctuation">,</span>
    jsonion<span class="token punctuation">.</span>sql<span class="token punctuation">.</span>embed<span class="token template-string"><span class="token string">`{ tablePath }_{ augmentation }`</span></span>
  <span class="token punctuation">]</span><span class="token punctuation">,</span>
  id<span class="token punctuation">:</span> <span class="token punctuation">[</span> <span class="token string">'id'</span><span class="token punctuation">,</span> <span class="token string">'Id'</span><span class="token punctuation">,</span> jsonion<span class="token template-string"><span class="token string">`{key}Id`</span></span><span class="token punctuation">,</span>
    sql<span class="token template-string"><span class="token string">`{key}_id`</span></span><span class="token punctuation">,</span> jsonion<span class="token template-string"><span class="token string">`{key} # .[Ii]d`</span></span><span class="token punctuation">,</span>
    jsonion<span class="token template-string"><span class="token string">`{key}.[Ii]d`</span></span><span class="token punctuation">,</span> <span class="token string">'...relation'</span> <span class="token punctuation">]</span>
  relation<span class="token punctuation">:</span> <span class="token punctuation">{</span> __match<span class="token punctuation">:</span><span class="token punctuation">{</span>__index<span class="token punctuation">:</span><span class="token punctuation">{</span> __gte<span class="token punctuation">:</span> <span class="token number">1</span> <span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">,</span>
  user<span class="token punctuation">:</span><span class="token punctuation">[</span> 
    json<span class="token template-string"><span class="token string">`{enacted}By`</span></span><span class="token punctuation">,</span> sql<span class="token template-string"><span class="token string">`{enacted}_by`</span></span> 
  <span class="token punctuation">]</span><span class="token punctuation">,</span>
  entity<span class="token punctuation">:</span> <span class="token punctuation">[</span>
    json<span class="token template-string"><span class="token string">`{enacted}As`</span></span><span class="token punctuation">,</span> sql<span class="token template-string"><span class="token string">`{enacted}_as`</span></span> 
  <span class="token punctuation">]</span><span class="token punctuation">,</span>
  agentType<span class="token punctuation">:</span> <span class="token punctuation">[</span>
    json<span class="token template-string"><span class="token string">`{enacting}{AgentType}`</span></span><span class="token punctuation">,</span>  sql<span class="token template-string"><span class="token string">`{enacting}_{agentType}`</span></span><span class="token punctuation">,</span> 
    json<span class="token template-string"><span class="token string">`{enacted}By{AgentType}`</span></span><span class="token punctuation">,</span> sql<span class="token template-string"><span class="token string">`{enacted}_by_{agentType}`</span></span><span class="token punctuation">,</span> 
  <span class="token punctuation">]</span><span class="token punctuation">,</span>
  timestamp<span class="token punctuation">:</span> <span class="token punctuation">[</span> <span class="token punctuation">{</span><span class="token string">'/[Tt]/'</span><span class="token punctuation">:</span><span class="token punctuation">{</span>ime<span class="token punctuation">:</span><span class="token punctuation">{</span>stamp<span class="token punctuation">:</span>$<span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">}</span><span class="token punctuation">,</span> json<span class="token template-string"><span class="token string">`{action}At`</span></span><span class="token punctuation">,</span>
    json<span class="token template-string"><span class="token string">`{enacted}At`</span></span><span class="token punctuation">,</span> json<span class="token template-string"><span class="token string">`{key}Time`</span></span><span class="token punctuation">,</span> json<span class="token template-string"><span class="token string">`{action}Time`</span></span>
    sql<span class="token template-string"><span class="token string">`{key}_time`</span></span><span class="token punctuation">,</span> sql<span class="token template-string"><span class="token string">`{action}_time`</span></span><span class="token punctuation">,</span> sql<span class="token template-string"><span class="token string">`time_{enacted}`</span></span><span class="token punctuation">,</span>
    sql<span class="token template-string"><span class="token string">`{action}_at`</span></span><span class="token punctuation">,</span> sql<span class="token template-string"><span class="token string">`{enacted}_at`</span></span> <span class="token punctuation">]</span><span class="token punctuation">,</span>
__try<span class="token punctuation">:</span> <span class="token punctuation">{</span> timestamp<span class="token punctuation">:</span> <span class="token punctuation">[</span> <span class="token string">'/.*[Dd]ate.*/'</span><span class="token punctuation">,</span> <span class="token operator">/</span><span class="token punctuation">.</span><span class="token operator">*</span><span class="token punctuation">[</span>Tt<span class="token punctuation">]</span>ime<span class="token punctuation">.</span><span class="token operator">*</span><span class="token operator">/</span> <span class="token punctuation">]</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>
__call<span class="token punctuation">:</span> <span class="token punctuation">[</span> redux<span class="token punctuation">.</span>allCaps<span class="token template-string"><span class="token string">`{action}_{tablePath}`</span></span> <span class="token punctuation">]</span><span class="token punctuation">,</span>
     <span class="token comment">// {type}: [ custom definitions ] … #{shortKey} sort, filter </span>

<span class="token punctuation">}</span><span class="token punctuation">,</span> <span class="token comment">// /\</span>
  <span class="token comment">/*..*/</span>    dictionaryTrie <span class="token operator">=</span> actions__en    <span class="token comment">//</span>
<span class="token punctuation">)</span>   <span class="token operator">=&gt;</span>   <span class="token punctuation">{</span>
 
  <span class="token keyword">var</span> actionList <span class="token operator">=</span> <span class="token punctuation">{</span>
    template<span class="token punctuation">:</span> tpl<span class="token punctuation">,</span>
    language<span class="token punctuation">:</span> dictionary<span class="token punctuation">.</span>languageCode<span class="token punctuation">[</span><span class="token string">'ISO 639-1'</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    dictionary<span class="token punctuation">:</span> dictionaryTrie<span class="token punctuation">,</span> <span class="token comment">// Unload memory while parsing ...</span>
    <span class="token operator">...</span>source
  <span class="token punctuation">}</span>

  <span class="token comment">//</span>
 <span class="token comment">//  Compile and merge with "jsonion" database process</span>
<span class="token comment">// ( a prepocessing method, reusable at runtime )</span>

  <span class="token keyword">var</span> <span class="token function-variable function">merge</span> <span class="token operator">=</span> <span class="token keyword">function</span> <span class="token punctuation">(</span>

<span class="token comment">//  Main input: calculate "difference" and "merge"</span>
      actionSource<span class="token punctuation">,</span> dictionaryTrie<span class="token punctuation">,</span> tpl<span class="token punctuation">,</span>

<span class="token comment">//  Main object to merge into</span>
      actionList<span class="token punctuation">,</span>

<span class="token comment">//  Multilingual Trie suffix parser</span>
      resolveSuffix <span class="token operator">=</span> resolveSuffix__en<span class="token punctuation">,</span>

<span class="token comment">//  Core process handle (optionally)</span>
      ctxKey <span class="token operator">=</span> <span class="token keyword">null</span><span class="token punctuation">,</span> <span class="token comment">// accessKey = {} // … if needed, besides</span>

  <span class="token punctuation">)</span><span class="token punctuation">{</span>
    
    <span class="token keyword">var</span> <span class="token punctuation">{</span> map<span class="token punctuation">,</span> index<span class="token punctuation">,</span> diff <span class="token punctuation">}</span> <span class="token operator">=</span> 
      <span class="token function">parseActions</span><span class="token punctuation">(</span> actionList<span class="token punctuation">,</span> resolveSuffix <span class="token punctuation">)</span><span class="token punctuation">{</span>

    <span class="token keyword">return</span> d_b<span class="token punctuation">.</span><span class="token function">coreProcessMerge</span><span class="token punctuation">(</span> ctxKey<span class="token punctuation">,</span> <span class="token punctuation">{</span>
     <span class="token string">'key'</span><span class="token punctuation">:</span> map<span class="token punctuation">,</span>
     <span class="token string">'key.tpl'</span><span class="token punctuation">:</span> d_b<span class="token punctuation">.</span>tpl<span class="token punctuation">,</span>
     <span class="token string">'__index'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token string">'key'</span><span class="token punctuation">:</span> index <span class="token punctuation">}</span>
    <span class="token punctuation">}</span><span class="token punctuation">)</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>

  actionList<span class="token punctuation">.</span>__merge <span class="token operator">=</span> merge<span class="token punctuation">;</span>

  <span class="token keyword">return</span> actionList 
<span class="token punctuation">}</span>


  <span class="token comment">//</span>
 <span class="token comment">// \</span>
<span class="token comment">/* ...parsingFunction procedure
  ( a multilingual feature )

   ```verb-tense // … what's expected in outcome array

  1 infinitive
  2 past simple

 &gt;&gt; …  await resolveSuffix &lt;&lt;
     ( language dependent )

  3 present-continuous

   ``` =&gt; {1}: [ ()=&gt;{}, {3}, &gt;&gt; ... &lt;&lt; , {2} ]

*/</span>  <span class="token keyword">function</span> <span class="token function">resolveSuffix__en</span><span class="token punctuation">(</span> wordList <span class="token punctuation">)</span><span class="token punctuation">{</span>

<span class="token punctuation">}</span>
</code></pre>
<pre class=" language-js"><code class="prism  language-js"><span class="token comment">/* 

 # Schema of a recent data state block
 … a uniform way of accessing a data node's context through time

 - JSON objects, consistent across data sources &amp; store implementations (in-memory Key-Value stores &amp; message queues, NoSQL databases)

 - Compatibility with SQL is planned as an effort for efficiency: sliced views for serving a variety of aspects; relational data model is aligned with indexing; generating tables for augmented collections at peak demand

*/</span>

<span class="token keyword">import</span> <span class="token punctuation">{</span> Text<span class="token punctuation">,</span> Integer <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./Types/'</span>
<span class="token keyword">import</span> <span class="token punctuation">{</span> 
  validationSchema<span class="token punctuation">,</span> withHolochain<span class="token punctuation">,</span> withEthereum 
<span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./db.valida.js'</span>
<span class="token keyword">import</span> <span class="token punctuation">{</span> Actions <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./actions'</span>	<span class="token comment">// … mirroring a part of data node -- 'eventsWithState' (to generate fields) || 'events'</span>

<span class="token comment">/* 

   A list of actions that write and modify state of data (node's context)... Rules of access to data are defined in scope of application? 

*/</span>
<span class="token comment">// To-do: Translate schema into JSON schema type (March - May, 2017)</span>

<span class="token keyword">var</span> nodeStem <span class="token operator">=</span> <span class="token punctuation">{</span>

 id<span class="token punctuation">:</span> <span class="token punctuation">{</span> type<span class="token punctuation">:</span> String<span class="token punctuation">,</span> unique<span class="token punctuation">:</span> <span class="token boolean">true</span> <span class="token punctuation">}</span><span class="token punctuation">,</span> <span class="token comment">// Data node ID; Unique for each data node?</span>

 <span class="token operator">...</span><span class="token function">augment</span><span class="token punctuation">(</span><span class="token string">'sql'</span><span class="token punctuation">,</span> <span class="token string">'json'</span><span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token punctuation">(</span><span class="token punctuation">{</span>
  key<span class="token punctuation">:</span> "no
 <span class="token punctuation">}</span><span class="token punctuation">)</span><span class="token punctuation">,</span>

 <span class="token comment">// Current branch (multiple content versions and translations may be contained)</span>
 branch_id<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span>
 branch_timestamp<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span>

 <span class="token comment">// Current published state</span>
 state_id<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span>  
 state_timestamp<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span>

 <span class="token operator">...</span><span class="token function">actions</span><span class="token punctuation">(</span><span class="token string">'create'</span><span class="token punctuation">,</span> <span class="token string">'update'</span><span class="token punctuation">,</span> <span class="token string">'publish'</span><span class="token punctuation">)</span><span class="token punctuation">,</span>
 <span class="token operator">...</span><span class="token function">actions</span><span class="token punctuation">(</span><span class="token string">'close'</span><span class="token punctuation">,</span> <span class="token string">'remove'</span><span class="token punctuation">)</span><span class="token punctuation">,</span>
 <span class="token operator">...</span><span class="token function">actions</span><span class="token punctuation">(</span><span class="token string">'unpublish'</span><span class="token punctuation">,</span> <span class="token string">'delete'</span><span class="token punctuation">)</span><span class="token punctuation">,</span>

 <span class="token operator">...</span><span class="token function">validators</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token function">on</span><span class="token punctuation">(</span>Holochain<span class="token punctuation">,</span> Twitter<span class="token punctuation">)</span>

<span class="token punctuation">}</span>

<span class="token comment">/* 	
	Type 'rhizome': data node's state of mapped relations within plurality of co-evolving contents
*/</span>
<span class="token comment">/*
import {rhizome_related_node, rhizome_by_type,
		contained_relation_types, agent_relation_types, external_relation_types,
		translate_request} from 'schema';
*/</span>
<span class="token comment">// Type 'multilingual': enables storing content in multiple languages, by adding translations to rhizome</span>

<span class="token comment">// import {state, state_translate_request} from 'schema';</span>
<span class="token comment">// import {draft, draft_translate_request} from 'schema';</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token comment">// Type 'reflections': enables commenting contents, giving ability to attach reflected realities during evolving</span>

<span class="token keyword">const</span> reflection <span class="token operator">=</span> <span class="token punctuation">{</span> <span class="token comment">// Modelling augmentation in early 2017</span>

	sql<span class="token punctuation">:</span> <span class="token punctuation">{</span> 
		node_id<span class="token punctuation">:</span> String<span class="token punctuation">,</span>
		branch_id<span class="token punctuation">:</span> Integer
	<span class="token punctuation">}</span><span class="token punctuation">,</span>
	
	state_id<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span>
	
	eventsWithFields<span class="token punctuation">:</span> <span class="token punctuation">[</span>actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>create<span class="token punctuation">,</span> actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>remove<span class="token punctuation">,</span> actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>mutate<span class="token punctuation">]</span><span class="token punctuation">,</span>

	events<span class="token punctuation">:</span> <span class="token punctuation">[</span>actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span><span class="token keyword">delete</span><span class="token punctuation">]</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>

<span class="token comment">// Type 'references': enables referencing contents (attachments)</span>

<span class="token keyword">const</span> reference <span class="token operator">=</span> <span class="token punctuation">{</span>

	sql<span class="token punctuation">:</span> <span class="token punctuation">{</span> 
		node_id<span class="token punctuation">:</span> String<span class="token punctuation">,</span>
		branch_id<span class="token punctuation">:</span> Integer
	<span class="token punctuation">}</span><span class="token punctuation">,</span>
	
	state_id<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span>
		  
	pointer_field<span class="token punctuation">:</span> String<span class="token punctuation">,</span>
	pointer_fulltext<span class="token punctuation">:</span> Integer<span class="token punctuation">,</span>

	eventsWithFields<span class="token punctuation">:</span> <span class="token punctuation">[</span>actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>create<span class="token punctuation">,</span> actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>remove<span class="token punctuation">]</span><span class="token punctuation">,</span>

	events<span class="token punctuation">:</span> <span class="token punctuation">[</span>actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span><span class="token keyword">delete</span><span class="token punctuation">]</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>

<span class="token comment">// Type 'reports': enables reporting inappropriate contents, falsifying invalid data - both in accord with specific circles</span>

<span class="token keyword">const</span> report <span class="token operator">=</span> <span class="token punctuation">{</span>

	eventsWithFields<span class="token punctuation">:</span> <span class="token punctuation">[</span>actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>create<span class="token punctuation">,</span> actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>resolve<span class="token punctuation">,</span> actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>close<span class="token punctuation">,</span> actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span>remove<span class="token punctuation">]</span><span class="token punctuation">,</span>

	events<span class="token punctuation">:</span> <span class="token punctuation">[</span>actions<span class="token punctuation">.</span>platform<span class="token punctuation">.</span><span class="token keyword">delete</span><span class="token punctuation">]</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>

<span class="token comment">// with any augmented collection (why just so)</span>
<span class="token comment">// parse pointers to data</span>
<span class="token comment">// parse markup syntax</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token comment">// Stems: {coll} / eventSource</span>
<span class="token comment">//</span>
<span class="token comment">// An event occurs one too many times ...</span>
<span class="token comment">// </span>

<span class="token keyword">var</span> augment<span class="token punctuation">,</span> inputSchema<span class="token punctuation">,</span> matchSchema <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token punctuation">}</span>

stem <span class="token operator">=</span> <span class="token punctuation">{</span>
  name<span class="token punctuation">:</span> <span class="token string">'eventSource'</span><span class="token punctuation">,</span>
<span class="token punctuation">}</span>

matchSchema<span class="token punctuation">.</span>type <span class="token operator">=</span> <span class="token punctuation">{</span>
 __unique<span class="token punctuation">:</span> <span class="token boolean">true</span><span class="token punctuation">,</span>
 __oneOf<span class="token punctuation">:</span> <span class="token punctuation">[</span>
  <span class="token string">'node_id'</span><span class="token punctuation">,</span> <span class="token string">'event_id'</span>
 <span class="token punctuation">]</span>
<span class="token punctuation">}</span>

<span class="token keyword">var</span> inputSchema <span class="token operator">=</span> <span class="token punctuation">{</span>

__standalone<span class="token punctuation">:</span> <span class="token punctuation">{</span>
    _<span class="token punctuation">:</span> <span class="token string">'string'</span><span class="token punctuation">,</span>
    match<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'object'</span><span class="token punctuation">,</span> <span class="token string">'ASC'</span><span class="token punctuation">]</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>

    collection<span class="token punctuation">:</span> <span class="token string">'string'</span><span class="token punctuation">,</span>
    timestamp<span class="token punctuation">:</span> <span class="token punctuation">[</span> Integer<span class="token punctuation">,</span> <span class="token number">11</span> <span class="token punctuation">]</span><span class="token punctuation">,</span>
<span class="token comment">//  augmented: ['string', 'array'],</span>
    action<span class="token punctuation">:</span>    <span class="token punctuation">[</span><span class="token string">'string'</span><span class="token punctuation">,</span> <span class="token string">'array'</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    user_id<span class="token punctuation">:</span>   <span class="token punctuation">[</span> Integer<span class="token punctuation">,</span> <span class="token string">'string'</span> <span class="token punctuation">]</span><span class="token punctuation">,</span>
    entity_id<span class="token punctuation">:</span> <span class="token punctuation">[</span> Integer<span class="token punctuation">,</span> <span class="token string">'string'</span> <span class="token punctuation">]</span><span class="token punctuation">,</span>

  __checksum<span class="token punctuation">:</span> <span class="token punctuation">{</span>
      md5<span class="token punctuation">:</span> <span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">,</span>
      sha256<span class="token punctuation">:</span> <span class="token punctuation">{</span>
       <span class="token string">'{{ chainType }}'</span><span class="token punctuation">:</span> <span class="token string">'{{ hash }}'</span>
      <span class="token punctuation">}</span><span class="token punctuation">,</span>
    <span class="token punctuation">}</span><span class="token punctuation">,</span>
  __defaultKeys<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'sha256'</span><span class="token punctuation">]</span>
<span class="token punctuation">}</span>

<span class="token comment">// findNamespace: ''</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token comment">/*

 # Logic of `jsonion` database schema definitions
 … harvesting the granularity of SQL data relations model (enabling further indexing and refactoring)

 */</span><span class="token comment">// Should export possible actions, relevant to what and when (in cosequence)</span>


<span class="token keyword">var</span> initDB <span class="token comment">// on first load (window || node.js) ; else</span>

<span class="token keyword">var</span> createCollection <span class="token comment">// write schema to LocalStorage, .json file (export schema; store file), SQL</span>

<span class="token keyword">var</span> indexRelation <span class="token comment">// Trie type index, SQL add index key</span>

<span class="token keyword">var</span> find<span class="token punctuation">,</span> filter <span class="token comment">// select</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
Import <span class="token punctuation">{</span> String<span class="token punctuation">,</span> Array<span class="token punctuation">,</span> Text<span class="token punctuation">,</span> Integer <span class="token keyword">as</span> Int <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">"./stdTypes"</span>
Export <span class="token punctuation">{</span> fieldDiff<span class="token punctuation">,</span> fieldDiffList<span class="token punctuation">,</span> fieldValue <span class="token punctuation">}</span>

<span class="token keyword">const</span> fieldDiff <span class="token operator">=</span> <span class="token punctuation">{</span> <span class="token comment">// Difference since previous state</span>
  field<span class="token punctuation">:</span> String<span class="token punctuation">,</span>
  diff<span class="token punctuation">:</span> String<span class="token punctuation">,</span> 
  n<span class="token punctuation">:</span> Int <span class="token comment">// Steps of change, where applicable</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>

<span class="token keyword">const</span> fieldDiffList <span class="token operator">=</span> <span class="token punctuation">{</span> <span class="token comment">// List of modifications</span>
  field<span class="token punctuation">:</span> String<span class="token punctuation">,</span>
  diffList<span class="token punctuation">:</span> <span class="token punctuation">[</span>
    <span class="token punctuation">{</span> diff<span class="token punctuation">:</span> String<span class="token punctuation">,</span> levensthein<span class="token punctuation">:</span> Int <span class="token punctuation">}</span>
  <span class="token punctuation">]</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>

<span class="token keyword">const</span> fieldValue <span class="token operator">=</span> <span class="token punctuation">{</span> <span class="token comment">// Field and value schema (SQL naming)</span>
  field<span class="token punctuation">:</span> String<span class="token punctuation">,</span>
  value<span class="token punctuation">:</span> <span class="token punctuation">[</span>Int<span class="token punctuation">,</span> Float<span class="token punctuation">,</span> String<span class="token punctuation">,</span> Text<span class="token punctuation">]</span>
<span class="token punctuation">}</span><span class="token punctuation">;</span>
</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token comment">// Working on parsing in 2019</span>

documentParsingFlow <span class="token operator">=</span> <span class="token punctuation">[</span>
 <span class="token string">'receiveContext'</span><span class="token punctuation">,</span>  <span class="token comment">// … dataset's ctx (automated)</span>
 <span class="token string">'receivePropsFrom'</span><span class="token punctuation">,</span> <span class="token comment">// … properties &amp; attributes</span>
	<span class="token string">'receiveObjectsFrom'</span><span class="token punctuation">,</span> <span class="token comment">// … merge in or transform</span>
 <span class="token string">'createArrayOfObjects'</span><span class="token punctuation">,</span>
   <span class="token string">'objectsRecreateByDelimiters'</span><span class="token punctuation">,</span>
  	<span class="token string">'js'</span><span class="token punctuation">,</span>
	 	<span class="token string">'id__createTemporaryId'</span><span class="token punctuation">,</span> <span class="token string">'*__temporary'</span><span class="token punctuation">,</span>
	  <span class="token string">'*'</span><span class="token punctuation">,</span>
 <span class="token string">'toContext'</span><span class="token punctuation">,</span> <span class="token comment">// … automated</span>
 <span class="token string">'toDatabaseTasks'</span><span class="token punctuation">,</span>
 <span class="token string">'pending'</span>
<span class="token punctuation">]</span><span class="token punctuation">,</span>

<span class="token function-variable function">abbreviate</span> <span class="token operator">=</span> <span class="token keyword">function</span><span class="token punctuation">(</span> array<span class="token punctuation">,</span> abbrTrie <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token punctuation">}</span><span class="token punctuation">,</span> abbr <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token punctuation">}</span> <span class="token punctuation">)</span><span class="token punctuation">{</span>
   array<span class="token punctuation">.</span><span class="token function">forEach</span><span class="token punctuation">(</span> <span class="token punctuation">(</span>str<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>
     abbrTrie <span class="token operator">=</span> <span class="token function">intoTrie</span><span class="token punctuation">(</span> str<span class="token punctuation">,</span> abbrTrie <span class="token punctuation">)</span>
     abbr<span class="token punctuation">[</span><span class="token punctuation">(</span> <span class="token function">getLeafPath</span><span class="token punctuation">(</span> str<span class="token punctuation">,</span> abbrTrie <span class="token punctuation">)</span><span class="token punctuation">)</span><span class="token punctuation">]</span> <span class="token operator">=</span> str
   <span class="token punctuation">}</span>
 <span class="token punctuation">}</span><span class="token punctuation">,</span>
 
<span class="token keyword">var</span> <span class="token punctuation">{</span> createArrayOfObjects<span class="token punctuation">,</span> receiveObjectsFromParser<span class="token punctuation">,</span> objectsRecreateByDelimiters<span class="token punctuation">,</span> receivePropsFromParser<span class="token punctuation">,</span> addToContext<span class="token punctuation">,</span> js<span class="token punctuation">,</span> id__createTemporaryId<span class="token punctuation">,</span> __temporary<span class="token punctuation">,</span> __notLast<span class="token punctuation">,</span> toContext<span class="token punctuation">,</span> toDatabasetasks<span class="token punctuation">,</span> pending <span class="token punctuation">}</span> 
<span class="token operator">=</span> <span class="token function">abbreviate</span><span class="token punctuation">(</span> documentParsingFlow <span class="token punctuation">)</span>

<span class="token keyword">const</span> parsingProcess <span class="token operator">=</span> <span class="token punctuation">{</span>

 serviceStart<span class="token punctuation">:</span> <span class="token punctuation">[</span>
  <span class="token string">'initCoreRunner'</span><span class="token punctuation">,</span>
  <span class="token string">'registerStdTypes'</span><span class="token punctuation">,</span> <span class="token comment">// … to escape he oblivion</span>

  <span class="token string">'getParserList'</span><span class="token punctuation">,</span>
  <span class="token string">'fnIndex__Wikipedia'</span><span class="token punctuation">,</span> <span class="token comment">// … reusable components</span>
 <span class="token punctuation">]</span><span class="token punctuation">,</span>

 initSequence<span class="token punctuation">:</span> <span class="token punctuation">[</span>
  <span class="token string">'receiveProps'</span><span class="token punctuation">,</span>   <span class="token comment">// keyPath, parserList, </span>
  <span class="token string">'receiveObjects'</span><span class="token punctuation">,</span> <span class="token comment">// ctxAdapter or dbAdapter, …</span>
  <span class="token string">'parseConfig'</span><span class="token punctuation">,</span>
  <span class="token string">'parseRemappingSchema'</span><span class="token punctuation">,</span>
  <span class="token string">'parsePath'</span><span class="token punctuation">,</span>
  <span class="token string">'initParsers'</span><span class="token punctuation">,</span>
 <span class="token punctuation">]</span><span class="token punctuation">,</span>

 initParsers<span class="token punctuation">:</span> <span class="token punctuation">[</span> <span class="token comment">// … invoking sequences for expressions &amp; layout blocks (complex encoding &amp; text)</span>
  <span class="token string">'receiveProps'</span><span class="token punctuation">,</span>
  <span class="token string">'initBlocks'</span><span class="token punctuation">,</span>
  <span class="token string">'initKeywords'</span><span class="token punctuation">,</span>
  <span class="token string">'initExpressions'</span><span class="token punctuation">,</span>
  <span class="token string">'intoTrie'</span><span class="token punctuation">,</span> <span class="token comment">// expressionFn to tokenize with</span>
 <span class="token punctuation">]</span><span class="token punctuation">,</span>

 parseDirectory<span class="token punctuation">:</span> <span class="token punctuation">[</span>
  <span class="token string">'findConfig'</span><span class="token punctuation">,</span>
  <span class="token string">'updateContext'</span><span class="token punctuation">,</span>
  <span class="token string">'parseFiles'</span><span class="token punctuation">,</span>
  <span class="token string">'setDatabaseTasks'</span><span class="token punctuation">,</span>
  <span class="token string">'setPending'</span>
 <span class="token punctuation">]</span><span class="token punctuation">,</span>


 <span class="token comment">// Processing information in normalized datasets</span>
 parseCollection<span class="token punctuation">:</span> <span class="token punctuation">[</span> <span class="token comment">// … JSON database output, SVG, RDF</span>
  <span class="token string">'sourceParamsToContext'</span><span class="token punctuation">,</span>
  <span class="token string">'parseDoc'</span>
 <span class="token punctuation">]</span><span class="token punctuation">,</span>

 parseFile<span class="token punctuation">:</span> <span class="token punctuation">[</span> <span class="token comment">// … not expecting XML and JS markup</span>
  <span class="token string">'parseDoc'</span><span class="token punctuation">,</span>
  <span class="token string">'filenameToContext'</span><span class="token punctuation">,</span>
  <span class="token string">'parseContext'</span>
 <span class="token punctuation">]</span><span class="token punctuation">,</span>

 parseDoc<span class="token punctuation">:</span> documentParsingFlow<span class="token punctuation">,</span>

 <span class="token comment">// Ad-hoc instructions from expressionFn in Trie</span>
	invokeSeq<span class="token punctuation">:</span> <span class="token punctuation">[</span>
		<span class="token string">'intoTrie'</span><span class="token punctuation">,</span>
 <span class="token punctuation">]</span><span class="token punctuation">,</span>
 
<span class="token comment">// There's a little more to it, though.</span>
 
</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token keyword">import</span> React <span class="token keyword">from</span> <span class="token string">'react'</span>
<span class="token keyword">import</span> _ <span class="token keyword">from</span> <span class="token string">'lodash'</span>

<span class="token keyword">import</span> <span class="token punctuation">{</span> <span class="token comment">// Logical operators — now building a necessary set (with usecases)</span>
	Scenario<span class="token punctuation">,</span> MatchOneOf <span class="token keyword">as</span> OneOf<span class="token punctuation">,</span> 
	ExpressionChain <span class="token keyword">as</span> Chain<span class="token punctuation">,</span> Trie<span class="token punctuation">,</span>
	ExpressionNativeJS <span class="token keyword">as</span> Expr<span class="token punctuation">,</span>
	Scoop <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'../logic'</span>

<span class="token keyword">import</span> <span class="token punctuation">{</span> Line <span class="token keyword">as</span> NL<span class="token punctuation">,</span> Headline <span class="token keyword">as</span> H<span class="token punctuation">,</span> Paragraph <span class="token keyword">as</span> P <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'./'</span> <span class="token comment">// Layout blocks</span>

<span class="token keyword">import</span> <span class="token punctuation">{</span> escapeExpression <span class="token keyword">as</span> e <span class="token punctuation">}</span> <span class="token keyword">from</span> <span class="token string">'../util'</span> <span class="token comment">// function unexistent here yet [!!!]</span>

<span class="token comment">/*
const exampleContent: "

	# Überschrift (aha!)

	Here is etwas
	1. Erste
	2. Zweite
	3. …

"
*/</span>


<span class="token keyword">export</span> <span class="token keyword">default</span> <span class="token keyword">function</span> <span class="token function">orderedList</span> <span class="token punctuation">(</span>props<span class="token punctuation">)</span> <span class="token punctuation">{</span>

	<span class="token comment">//</span>
	<span class="token comment">// Content blocks in which this expression can appear</span>
	<span class="token comment">//(even when not explicitly declared)</span>
	<span class="token comment">//</span>
	
	<span class="token keyword">this</span><span class="token punctuation">.</span>compatible <span class="token operator">=</span> <span class="token punctuation">{</span> 
		<span class="token keyword">in</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token comment">// Needless to declare: "Document.*"</span>
			text2json<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Section"</span><span class="token punctuation">,</span> <span class="token string">"Paragraph"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
			parserName<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">""</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
			parserName_2<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">""</span><span class="token punctuation">]</span>
		<span class="token punctuation">}</span><span class="token punctuation">,</span>
		contains<span class="token punctuation">:</span> <span class="token punctuation">{</span>
			parserName<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Expressions"</span><span class="token punctuation">,</span> <span class="token string">"Blocks"</span><span class="token punctuation">]</span>
		<span class="token punctuation">}</span><span class="token punctuation">,</span>
		<span class="token keyword">with</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token comment">// Both wrapped "in" or "contains"</span>
			parserName<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Expr"</span><span class="token punctuation">,</span> <span class="token string">"Block"</span><span class="token punctuation">]</span>
		<span class="token punctuation">}</span><span class="token punctuation">,</span>
		not<span class="token punctuation">:</span> <span class="token punctuation">{</span>
			parserName<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Expr"</span><span class="token punctuation">,</span> <span class="token string">"Block"</span><span class="token punctuation">]</span>
		<span class="token punctuation">}</span>
	<span class="token punctuation">}</span>
	<span class="token comment">// … Is extensible (before considering fnIndex__Wikipedia)</span>
	<span class="token keyword">if</span><span class="token punctuation">(</span>_<span class="token punctuation">.</span><span class="token function">isObject</span><span class="token punctuation">(</span>props<span class="token punctuation">.</span><span class="token keyword">in</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
		compatible<span class="token punctuation">.</span><span class="token keyword">in</span> <span class="token operator">=</span> _<span class="token punctuation">.</span><span class="token function">merge</span><span class="token punctuation">(</span>compatible<span class="token punctuation">.</span><span class="token keyword">in</span><span class="token punctuation">,</span> props<span class="token punctuation">.</span><span class="token keyword">in</span><span class="token punctuation">)</span>


	<span class="token keyword">this</span><span class="token punctuation">.</span>symbols <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token punctuation">}</span>


	<span class="token keyword">this</span><span class="token punctuation">.</span>NumberedItem <span class="token operator">=</span> <span class="token punctuation">{</span>
		expr<span class="token punctuation">:</span> <span class="token string">"numberedItem"</span><span class="token punctuation">,</span>
		compatible<span class="token punctuation">:</span> <span class="token punctuation">{</span>
			<span class="token keyword">in</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token operator">...</span>compatible <span class="token punctuation">}</span><span class="token punctuation">,</span>
			contains<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token operator">...</span>compatible <span class="token punctuation">}</span><span class="token punctuation">,</span>
			ruleOut<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token operator">...</span>compatible <span class="token punctuation">}</span>
		<span class="token punctuation">}</span><span class="token punctuation">,</span>
		symbols<span class="token punctuation">:</span> <span class="token punctuation">{</span>
			opening<span class="token punctuation">:</span> <span class="token punctuation">{</span>
				<span class="token string">"[0-9]+\.\s"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"md"</span><span class="token punctuation">,</span> <span class="token string">"text2json"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
				<span class="token string">"[0-9]+\s{0,1}\)\s+"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"text2json"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
				<span class="token string">"[0-9]+\s+"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"text2json"</span><span class="token punctuation">]</span>
			<span class="token punctuation">}</span>
		<span class="token punctuation">}</span><span class="token punctuation">,</span>
		match<span class="token punctuation">:</span> <span class="token punctuation">(</span>input<span class="token punctuation">,</span> el<span class="token punctuation">,</span> db<span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>


			<span class="token comment">// Does the previous list item somehow share the same block?</span>
			<span class="token comment">//</span>
			<span class="token comment">// Conditions must be met (descending by priority — higher priority first):</span>
			<span class="token comment">// — at least two items with an ascending order of numbers exist at same indentation</span>
			<span class="token comment">// — no elements with a lower depth from tree root exist in between two items</span>
			<span class="token comment">//	(ie.: left in tree ~ with a smaller indentation)</span>
			<span class="token keyword">var</span> previousListItem


			<span class="token comment">// 1) run a query (when expression doesn't issue temporary tokens)</span>
			previousListItem <span class="token operator">=</span> db
				<span class="token punctuation">.</span><span class="token keyword">get</span><span class="token punctuation">(</span><span class="token string">'tokens'</span><span class="token punctuation">)</span>
				<span class="token punctuation">.</span><span class="token function">queryTx</span><span class="token punctuation">(</span><span class="token punctuation">{</span>	<span class="token comment">// … </span>
					expr<span class="token punctuation">:</span> el<span class="token punctuation">.</span>expr<span class="token punctuation">,</span>
					parser<span class="token punctuation">:</span> <span class="token keyword">null</span><span class="token punctuation">,</span>
					<span class="token keyword">with</span><span class="token punctuation">:</span> compatible<span class="token punctuation">,</span>
					<span class="token comment">// When retrieving token data …</span>
					ref<span class="token punctuation">:</span> <span class="token number">123</span><span class="token punctuation">,</span>				<span class="token comment">// — shares one of the same containers</span>
					treeDepth_current<span class="token punctuation">:</span> <span class="token number">123</span><span class="token punctuation">,</span> <span class="token comment">// — is on the same level as previous token</span>
					treeDepth_search<span class="token punctuation">:</span> <span class="token number">3</span><span class="token punctuation">,</span>		<span class="token comment">// — will traverse tree of tokens N levels</span>
					<span class="token comment">// Sorting results</span>
					sort<span class="token punctuation">:</span> <span class="token string">"desc"</span><span class="token punctuation">,</span>
					limit<span class="token punctuation">:</span> <span class="token number">1</span><span class="token punctuation">,</span>
					recent<span class="token punctuation">:</span> <span class="token number">1</span> <span class="token comment">// shorthand for the above two parameters</span>
				<span class="token punctuation">}</span><span class="token punctuation">)</span>
				<span class="token punctuation">.</span><span class="token function">value</span><span class="token punctuation">(</span><span class="token punctuation">)</span>

			<span class="token comment">// 2) or check cache (when expression)</span>
			previousListItem <span class="token operator">=</span> db
				<span class="token punctuation">.</span><span class="token keyword">get</span><span class="token punctuation">(</span><span class="token string">'tokens.cache'</span><span class="token punctuation">)</span>
				<span class="token punctuation">.</span><span class="token function">find</span><span class="token punctuation">(</span><span class="token punctuation">{</span> expr<span class="token punctuation">:</span> el<span class="token punctuation">.</span>expr<span class="token punctuation">,</span> blocks<span class="token punctuation">:</span> <span class="token string">'!!!'</span> <span class="token punctuation">}</span><span class="token punctuation">)</span> <span class="token comment">// … matching IDs</span>
				<span class="token punctuation">.</span><span class="token function">recent</span><span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">)</span>
				<span class="token punctuation">.</span><span class="token function">value</span><span class="token punctuation">(</span><span class="token punctuation">)</span>


			end <span class="token operator">=</span> <span class="token punctuation">(</span>previousListItem<span class="token punctuation">)</span> <span class="token operator">?</span> previousListItem<span class="token punctuation">.</span>index <span class="token punctuation">:</span> <span class="token number">1</span>
			<span class="token keyword">for</span> <span class="token punctuation">(</span>i <span class="token operator">=</span> input<span class="token punctuation">.</span>first <span class="token punctuation">;</span> i <span class="token operator">&lt;=</span> end <span class="token punctuation">;</span> i<span class="token operator">++</span><span class="token punctuation">)</span><span class="token punctuation">{</span>

				<span class="token keyword">if</span><span class="token punctuation">(</span> matchingExpression <span class="token punctuation">)</span><span class="token punctuation">{</span>

					end<span class="token operator">++</span>

					db<span class="token punctuation">.</span><span class="token keyword">get</span><span class="token punctuation">(</span><span class="token string">'parser.runtime'</span><span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token function">setBufferLen</span><span class="token punctuation">(</span><span class="token keyword">this</span><span class="token punctuation">.</span>expr<span class="token punctuation">)</span> <span class="token comment">// [!!!] Pass expression/block token ID</span>
				<span class="token punctuation">}</span>
			<span class="token punctuation">}</span>

			db<span class="token punctuation">.</span><span class="token keyword">get</span><span class="token punctuation">(</span><span class="token string">'parser.runtime'</span><span class="token punctuation">)</span><span class="token punctuation">.</span><span class="token function">resetBufferLen</span><span class="token punctuation">(</span><span class="token keyword">this</span><span class="token punctuation">.</span>expr<span class="token punctuation">)</span> <span class="token comment">// [!!!] Pass expression/block token ID</span>


			<span class="token keyword">return</span> <span class="token punctuation">{</span> i <span class="token punctuation">}</span>

		<span class="token punctuation">}</span><span class="token punctuation">,</span>
		trie<span class="token punctuation">:</span> <span class="token punctuation">{</span>  <span class="token punctuation">}</span>
	<span class="token punctuation">}</span>
	<span class="token comment">// … Is extensible</span>
	<span class="token keyword">if</span><span class="token punctuation">(</span>_<span class="token punctuation">.</span><span class="token function">isObject</span><span class="token punctuation">(</span>props<span class="token punctuation">.</span>NumberedItem<span class="token punctuation">.</span>symbols<span class="token punctuation">)</span><span class="token punctuation">)</span>
		NumberedItem<span class="token punctuation">.</span>symbols <span class="token operator">=</span> <span class="token function">extendSymbols</span><span class="token punctuation">(</span>NumberedItem<span class="token punctuation">.</span>symbols<span class="token punctuation">,</span> props<span class="token punctuation">.</span>symbols<span class="token punctuation">)</span>


	<span class="token keyword">return</span> <span class="token punctuation">(</span>

		<span class="token operator">&lt;</span>OrderedList componentLang<span class="token operator">=</span><span class="token string">"en"</span><span class="token operator">&gt;</span>

			<span class="token operator">&lt;</span>Scoop<span class="token operator">&gt;</span>

				<span class="token operator">&lt;</span>H <span class="token operator">/</span><span class="token operator">&gt;</span>
				<span class="token operator">&lt;</span>P <span class="token operator">/</span><span class="token operator">&gt;</span>

				<span class="token operator">&lt;</span>OneOf resolve<span class="token operator">=</span><span class="token string">"auto"</span><span class="token operator">&gt;</span>
					<span class="token operator">&lt;</span>Scenario<span class="token operator">&gt;</span>
						<span class="token operator">&lt;</span>Expr <span class="token keyword">with</span><span class="token operator">=</span><span class="token string">"{this.NumberedItem}"</span><span class="token operator">&gt;</span>
							<span class="token punctuation">{</span>children<span class="token punctuation">}</span>
<span class="token punctuation">{</span> <span class="token comment">/*

	Expressions which are repeated should	not overload the 
	Trie parser structure	with recurrence. Rather, they should be	
	separately listed in a non-parsable category.

								&lt;Scenario&gt;
									{children}
								&lt;/Scenario&gt;
								&lt;Scenario&gt;
									{children}
								&lt;/Scenario&gt;
*/</span> <span class="token punctuation">}</span>
						<span class="token operator">&lt;</span><span class="token operator">/</span>Expr<span class="token operator">&gt;</span>
					<span class="token operator">&lt;</span><span class="token operator">/</span>Scenario<span class="token operator">&gt;</span>

					<span class="token operator">&lt;</span>Scenario<span class="token operator">&gt;</span>
						<span class="token operator">&lt;</span>Expr <span class="token keyword">with</span><span class="token operator">=</span><span class="token string">"{this.AlphabeticalItem}"</span><span class="token operator">&gt;</span>
							<span class="token punctuation">{</span>children<span class="token punctuation">}</span>
						<span class="token operator">&lt;</span><span class="token operator">/</span>Expr<span class="token operator">&gt;</span>
					<span class="token operator">&lt;</span><span class="token operator">/</span>Scenario<span class="token operator">&gt;</span>
				<span class="token operator">&lt;</span><span class="token operator">/</span>OneOf<span class="token operator">&gt;</span>

			<span class="token operator">&lt;</span><span class="token operator">/</span>Scoop<span class="token operator">&gt;</span>

		<span class="token operator">&lt;</span><span class="token operator">/</span>OrderedList<span class="token operator">&gt;</span>
	<span class="token punctuation">)</span>
<span class="token punctuation">}</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
<span class="token keyword">export</span> <span class="token punctuation">{</span>
  exprWrap<span class="token punctuation">,</span> extendGen<span class="token punctuation">,</span>
  generateTokenId

  <span class="token comment">// stdExpr, noSuffix, withSuffix (some RegExp types)</span>
<span class="token punctuation">}</span>

<span class="token comment">// Understand expressions, deterministic first off (NSFW)?</span>
<span class="token comment">/*

## Expression function wrapper validates "arguments" and resolves subtypes

*/</span>  <span class="token comment">//  //  //</span>

<span class="token keyword">const</span> exprWrap <span class="token operator">=</span> <span class="token punctuation">(</span> exprFn<span class="token punctuation">,</span> argList <span class="token operator">=</span> <span class="token punctuation">[</span>
 <span class="token comment">/* Sets of arguments: runtime, subtype (&amp; internal) */</span>
<span class="token punctuation">]</span> <span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>


	 <span class="token keyword">var</span> wrap <span class="token operator">=</span> <span class="token punctuation">{</span> <span class="token comment">/* … will await a call in memory */</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>
  inputSchema <span class="token operator">=</span> <span class="token keyword">null</span><span class="token punctuation">,</span> err <span class="token operator">=</span> <span class="token keyword">null</span>

  <span class="token keyword">if</span> <span class="token punctuation">(</span> <span class="token operator">!</span>argList<span class="token punctuation">.</span>length <span class="token punctuation">)</span><span class="token punctuation">{</span> <span class="token comment">// Check to save some memory</span>
    <span class="token keyword">var</span> <span class="token punctuation">{</span> 
     invokeSeq<span class="token punctuation">,</span> inputSchema<span class="token punctuation">,</span> configInternal 
    <span class="token punctuation">}</span> <span class="token operator">=</span> <span class="token function">exprFn</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token comment">// … an introductory greeting call</span>
  <span class="token punctuation">}</span>


  <span class="token comment">//</span>
  <span class="token comment">// Expression validation layer</span>

  <span class="token keyword">const</span> <span class="token function-variable function">runValid</span> <span class="token operator">=</span> <span class="token keyword">function</span><span class="token punctuation">(</span> 
   fn <span class="token operator">=</span> exprFn<span class="token punctuation">,</span> argList <span class="token operator">=</span> argList<span class="token punctuation">,</span> schema <span class="token operator">=</span> inputSchema 
  <span class="token punctuation">)</span><span class="token punctuation">{</span>

    <span class="token keyword">if</span><span class="token punctuation">(</span> <span class="token operator">!</span>schema <span class="token punctuation">)</span>
      <span class="token keyword">var</span> inputSchema <span class="token operator">=</span> <span class="token function">exprFn</span><span class="token punctuation">(</span><span class="token string">'inputSchema'</span><span class="token punctuation">)</span>

    <span class="token comment">// Check inputs</span>
    <span class="token keyword">return</span> <span class="token punctuation">(</span> err <span class="token operator">=</span> <span class="token function">evaluateArgs</span><span class="token punctuation">(</span>inputSchema<span class="token punctuation">,</span> argList<span class="token punctuation">)</span> <span class="token punctuation">)</span>
    <span class="token operator">?</span> <span class="token function">fn</span><span class="token punctuation">(</span> argList <span class="token punctuation">)</span> 
    <span class="token punctuation">:</span> err
  <span class="token punctuation">}</span>


  <span class="token comment">//</span>
  <span class="token comment">// Wrapping up ...</span>
  <span class="token comment">//</span>

  <span class="token function-variable function">wrap</span> <span class="token operator">=</span> <span class="token punctuation">(</span>runtimeArgs <span class="token operator">=</span> <span class="token keyword">null</span><span class="token punctuation">,</span> subtypeArgs <span class="token operator">=</span> <span class="token keyword">null</span><span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>

    <span class="token keyword">var</span> argList <span class="token operator">=</span> <span class="token punctuation">(</span> runtimeArgs <span class="token operator">||</span> subtypeArgs <span class="token punctuation">)</span> 
      <span class="token operator">?</span> <span class="token function">mergeArrays</span><span class="token punctuation">(</span> runtimeArgs<span class="token punctuation">,</span> subtypeArgs<span class="token punctuation">)</span>
      <span class="token punctuation">:</span> <span class="token keyword">null</span>

    <span class="token keyword">if</span> <span class="token punctuation">(</span> <span class="token operator">!</span>inputSchema <span class="token punctuation">)</span>
      <span class="token keyword">var</span> inputSchema <span class="token operator">=</span> <span class="token function">exprFn</span><span class="token punctuation">(</span><span class="token string">'inputSchema'</span><span class="token punctuation">)</span>

    <span class="token keyword">return</span> <span class="token function">runValid</span><span class="token punctuation">(</span> exprFn<span class="token punctuation">,</span> argList<span class="token punctuation">,</span> schema <span class="token punctuation">)</span> <span class="token punctuation">}</span><span class="token punctuation">;</span>


  wrap<span class="token punctuation">.</span><span class="token function-variable function">defineType</span> <span class="token operator">=</span> <span class="token punctuation">(</span> typeName<span class="token punctuation">,</span> typeArgs <span class="token punctuation">)</span> <span class="token operator">=&gt;</span> <span class="token punctuation">{</span>

    <span class="token keyword">if</span> <span class="token punctuation">(</span> <span class="token operator">!</span>inputSchema <span class="token punctuation">)</span>
      <span class="token keyword">var</span> <span class="token punctuation">{</span> 
       invokeSeq<span class="token punctuation">,</span> inputSchema<span class="token punctuation">,</span> configInternal 
      <span class="token punctuation">}</span> <span class="token operator">=</span> <span class="token function">exprFn</span><span class="token punctuation">(</span><span class="token punctuation">{</span> <span class="token string">'greetWith'</span><span class="token punctuation">:</span> argList <span class="token punctuation">}</span><span class="token punctuation">)</span>

    <span class="token keyword">var</span> <span class="token function-variable function">wrapType</span> <span class="token operator">=</span> <span class="token keyword">function</span><span class="token punctuation">(</span> runtimeArgs <span class="token operator">=</span> <span class="token keyword">null</span> <span class="token punctuation">)</span><span class="token punctuation">{</span>
    
      <span class="token keyword">var</span> argList <span class="token operator">=</span> <span class="token punctuation">(</span> runtimeArgs <span class="token punctuation">)</span>
        <span class="token operator">?</span> <span class="token function">mergeArrays</span><span class="token punctuation">(</span> runtimeArgs<span class="token punctuation">,</span> typeArgs <span class="token punctuation">)</span>
        <span class="token punctuation">:</span> typeArgs

      <span class="token keyword">return</span> <span class="token function">runValid</span><span class="token punctuation">(</span> exprFn<span class="token punctuation">,</span> argList<span class="token punctuation">,</span> inputSchema <span class="token punctuation">)</span>
    <span class="token punctuation">}</span>

    wrapType<span class="token punctuation">.</span>config <span class="token operator">=</span> configInternal<span class="token punctuation">,</span>
    wrapType<span class="token punctuation">.</span>invokeSeq <span class="token operator">=</span> invokeSeq

    <span class="token keyword">return</span> wrapType
  <span class="token punctuation">}</span>

  <span class="token comment">//</span>
  <span class="token comment">// … Any differences here and there?</span>
  <span class="token comment">// ( .config and .invokeSeq )</span>
  <span class="token comment">//</span>

  <span class="token keyword">if</span> <span class="token punctuation">(</span>inputSchema<span class="token punctuation">)</span> <span class="token punctuation">{</span>
    wrap<span class="token punctuation">.</span>config <span class="token operator">=</span> configInternal
    wrap<span class="token punctuation">.</span>invokeSeq <span class="token operator">=</span> invokeSeq
  <span class="token punctuation">}</span>


  <span class="token keyword">return</span> wrap<span class="token punctuation">;</span>
<span class="token punctuation">}</span> <span class="token comment">// … consider storing within wraps the "db.tokens" references, and greeting's object's "checksum" values (for comparison)</span>


<span class="token comment">//</span>
<span class="token comment">// # Invoking a variety of types by arguments</span>
<span class="token comment">// … storing and accessing subtypes of one expression</span>
<span class="token comment">//</span>
<span class="token comment">// ie. expressionType(), expression Type["subtype"]</span>
<span class="token comment">//</span>

</code></pre>
<pre class=" language-js"><code class="prism  language-js">
__indexParams <span class="token operator">=</span> <span class="token punctuation">{</span> <span class="token comment">// …</span>
  lastInsert<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'{t}'</span><span class="token punctuation">,</span> <span class="token string">'{i}'</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
  trie<span class="token punctuation">:</span> <span class="token punctuation">{</span>
 <span class="token comment">/*  Optimized fast-access index
   … a derivate of query patterns (of frequent and relevant steps in loop) */</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>
 <span class="token string">'{sortedBy}'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span>  <span class="token comment">// … inMemory cache (once)</span>
    store<span class="token punctuation">:</span> <span class="token punctuation">{</span> data<span class="token punctuation">:</span> <span class="token boolean">false</span><span class="token punctuation">,</span> captions<span class="token punctuation">:</span> <span class="token boolean">false</span><span class="token punctuation">,</span> refs<span class="token punctuation">:</span> <span class="token boolean">true</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>
    count<span class="token punctuation">:</span> <span class="token string">'{n}'</span><span class="token punctuation">,</span>

    totalRanges<span class="token punctuation">:</span> <span class="token punctuation">{</span>
     <span class="token number">0</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'{a_}'</span><span class="token punctuation">,</span> <span class="token string">'{b_}'</span><span class="token punctuation">,</span> <span class="token string">'{a__utf8}'</span><span class="token punctuation">,</span> <span class="token string">'{z__utf8}'</span><span class="token punctuation">]</span>
    <span class="token punctuation">}</span><span class="token punctuation">,</span>
    rangeByKeyIndex<span class="token punctuation">:</span> <span class="token punctuation">{</span>
     <span class="token number">0</span><span class="token punctuation">:</span> <span class="token punctuation">[</span>
        <span class="token punctuation">[</span> <span class="token string">'{a_}'</span><span class="token punctuation">,</span> <span class="token string">'{b_}'</span><span class="token punctuation">,</span> <span class="token string">'{a__utf8}'</span><span class="token punctuation">,</span> <span class="token string">'{b__utf8}'</span><span class="token punctuation">,</span> <span class="token string">'{i}'</span><span class="token punctuation">,</span> <span class="token string">'{n}'</span><span class="token punctuation">,</span> <span class="token string">'{indexObj__next}'</span><span class="token punctuation">,</span> <span class="token string">'{indexObj__prev}'</span> <span class="token punctuation">]</span> <span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token punctuation">]</span><span class="token punctuation">,</span>

    expireAfter<span class="token punctuation">:</span> <span class="token operator">-</span><span class="token number">1</span><span class="token punctuation">,</span>
    insertedKeys<span class="token punctuation">:</span> <span class="token punctuation">[</span>    <span class="token comment">// … unprocessed inserted row numbers</span>
      <span class="token punctuation">{</span> t<span class="token punctuation">:</span> <span class="token keyword">null</span><span class="token punctuation">,</span> i<span class="token punctuation">:</span> <span class="token keyword">null</span><span class="token punctuation">,</span> key<span class="token punctuation">:</span> <span class="token keyword">null</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>
    <span class="token punctuation">]</span><span class="token punctuation">,</span>
    stepPolynomial<span class="token punctuation">:</span> <span class="token punctuation">[</span>  <span class="token comment">// … keyword density at traversed areas</span>
      <span class="token punctuation">{</span> <span class="token string">'{routeMatch}'</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'{a__utf8}'</span><span class="token punctuation">,</span> <span class="token string">'{b__utf8}'</span><span class="token punctuation">,</span> <span class="token string">'{i}'</span><span class="token punctuation">,</span> <span class="token string">'{n}'</span><span class="token punctuation">,</span>
        <span class="token string">'{lastQueryAt}'</span><span class="token punctuation">,</span> <span class="token string">'{queryFrequency}'</span><span class="token punctuation">,</span> <span class="token string">'{avgMatchRatio}'</span><span class="token punctuation">]</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>
    <span class="token punctuation">]</span><span class="token punctuation">,</span>
    lastQueryAt<span class="token punctuation">:</span> <span class="token string">'{timestamp}'</span><span class="token punctuation">,</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>
  priority<span class="token punctuation">:</span> <span class="token punctuation">{</span> highest<span class="token punctuation">:</span> <span class="token number">1</span><span class="token punctuation">,</span> lowest<span class="token punctuation">:</span> <span class="token number">4</span><span class="token punctuation">,</span> 
    deprioritizeUntil<span class="token punctuation">:</span> <span class="token number">2</span><span class="token punctuation">,</span> offloadAt<span class="token punctuation">:</span> <span class="token number">3</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>
  methodsWikipedia<span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token string">'{functionPath}'</span><span class="token punctuation">:</span> <span class="token string">'{Wikipedia__URL}'</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>
<span class="token punctuation">}</span><span class="token punctuation">,</span>


<span class="token function-variable function">indexLoops</span> <span class="token operator">=</span> <span class="token keyword">function</span><span class="token punctuation">(</span> onionPath<span class="token punctuation">,</span> <span class="token comment">// </span>

  sortedBy <span class="token operator">=</span> <span class="token punctuation">{</span>
  <span class="token string">'{timestamp.update}'</span><span class="token punctuation">:</span> <span class="token string">'DESC'</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>
  rangeParams <span class="token operator">=</span> <span class="token punctuation">{</span>
    offset<span class="token punctuation">:</span> <span class="token number">0</span><span class="token punctuation">,</span> limit<span class="token punctuation">:</span> <span class="token number">30</span><span class="token punctuation">,</span>
  <span class="token string">'{timestamp.update}'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> a_<span class="token punctuation">:</span> <span class="token number">0</span><span class="token punctuation">,</span> b_<span class="token punctuation">:</span> <span class="token function">char</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token operator">^</span><span class="token number">64</span><span class="token punctuation">)</span> <span class="token punctuation">}</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>

  returnType <span class="token operator">=</span> <span class="token punctuation">{</span>
    data<span class="token punctuation">:</span> <span class="token boolean">false</span><span class="token punctuation">,</span>
    captions<span class="token punctuation">:</span> <span class="token boolean">false</span><span class="token punctuation">,</span>
    ref<span class="token punctuation">:</span> <span class="token boolean">true</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>
  persistentIndex <span class="token operator">=</span> <span class="token punctuation">{</span>
    expire<span class="token punctuation">:</span> <span class="token number">7</span><span class="token operator">*</span><span class="token number">24</span><span class="token operator">*</span><span class="token number">3600</span><span class="token punctuation">,</span>
    priority<span class="token punctuation">:</span> <span class="token punctuation">{</span> high<span class="token punctuation">:</span> <span class="token number">1</span><span class="token punctuation">,</span> low<span class="token punctuation">:</span> <span class="token number">4</span><span class="token punctuation">,</span> offload<span class="token punctuation">:</span> <span class="token number">3</span> <span class="token punctuation">}</span><span class="token punctuation">,</span>
    maxLen<span class="token punctuation">:</span> <span class="token number">5000</span><span class="token punctuation">,</span>
    minLen<span class="token punctuation">:</span> <span class="token number">1000</span>
  <span class="token punctuation">}</span>

<span class="token punctuation">)</span><span class="token punctuation">{</span>

  <span class="token keyword">var</span> next <span class="token operator">=</span> <span class="token punctuation">(</span> <span class="token keyword">typeof</span> onionPath<span class="token punctuation">.</span>next <span class="token operator">===</span> <span class="token string">'object'</span> <span class="token punctuation">)</span>
              <span class="token operator">?</span> onionPath<span class="token punctuation">.</span>next <span class="token punctuation">:</span> <span class="token keyword">null</span>
<span class="token comment">/*
  [
    {indexObj}, {i}, {order},
    {offset}, {limit},
    {returnType__obj},

    {sortingKey}, ({rangeParams__obj}), {order}, … ;

    {keyPath}, {persistentIndex_expire},
    {priority_a}, {priority_b}
  ]
 */</span>
</code></pre>
<pre class=" language-jsonion"><code class="prism .tx2gql language-jsonion">

      //    //    //    // Beware

     //   _.* =&gt; 1|.*  // Mashup

    //   __  =&gt; _     // Partials

   //    //    //    // Consideration


export default const collections = () =&gt; {
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

  ...collection.resource, // &lt;- repeat main resource

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
// Governed by entities (a group of people &amp; circles) with defined agency
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

</code></pre>
<pre class=" language-json"><code class="prism  language-json">
<span class="token punctuation">{</span>
<span class="token string">'.{propertyName} #'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> <span class="token comment">// … looking for Facebook 'status_updates'</span>
	 This<span class="token punctuation">:</span> <span class="token string">"post"</span><span class="token punctuation">,</span>
__allOf<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token punctuation">]</span><span class="token punctuation">,</span> <span class="token comment">// … is this the dataset we're looking for?</span>
__oneOf<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
	 map<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'timestamp'</span><span class="token punctuation">,</span> <span class="token string">'full_name'</span><span class="token punctuation">,</span> <span class="token string">'action'</span><span class="token punctuation">,</span> <span class="token string">'post'</span><span class="token punctuation">,</span> <span class="token string">'event_name'</span><span class="token punctuation">,</span> <span class="token string">'place_name'</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

 <span class="token string">'.title'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span>
    Remove<span class="token punctuation">:</span> <span class="token boolean">true</span><span class="token punctuation">,</span> <span class="token comment">// … task executed after jsIons react, while finally mapping to JSON tree</span>

		 <span class="token comment">// jsIons transform data state (where RegExp condition !false)</span>
	  <span class="token string">'/(.*) shared an event./'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span> 
	     As<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'full_name'</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
	    <span class="token string">'post.action'</span><span class="token punctuation">:</span> <span class="token string">'event_shared'</span>
 	  <span class="token punctuation">}</span><span class="token punctuation">,</span>
 	 <span class="token string">'/(.*) was attending (.*) at (.*)./'</span><span class="token punctuation">:</span> <span class="token punctuation">{</span>
	     As<span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">'full_name'</span><span class="token punctuation">,</span> <span class="token string">'event_name'</span><span class="token punctuation">,</span> <span class="token string">'place_name'</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
	    <span class="token string">'post.action'</span><span class="token punctuation">:</span> <span class="token string">'event_attending'</span>
	   <span class="token punctuation">}</span>
  <span class="token punctuation">}</span>
<span class="token punctuation">}</span><span class="token punctuation">,</span>
<span class="token comment">/*

Like dissoluted ions... The encoded parsing rules enter and react with substances kept in a medium's data structure; so to harness and map modified contents into a resulting JSON data tree.

*/</span>
<span class="token punctuation">}</span>

</code></pre>
<pre class=" language-gql"><code class="prism  language-gql">
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

 # Audit Trail: Modifications to data node state (History &amp; Draft)
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
</code></pre>
<pre class=" language-js"><code class="prism  language-js"><span class="token punctuation">{</span>
  <span class="token string">"__description"</span><span class="token punctuation">:</span> <span class="token string">"Register of built-in Types and their synonyms and expression sequences (right-hand)"</span><span class="token punctuation">,</span>
  <span class="token string">"__types"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Type"</span><span class="token punctuation">,</span> <span class="token string">"Synonym"</span><span class="token punctuation">,</span> <span class="token string">"Abbreviation"</span><span class="token punctuation">,</span> <span class="token string">"Reference"</span><span class="token punctuation">,</span> <span class="token string">"Operator"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
  <span class="token string">"__apply"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"/\s/"</span><span class="token punctuation">,</span> <span class="token string">"__strDecode"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
  
  <span class="token string">"P &lt;= TangibleProcess"</span><span class="token punctuation">:</span> <span class="token punctuation">{</span>

    <span class="token string">"Abbreviation"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Abbrev"</span><span class="token punctuation">,</span> <span class="token string">"Abbr"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token string">"Aggregation"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>

    <span class="token string">"Create"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>
    <span class="token string">"Read"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>
    <span class="token string">"Update"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>
    <span class="token string">"Delete"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>
    <span class="token string">"Select"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Filter"</span><span class="token punctuation">,</span> <span class="token string">"Pick"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token string">"Join"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Merge"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token string">"Insert"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>

    <span class="token string">"Difference"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Diff"</span><span class="token punctuation">,</span> <span class="token string">"~"</span><span class="token punctuation">,</span> <span class="token string">"%0% ~~ %1%"</span><span class="token punctuation">,</span> <span class="token string">"~="</span><span class="token punctuation">,</span> <span class="token string">"~=="</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token string">"Patch"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"%0% (%1%)-&gt; %2%"</span><span class="token punctuation">,</span> <span class="token string">"%0% -(%1%)&gt; %2%"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    
    <span class="token string">"Fork"</span><span class="token punctuation">:</span> <span class="token string">"Fork %0% -&gt; %1%"</span><span class="token punctuation">,</span>
    <span class="token string">"Stem"</span><span class="token punctuation">:</span> <span class="token string">"Stem %0% -&gt; %1%"</span><span class="token punctuation">,</span>
    
    <span class="token string">"functionIndexKeyStore"</span><span class="token punctuation">:</span> <span class="token string">"[%0%](https://wikipedia.org/en/%1%)"</span><span class="token punctuation">,</span>
    <span class="token string">"Initialization"</span><span class="token punctuation">:</span> <span class="token string">"Init"</span><span class="token punctuation">,</span>
    <span class="token string">"Input"</span><span class="token punctuation">:</span> <span class="token string">"I"</span><span class="token punctuation">,</span>
    <span class="token string">"Output"</span><span class="token punctuation">:</span> <span class="token string">"O"</span><span class="token punctuation">,</span>
    <span class="token string">"PointOfValidation"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"API"</span><span class="token punctuation">,</span> <span class="token string">"Mirror"</span><span class="token punctuation">,</span> <span class="token string">"Package"</span><span class="token punctuation">,</span> <span class="token string">"Module"</span><span class="token punctuation">,</span> <span class="token string">"Component"</span><span class="token punctuation">,</span> <span class="token string">"Function"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    
    <span class="token string">"Index"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"toIndex"</span><span class="token punctuation">,</span> <span class="token string">"i"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

    <span class="token string">"MapTo"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Remap"</span><span class="token punctuation">,</span> <span class="token string">"Map"</span><span class="token punctuation">,</span> <span class="token string">"%0% -&gt; %1%"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token string">"Reference"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Ref"</span><span class="token punctuation">,</span> <span class="token string">'\"%0%\" =&gt; \"%1%\"'</span><span class="token punctuation">,</span> <span class="token string">"\'%0%\' =&gt; \'%1%\'"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

    <span class="token string">"Pending"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>

    <span class="token string">"Query"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>
    <span class="token string">"Mutate"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>

    <span class="token string">"StringVariable"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"\{Var\}"</span><span class="token punctuation">,</span> <span class="token string">"{%}"</span><span class="token punctuation">,</span> <span class="token string">"{{%}}"</span><span class="token punctuation">,</span> <span class="token string">"${%}"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

    <span class="token string">"Trie"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"%0% { %1%"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

    <span class="token string">"Validation"</span><span class="token punctuation">:</span> <span class="token string">"null"</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>

  <span class="token string">"__caseInsensitive"</span><span class="token punctuation">:</span> <span class="token punctuation">{</span>
    <span class="token string">"jsonion"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>
    <span class="token string">"md"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"Markdown"</span><span class="token punctuation">,</span> <span class="token string">"CommonMark"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token string">"regex"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"RegExp"</span><span class="token punctuation">,</span> <span class="token string">"/%/"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
    <span class="token string">"v32svgn"</span><span class="token punctuation">:</span> <span class="token string">"null"</span><span class="token punctuation">,</span>
    <span class="token string">"validation"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span><span class="token string">"valida.jsonion"</span><span class="token punctuation">,</span> <span class="token string">"valida"</span><span class="token punctuation">,</span> <span class="token string">"validate"</span><span class="token punctuation">]</span><span class="token punctuation">,</span>
  <span class="token punctuation">}</span><span class="token punctuation">,</span>

  <span class="token string">"__footing"</span><span class="token punctuation">:</span> <span class="token punctuation">[</span>
    <span class="token string">"including String and Numeric types, as commonly redefined in schema validation"</span>
  <span class="token punctuation">]</span><span class="token punctuation">,</span>
  <span class="token string">"__syntax"</span><span class="token punctuation">:</span> <span class="token string">"JavaScript ES6"</span>
<span class="token punctuation">}</span>
</code></pre>

