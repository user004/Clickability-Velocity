# Clickability Velocity

Based on [jampow's Velocty package](https://github.com/jampow/velocity-sublime), but modified to use [Clickability](http://www.clickability.com/)'s custom functions and version of Velocity. Somewhat built using the Template Language Reference Guide.

Less/Greater than means `<optional>`

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
| `content` | `$cms.content<( id )>` |
| `link` | `$cms.link<( <name/path><, index> )>` |
| `links` | `$cms.links<( <name/path><, index><, size> )>` |
| `flinks` | `$cms.filteredLinks( type<, name/path><, index><, size> )` |
| `clinks` | `$cms.categorizedLinks( categorization, 'name/path', index, size )` |
| `cat` | `$cms.getCategorization( [ 'sets' ], [ 'categories' ]<, match all> )` |
| `wss` | `$cms.websiteSection<( name/path/id )>` |
| `parent` | `cms.parent<( name/path/object )>` |
| `template` | `$cms.template( name )` |
| `include` | `$cms.include( name )` |

### Media

| Shortcut | Output |
| --- | --- |
| `media` | `$cms.media( name/id<, type> )` |
| `tag` | `$util.tag( media<, show attributes><, extra info> )` |
| `linkedTag` | `$util.linkedTag( media<, show attributes><, extra info> )` |
| `unlinkedTag` | `$util.unlinkedTag( media<, show attributes><, extra info> )` |
| `resizeImageTag` | `$util.resizeImageTag( media<, percent/width><, height><, show attributes><, extra info> )` |
| `unlinkedResizeImageTag` | `$util.unlinkedResizeImageTag( media<, percent/width><, height><, show attributes><, extra info> )` |

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
| `end` | `#end##` |

`for`:
```
#foreach( item in itemList )##
	## statement
#end##
```

`if`:
```
#if( condition )##
	## statement
#end##
```

`else`:
```
#else<if( condition )>##
	## statement
```

### HashMaps

| Shortcut | Output |
| --- | --- |
| `hm` | `$util.newHashMap` |

### Helpers

| Shortcut | Output |
| --- | --- |
| `$` | `$<!>{variable}` |
| `vc` | `$velocityCount` |

`#*`:
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
| `param` | `$req.param( parameter )` |

### Strings

| Shortcut | Output |
| --- | --- |
| `charAt` | `$string.charAt( string, index )` |
| `endsWith` | `$string.endsWith( string, suffix )` |
| `equals` | `$string.equals<IgnoreCase>( string )` |
| `hashCode` | `$string.hashCode( string )` |
| `indexOf` | `$string.indexOf( string, substring<, start> )` |
| `lastIndexOf` | `$string.lastIndexOf( string, substring<, start> )` |
| `length` | `$string.length( string )` |
| `removeSpaces` | `$string.removeSpaces( string )` |
| `replaceAll` | `$string.replaceAll( string, find, replace )` |
| `replaceFirst` | `$string.replaceFirst( string, find, replace )` |
| `splitOnRegex` | `$string.splitOnRegex( string, separatorRegex<, trimResults><, omitEmptyStrings> )` |
| `splitString` | `$string.splitString( string, separator<, trimResults><, omitEmptyStrings> )` |
| `startsWith` | `$string.startsWith( string, prefix )` |
| `substring` | `$string.substring( string, start, end )` |
| `toLowerCase` | `$string.toLowerCase( string )` |
| `toUpperCase` | `$string.toUpperCase( string )` |
| `trim` | `$string.trim( string )` |

### Utilities

| Shortcut | Output |
| --- | --- |
| `obj` | `$util.newObject` |
| `type` | `$util.type( object )` |
| `className` | `$util.className( object )` |
| `isNull` | `$util.isNull( object )` |

### Debugging

| Shortcut | Output |
| --- | --- |
| `log` | `$codeDebug.log( string )` |
| `watchpoint` | `$codeDebug.watchpoint<( string/arrayList )>` |
