## JSC News

### Technology Preview 119 [270749-371358](https://trac.webkit.org/log?stop_rev=270749&rev=271358&limit=999)

- Fixed non-enumerable property to shadow inherited enumerable property from for-in (r270874)
- Fixed Intl.DateTimeFormat#formatRange to generate the same output to Intl.DateTimeFormat#format if startDate and endDate are “practically-equal” (r271224)
- Implemented arbitrary-module-namespace-identifier-names (r270923)
- Improved performance of Object rest and spread (r271343)

### Technology Preview 118 [270230-270749](https://trac.webkit.org/log?stop_rev=270230&rev=270749&limit=999)

- Enabled “at” methods (r270550)
- Changed get and set for object literal and class to not be escaped (r270487)
- Accepted escaped keywords for class and object property names (r270481)
- Aligned %TypedArray% constructor/slice behavior with the specification strictly (r270552, r270371)
- Added a JSC API to allow acquiring the JSLock to accelerate performance (r270659)
- Removed unnecessary JSLock use from various JSC APIs (r270665)
- Aligned [[DefineOwnProperty]] method of mapped arguments object with the specification strictly (r270664)
- Changed Reflect.preventExtensions not throwing if called on WindowProxy or Location (r270702)

### Technology Preview 117 [268651-270230](https://trac.webkit.org/log?stop_rev=268651&rev=270230&limit=1579)

- Enabled static public class fields (r269922, r269939)
- Enabled static and instance private class fields (r270066)
- Implemented Intl.DateTimeFormat.formatRangeToParts (r269706)
- Implemented Intl.ListFormat (r268956)
- Aligned %TypedArray% behavior with recent spec adjustments (r269670)
- Implemented @@species support in ArrayBuffer#slice (r269574)
- Fixed toLocaleDateString() resolving incorrect date for some old dates (r269502)
- Resurrected SharedArrayBuffer and Atomics behind a flag (JSC_useSharedArrayBuffer=1) (r269531)

### Technology Preview 116 [267959-268651](https://trac.webkit.org/log?stop_rev=267959&rev=268651&limit=999)

- Changed arguments.callee to become ThrowTypeError if the function has a complex-parameter-list (spec-term) (r268323)
- Changed BigInt constructor to be constructible while it always throws an error (r268322)
- Fixed Array.prototype.sort‘s sortBucketSort which accessed an array in an invalid way leading to incorrect results with indexed properties on the prototype chain (r268375)
- Improved the essential internal methods for %TypedArray% to adhere to spec (r268640)

### Technology Preview 115 [267325-267959](https://trac.webkit.org/log?stop_rev=267325&rev=267959&limit=999)

- Fixed BigInt to work with Map and Set (r267373)
- Enabled Intl.DateTimeFormat dayPeriod (r267454)
- Updated Intl rounding behavior to align with specifications update (r267500)
- Updated functions to consistently enumerate length property before name property (r267364)
- Updated Array.prototype.sort to be consistent with specifications (r267514)
- Implemented item method proposal, note that this will be renamed to at later (r267814)

### Technology Preview 114 [265893-267325](https://trac.webkit.org/log?stop_rev=265893&rev=267325&limit=1432)

