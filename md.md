# Markdown Language

This is me learning how to document stuff in markdown language. I started [here](https://www.markdownguide.org/getting-started/). This is pretty cool as I write it in **notead++**, I realize maybe the world is a *beautiful* place.
bold
: `**bold text**`
italic
: `*italic text*`
## block quotes

> this is a blockquote. maybe i can use this for code?
> 
> meanwhile,
>> this is a nested blockquote
>
> but really who needs all of that?

---

## lists

1. this
2. is
3. an
4. ordered
5. list
	1. of
	2. things
	3. you never
		- knew
		- you
		- needed
	4. to
	- know

---

## codeblocks
to make a code block, you indent 1 tab

	<html>
		<head><title>ho shuck</title></head>
		<body>
			<h1>whoda thunk?</h1>
		</body>
	</head>
	
### general code
encase generic code thats not a block in backtics.
this is some `code right here`
to escape back tics, use two. run ``echo whoami``

### extended codeblocks
you can use three backticks, \`\`\` or three tildes \~\~\~ on the first and last line of the block to avoid dealing with tabs

```
{
  "food": "tacos",
  "cost": 0.00,
  "when": 'NOW!'
}
```
---	

## images

put an exclamation point \! before square brackets with the alt text, and after, in parenthisis put the src

![tux the pengin](https://d33wubrfki0l68.cloudfront.net/e7ed9fe4bafe46e275c807d63591f85f9ab246ba/e2d28/assets/images/tux.png)

---

## links!
to make a link, you need some square brackets and some parenthasis and optionally some quotes to give it a mouse over title
example: 
> my favorite stock site is [finviz](https://www.finviz.com "a great place to viz some fin").

### quick links
just enclose in angle brackets
> my favorite crpyto site is by far <https://coinmarketcap.com>

---

## escaping characters
you can escape characters with a literal backslash. \\ this will escape all of the markdown special characters like \[ and \#

---

## extended markup
theres a slim chance that this will work, lets try it out!

### tables

| food | price |
| --- | --- |
| tacos | $0.00 |
| picadillo | $0.00 | 
| sashimi | $0.00 |

> theres some things money can buy, but for everything else, theres **crypto**

on the hrs of the headers, you can add colons \: to denominate the alignment. 

| places | rank | cost | 
| :--- | :---: | ---: |
| charlotte | 17 | $500 |
| costa rica | 3 | $1500 |
| sri lanka | 7 | $2200 |

### syntax highlighting on extended codeblocks.

earlier when i did the example of the codeblock with the json blob in it, it looked pretty bleh. lets add some pretty colors by adding the language declaration at the opening tag of the codeblock.

```json
{
  "food": "tacos",
  "cost": 0.00,
  "when": 'NOW!'
}
```

### strikethroughs
if you want to do a strikethrough, encapsulate with double tildes.

we all know that ~~james cameron~~ is the best director

### task lists
you can make check lists using markup. this would be extremely useful
- [x] this item is done
- [ ] this item is not
- [ ] neither is this item
- [x] but this item is done

### definition lists

To make a definition list, do the term on one line, and the next line, put a colon.

Food
: It's what you eat
Clothes
: They're what you wear
Places
: They're where you go.

### heading ids

#### making ids for your headings
to make ids for your headings you would use `{#custom-id}` at the end of the heading

####### custom heading {#custom-heading}

#### linking to custom headings
just make a link to that custom id like [this](#custom-heading "click here to find out more")