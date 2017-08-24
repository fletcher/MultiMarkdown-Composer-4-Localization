# MultiMarkdown Composer 4 Localization

## Introduction ##


MultiMarkdown Composer v4 makes use of the standard localization process for macOS apps.


Unfortunately, MultiMarkdown Composer isn't currently a "big" enough project to support a team of developers or pay lots of people to help.  This includes paying for professional localization of the application for all the countries in the world.

Fortunately, several kind people have volunteered to offer some help.  This project is an attempt to enable that.



## Instructions ##


The preferred way to contribute a localization is to use this project via git and GitHub.


1. Create a GitHub account and fork the Composer Localization repository

	<https://github.com/fletcher/MultiMarkdown-Composer-4-Localization>


2. Clone your fork to your machine:

		git clone https://github.com/<your user name here>/MultiMarkdown-Composer-4-Localization.git

3. Work on your translation (see below)

4. Create a new branch for your work, and submit a pull request for your changes



## Alternative Approach ##

If you're unfamiliar with git or GitHub, you can just email me the modified file and I'll submit to GitHub.  This will be a little bit slower, but still appreciated!!


1. Download the files from Github

	<https://github.com/fletcher/MultiMarkdown-Composer-4-Localization>

2. Work on your translation (see below)

3. Email me the file that you worked on and I'll incorporate the changes


## Translating an existing file ##

If someone has already started a language, e.g. `it.xliff`, then you can start editing it.  For example:

	<trans-unit id="5kV-Vb-QxS.title">
		<source>About MultiMarkdown Composer</source>
		<target>About MultiMarkdown Composer</target>
		<note>Class = "NSMenuItem"; title = "About MultiMarkdown Composer"; ObjectID = "5kV-Vb-QxS";</note>
	</trans-unit>


To translate this, you want to leave the `<source>...</source>` part alone --
that is the English for reference.  You want to make your changes to the
`<target>...</target>` part.

## Creating a new translation ##

If the language you want to work on doesn't exist, then copy an existing
translation and rename it using the standard 2 letter code for your language
(e.g. German = `de`).

Be sure to change *every* instance of `target-language="it"` in your file to
`target-language="de"` (for example).


## Prioritization ##

It may take a while to get everything translated. I would recommend starting with the most commonly used parts first.

1. Menu bars -- these are at the top under (`Main.storyboard`)

2. Preferences -- `Preferences.xib`

	* There are some preferences that are not actually available in the app --
	I needed them for testing.  Focus on strings that you actually see.
	Don't worry about the rest.

3. Don't worry about the rest (for now -- more to come).

