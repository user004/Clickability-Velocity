# Clickabilty Velocity

Based on [jampow's Velocty package](https://github.com/jampow/velocity-sublime), but modified to use [Clickability](http://www.clickability.com/)'s custom functions and version of Velocity. Somewhat built using the Template Language Reference Guide.

## Snippets

### ArrayLists

| Shortcut | Output |
| --- | --- |
| `al` | `$util.newArrayList` |
| `..` | `[ start .. end ]` |
| `.addAll` | `.addAll( arrayList )` |
| `.add` | `.add( <index, >object )` |
| `.clear` | `.clear()` |
| `.contains` | `.contains( object )` |
| `.get` | `.get( index )` |
| `.indexOf` | `.indexOf( object )` |
| `.isEmpty` | `.isEmpty()` |
| `.remove` | `.remove( index )` |
| `.set` | `.set( index, object )` |
| `.subList` | `.subList( start, end )` |

### CMS

| Shortcut | Output |
| --- | --- |
| `cat` | `$cms.getCategorization( [ 'sets' ], [ 'categories' ]<, match all> )` |
| `clinks` | `$cms.categorizedLinks( categorization, 'domain', 'name/path', index, size )` |
| `cont` | `$cms.content( id )` |
| `flinks` | `$cms.filteredLinks( 'content type', 'domain', 'name/path', index, size )` |
| `link` | `$cms.link( 'domain', 'name/path', index )` |
| `links` | `$cms.links( 'domain', 'name/path', index, size )` |
| `parent` | `cms.parent( 'domain', 'name/path/object' )` |
| `temp` | `${cms.template( 'name' )}##` |
| `parent` | `$cms.parent( '(string/object) ID/domain/name/path/section', '(int/string) ID/name/path' )` |
| `wss` | `$cms.websiteSection( 'domain', 'id/name/path' )` |

### Dates

* newDate
* Date
* Add
* Now
* Tomorrow
* Yesterday
* compareDates
* currentYear
* difference
* getDate
* getDay
* getHours
* getMinutes
* getMonth
* getSeconds
* getTime
* getTimezoneOffset
* getYear
* inSameDay
* inSameHour
* inSameMonth
* inSameYear
* isAfter
* isBefore
* isBetween
* isEqualDate
* isEqualTime
* parseDate
* toDateTime
* whenIs

### Directives

| Shortcut | Output |
| --- | --- |
| `set` | `#set( $name = expression )` |
| `for` |
```
#foreach( item in itemList )##
	## statement
#end##
```
| Shortcut | Output |
| --- | --- |
| `if` |
```
#if( condition )##
	## statement
#end##
```
| Shortcut | Output |
| --- | --- |
| `else` |
```
#else[if( condition )]##
	## statement
```
| Shortcut | Output |
| --- | --- |
| `end` | `#end##` |

### HashMaps

| Shortcut | Output |
| --- | --- |
| `hm` | `$util.newHashMap` |

### Helpers

| Shortcut | Output |
| --- | --- |
| `$` | `$[!]{variable}` |
| `vc` | `$velocityCount` |
| `#*` |
```
#* ============================================================================
Company Name
Copyright, Year
Title: Template Name
========================================================================== *###
```

### Math

| Shortcut | Output |
| --- | --- |
| `double` | `$math.newDouble( number )` |
| `float` | `$math.newFloat( number )` |
| `int` | `$math.newInt( number )` |
| `%` | `$math.mod( integer, integer )` |
| `*` | `$math.multiply( number, number )` |
| `+` | `$math.add( number, number )` |
| `-` | `$math.subtract( number, number )` |
| `/` | `$math.divide( number, number )` |
| `abs` | `$math.abs( number )` |
| `pow` | `$math.pow( number, number )` |
| `rand` | `$math.random` |
| `round` | `$math.round( number )` |
| `sqrt` | `$math.sqrt( number )` |

### Requests

| Shortcut | Output |
| --- | --- |
| `param` | `$req.param( 'parameter' )` |

### Strings

| Shortcut | Output |
| --- | --- |
| `charAt` | `$string.charAt( string, index )` |
| `endsWith` | `$string.endsWith( string, suffix )` |
| `equals` | `$string.equals[IgnoreCase]( string )` |
| `hashCode` | `$string.hashCode( string )` |
| `indexOf` | `$string.indexOf( string, substring[, start] )` |
| `lastIndexOf` | `$string.lastIndexOf( string, substring[, start] )` |
| `length` | `$string.length( string )` |
| `removeSpaces` | `$string.removeSpaces( string )` |
| `replaceAll` | `$string.replaceAll( string, find, replace )` |
| `replaceFirst` | `$string.replaceFirst( string, find, replace )` |
| `splitOnRegex` | `$string.splitOnRegex( string, separatorRegex[, trimResults][, omitEmptyStrings] )` |
| `splitString` | `$string.splitString( string, separator[, trimResults][, omitEmptyStrings )` |
| `startsWith` | `$string.startsWith( string, prefix )` |
| `substring` | `$string.substring( string, start, end )` |
| `toLowerCase` | `$string.toLowerCase( string )` |
| `toUpperCase` | `$string.toUpperCase( string )` |
| `trim` | `$string.trim( string )` |

### SQL

>TODO: Do we use these? There are a couple examples in the docs...

### Utilities

| Shortcut | Output |
| --- | --- |
| `obj` | `$util.newObject` |
| `type` | `${util.type( object )}` |
| `className` | `${util.className( object )}` |
| `isNull` | `${util.isNull( object )}` |
