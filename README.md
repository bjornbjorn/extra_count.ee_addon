Extra Count
====================

{count} being overridden within a tag? Not any more - with the AWESOME POWER of {extra:count} !!

Extra Count will add a variable called {extra:count} to all {exp:channel:entries} tags that hopefully won't be overridden.

Fixes this problem:

```
{exp:ee_addon:tag}

	{exp:channel:entries channel="blog" limit="10"}
		Oh no {count} is always 1 due to EE's template parser! .. {extra:count} to the rescue :-)
	{/exp:channel:entries}

{/exp:ee_addon:tag}

```