- Added Intl.DateTimeFormat dateStyle and timeStyle (r266035)
- Added Intl.Segmenter (r266032)
- Added a syntax error for async function in a single-statement context (r266340)
- Added Object.getOwnPropertyNames caching and accelerated Object.getOwnPropertyDescriptor (r265934)
- Aligned legacy Intl constructor behavior to spec (r266655)
- Applied Intl.DateTimeFormat hour-cycle correctly when timeStyle is used (r267108)
- Enabled Intl.DisplayNames (r266029)
- Changed to not allow let [ sequence to appear in an ExpressionStatement context (r266327)
- Changed to allow new super.property syntax (r266322)
- Changed to allow new import.meta() syntax (r266318)
- Changed to use locale-sensitive grouping for grouping options in IntlRelativeTimeFormat (r266341)
- Implemented Intl.DateTimeFormat dayPeriod (r266323)
- Implemented Intl Language Tag Parser (r266039)
- Implemented Intl.DateTimeFormat.prototype.formatRange (r266033)
- Implemented unified Intl.NumberFormat (r266031)
- Fixed an invalid early error for object literal method named proto (r266117)
- Fixed implementation of the class “extends” clause incorrectly using proto for setting prototypes (r266106)
- Fixed Performance and PerformanceNavigation interfaces missing toJSON operations (r267316)
- Updated Intl.Collator to take a collation option (r267102)
- Updated Array.prototype.push to always perform Set in strict mode (r266581, r266641)
- Updated Promise.prototype.finally to perform PromiseResolve (r266896)

### Technology Preview 113 [265179-265893](https://trac.webkit.org/log?stop_rev=265179&rev=265893&limit=999) WebKitGtk 2.30+ (r265542)

### Technology Preview 112 [264601-265179](https://trac.webkit.org/log?stop_rev=264852&rev=265331&limit=999)

- Implemented Intl.DisplayNames (r264639)
- Changed eval?.() to be an indirect eval (r264633)

### Technology Preview 111 [263988-264601](https://trac.webkit.org/log?stop_rev=263988&rev=264601&limit=999)

- Made String.protoytpe.toLocaleLowerCase'savailableLocales` HashSet more efficient (r264293)
- Changed Intl.Locale maximize, minimize to return Intl.Locale instead of String (r264275)
- Fixed Math.max() yielding the wrong result for max(0, -0) (r264507)
- Fixed redefining a property that should not change its insertion index (Object.keys order) (r264574)

### Technology Preview 110 [263214-263988](https://trac.webkit.org/log?stop_rev=263214&rev=263988&limit=999)

- Enabled RelativeTimeFormat and Locale by default (r263227)
- Configured option-offered numberingSystem in Intl.NumberFormat through locale (r263837)
- Changed Intl.Collator to set usage:”search” option through ICU locale (r263833)
- Fixed Promise built-in functions to be anonymous non-constructors (r263222)
- Fixed incorrect TypedArray.prototype.set with primitives (r263216)

### Technology Preview 109 [262502-263214](https://trac.webkit.org/log?stop_rev=262502&rev=263214&limit=999)

- Added support for private class fields (r262613)
- Added “el” (Greek) to our maintained available locales list (r262992)
- Changed Logical Assignment to perform NamedEvaluation of anonymous functions (r262638)
- Changed JSON.stringify to throw stack overflow error (r262727)
- Changed RegExp.prototype getters to throw on cross-realm access (r262908)
- Changed super to not depend on proto (r263035)
- Fixed AsyncGenerator to await return completions (r262979)
- Made errors an own property of AggregateError instead of a prototype accessor (r263006)

### Technology Preview 108 [262002-262502](https://trac.webkit.org/log?stop_rev=262002&rev=262502&limit=999)

- Fixed Array.prototype.splice not setting the length of the returned object if not an Array (r262088)
- Fixed BigInt operations to handle exceptions correctly (r262386)

### Technology Preview 107 [261057-262002](https://trac.webkit.org/log?stop_rev=261057&rev=262080&limit=999)

- Fixed Object.prototype.toString to match standards (r261159)
- Implemented Intl.Locale (r261215)
- Implemented BigInt.asIntN and BigInt.asUintN (r261156, r261199)
- Enabled logical assignment operators (r261728)
- Ensured IntlCollator.prototype.resolvedOptions returns relevant locale extension keys in alphabetical order (r261182)

### Technology Preview 106 [260266-261057](https://trac.webkit.org/log?stop_rev=260266&rev=261057&limit=999)

- Enabled BigInt (r260345)
- Changed BigInt constructor to accept larger integers than safe-integers (r260863)
- Added support for Intl.RelativeTimeFormat (r260349)
- Redesigned for-of iteration for arrays (r260323)

### Technology Preview 105 [259476-260266](https://trac.webkit.org/log?stop_rev=259472&rev=260266&limit=999)

- Fixed Intl.DateTimeFormat patterns and fields (r260145)
- Implemented BigInt.prototype.toLocaleString` (r259919)
- Updated Intl to allow calendar and numberingSystem options (r259941)
- Implemented logical assignment operators (r260119)
- Updated canonicalizeLocaleList to gracefully throw OOM error if the input and error message is too large (r259481)
- Updated module’s default cross-origin value should be “anonymous” (r260003, r260038)

### Technology Preview 104 [258409-259472](https://trac.webkit.org/log?stop_rev=258409&rev=259472&limit=999)

Updated Intl.NumberFormat.prototype.format to preserve a sign of -0 (r259370)

### Technology Preview 103 [257162-258409](https://trac.webkit.org/log?stop_rev=256576&rev=257162&limit=999)

### Technology Preview 102 [256576-257162](https://trac.webkit.org/log?stop_rev=256576&rev=257162&limit=999)

### Technology Preview 101 [255473-256576](https://trac.webkit.org/log?stop_rev=255473&rev=256576&limit=999) WebKit 2.28+ (r255666)

- Added support for BigInt literal as PropertyName (r256541)
- Fixed quantifiers after lookahead assertions to be syntax errors in Unicode patterns only (r255689)
- Fixed \0 identity escapes to be syntax errors in Unicode patterns only (r255584)

### Technology Preview 100 [254696-255473](https://trac.webkit.org/log?stop_rev=254696&rev=255473&limit=999)

- Fixed DateMath to accept more ISO-8601 timezone designators even if they are not included in ECMA262 to produce expected results in the wild code (r254939)

### Technology Preview 99 [253789-254696](https://trac.webkit.org/log?stop_rev=253789&rev=254696&limit=999)

- Changed Object.keys to throw if called on a module namespace object with uninitialized binding (r254390)
- Changed Object.preventExtensions to throw if not successful (r254626)
- Fixed String.prototype.replace() incorrectly handling named references on regular expressions without named groups (r254088)
- Fixed invalid date parsing for ISO 8601 strings when no timezone given (r254038)
- Fixed RegExp.prototype[Symbol.replace] to support named capture groups (r254195)


### Technology Preview 98 [252823-253789](https://trac.webkit.org/log?stop_rev=252823&rev=253789&limit=999)

- Changed Object.prototype.isPrototypeOf() to check if the passed in value is a non-object first (r253264)

### Technology Preview 97 [251627-252823](https://trac.webkit.org/log?stop_rev=251627&&rev=252823&limit=999)

- Added BigInt support for ++ and -- (r252680)
- Fixed Intl.DateTimeFormat to return resolvedOptions in the correct order (r251815)
- Optimized Promise runtime functions (r251671)
- Implement String.prototype.replaceAll (r252683)

### Technology Preview 96 [251210-251627](https://trac.webkit.org/log?stop_rev=251210&&rev=251627&limit=999)

Changed String.prototype.matchAll to throw on non-global regex (r251483)
Fixed a bad is array assertion JSON.parse (r251394)
Removed wasmAwareLexicalGlobalObject (r251529)

### Technology Preview 95 [250947-251210](https://trac.webkit.org/log?stop_rev=250947&&rev=251210&limit=999)

### Technology Preview 94 [250329-250947](https://trac.webkit.org/log?stop_rev=250329&&rev=250947&limit=999)

- Changed toExponential, toFixed, and toPrecision to allow arguments up to 100 (r250389)
- Fixed JSON.parse to correctly handle array proxies (r250860)

### Technology Preview 93 [249750-250329](https://trac.webkit.org/log?stop_rev=249750&&rev=250329&limit=999) (Kudo's 250230.2.1)

- Fixed Date.prototype.toJSON to properly execute (r249861)
- Added missing syntax errors for await in function parameter default expressions (r249925)

### Technology Preview 92 [249190-249750](https://trac.webkit.org/log?stop_rev=249190&&rev=249750&limit=999) WebKitGtk 2.26+

- Fixed Math.round() which produced a wrong result for value prior to 0.5 (r249597)
- Made Promise implementation faster (r249509)

### Technology Preview 91 [248705-249190](https://trac.webkit.org/log?stop_rev=248705&&rev=249190&limit=999)

- Added a public API for unhandled promise rejections (r249058)
- Added support for hashbang in ESNext (r248826)
- Implemented optional chaining in ESNext (r248829)
- Implemented StaticRange constructor (r249079)
- Fixed Date.prototype.toJSON to not throw an exception if toISOString returns an object (r248876)
- Fixed more missing exception checks in String.prototype (r248716)
- Fixed a bad error message when for-await-of is used in a non-async function (r248711)
- Fixed ProxyObject to not allow access to its target’s private properties (r248796)
- Updated the Promise constructor to check argument before `Construct?“ (r248787)
- Updated Promise.prototype.finally to accept non-promise objects (r248793)
- Changed to avoid looking up the join function each time Array.prototype.toString is called (r248906)
- Ensured x?.y ?? z is fast (r249117)

### Technology Preview 90 [248024-248705](https://trac.webkit.org/log?stop_rev=248024&&rev=248705&limit=999)

### Technology Preview 89 [247433-248024](https://trac.webkit.org/log?stop_rev=247433&&rev=248024&limit=999)

- Implemented nullish coalescing with the ?? operator for ESNext (r247819)

### Technology Preview 88 [247047-247433](https://trac.webkit.org/log?stop_rev=247047&&rev=247433&limit=999)

- Enabled Intl.PluralRules and Intl.NumberFormatToParts by default (r247247)

### Technology Preview 87 [246691-247047](https://trac.webkit.org/log?stop_rev=246691&&rev=247047&limit=999)

### Technology Preview 86 [246093-246691](https://trac.webkit.org/log?stop_rev=246093&&rev=246691&limit=999)

- Added support for String.prototype.matchAll (r246567))
- Changed to throw a TypeError exception if Proxy’s set trap returns falsy value (r246346)
- Fixed JSON.parse to throw a syntax error when called without arguments (r246162)

### Technology Preview 85 [245618-246093](https://trac.webkit.org/log?stop_rev=245618&&rev=246093&limit=999)

- Implemented Promise.allSettled (r245869)
- Implemented support for Numeric Separators (r245655)
- Implemented opwide16 and opwide32 and introduced 16-bit version bytecode (r245906)
- Fixed InferredValue to not be a JSCell (r246073)
- Reduced metadata footprint (r245658)
- Changed createListFromArrayLike to throw a type error if the value is not an object (r245675)

### Technology Preview 83 (245007-245618) (RN official 245459.0.0)

- 