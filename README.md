# Browser Bible 

A browser based Bible Study Application built with the holy trinity of HTML, CSS, and JavaScript.

* Created by: [http://www.dbsbible.org](Digital Bible Society)
* Project Leader: John Dyer [http://j.hn/](http://j.hn/)
* Code License: GPLv2/MIT
* Content License: See each content folder for a license

## Goals

HTML and JavaScript based Bible software that can run

* on any browser
* on any device
* in any nation

The application has full search and highlighting features but requires

* no install
* no server
* no trace

### Mobile Version

The mobile version uses [http://www.jquerymobile.com/](jQuery Mobile) to navigate through the Bible chapter by chapter

### Desktop Version

The desktop version is a multipane application based off ideas at [http://biblewebapp.com/](http://biblewebapp.com/)

## File Formats

Each Bible lives in the `/content/bibles/` directory in a folder named for it's language and name (such as `en_kjv` for English King James Version)

### Header

The document opens with links to core JavaScript and CSS files and basic navigation in the `<body>`

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<title>Isaiah 64 (KJV)</title>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
	<script src="../../../js/mobile.js"></script>
	<link href="../../../css/mobile.css" rel="stylesheet" />
</head>
<body>
<div data-role="page">
	<div data-role="header">
		<a href="Isa.63.html" data-icon="arrow-l">Isa 63</a>
		<h1>Isaiah 64 (KJV)</h1>
		<a href="Isa.65.html" data-icon="arrow-r">Isa 65</a>
	</div>
	<div data-role="content">
```


### Content

In the middle is HTML marking up the chapter and each verse number

```html
<div class="chapter version-kjv" data-osis="Isa.64" dir="ltr" lang="en">
	<h2 class="chapter-num">64</h2>
	<p>
	<span class="verse" data-osis="Isa.64.1"><span class="verse-num verse-1">1&nbsp;</span><span class="word" data-lemma="strong:H3863">Oh</span> <span class="word" data-lemma="strong:H7167">that thou wouldest rend</span> <span class="word" data-lemma="strong:H8064">the heavens</span> <span class="word" data-lemma="strong:H3381">that thou wouldest come down</span> <span class="word" data-lemma="strong:H2022">that the mountains</span> <span class="word" data-lemma="strong:H2151">might flow down</span> <span class="word" data-lemma="strong:H6440">at thy presence</span> </span>
	<span class="verse" data-osis="Isa.64.2"><span class="verse-num">2&nbsp;</span><span class="word" data-lemma="strong:H2003">the melting</span> <span class="word" data-lemma="strong:H0784">fire</span> <span class="word" data-lemma="strong:H6919">burneth</span> <span class="word" data-lemma="strong:H0784">the fire</span> <span class="word" data-lemma="strong:H4325">causeth the waters</span> <span class="word" data-lemma="strong:H1158">to boil</span> <span class="word" data-lemma="strong:H8034">to make thy name</span> <span class="word" data-lemma="strong:H3045">known</span> <span class="word" data-lemma="strong:H6862">to thine adversaries</span> <span class="word" data-lemma="strong:H1471">the nations</span> <span class="word" data-lemma="strong:H7264">may tremble</span> <span class="word" data-lemma="strong:H6440">at thy presence</span> </span>
	<span class="verse" data-osis="Isa.64.3"><span class="verse-num">3&nbsp;</span><span class="word" data-lemma="strong:H6213">When thou didst</span> <span class="word" data-lemma="strong:H3372">terrible things</span> <span class="word" data-lemma="strong:H6960">we looked</span> <span class="word" data-lemma="strong:H3381">not for, thou camest down</span> <span class="word" data-lemma="strong:H2022">the mountains</span> <span class="word" data-lemma="strong:H2151">flowed down</span> <span class="word" data-lemma="strong:H6440">at thy presence</span> </span>
	<span class="verse" data-osis="Isa.64.4"><span class="verse-num">4&nbsp;</span><span class="word" data-lemma="strong:H5769">For since the beginning of the world</span> <span class="word" data-lemma="strong:H8085">have not heard</span> <span class="word" data-lemma="strong:H0238">nor perceived by the ear</span> <span class="word" data-lemma="strong:H5869">neither hath the eye</span> <span class="word" data-lemma="strong:H7200">seen</span> <span class="word" data-lemma="strong:H0430">O God</span> <span class="word" data-lemma="strong:H2108">beside</span> <span class="word" data-lemma="strong:H6213">he hath prepared</span> <span class="word" data-lemma="strong:H2442">for him that waiteth</span> </span>
	<span class="verse" data-osis="Isa.64.5"><span class="verse-num">5&nbsp;</span><span class="word" data-lemma="strong:H6293">Thou meetest</span> <span class="word" data-lemma="strong:H7797">him that rejoiceth</span> <span class="word" data-lemma="strong:H6213">and worketh</span> <span class="word" data-lemma="strong:H6664">righteousness</span> <span class="word" data-lemma="strong:H2142">remember</span> <span class="word" data-lemma="strong:H1870">thee in thy ways</span> <span class="word" data-lemma="strong:H7107">behold, thou art wroth</span> <span class="word" data-lemma="strong:H2398">for we have sinned</span> <span class="word" data-lemma="strong:H5769">in those is continuance</span> <span class="word" data-lemma="strong:H3467">and we shall be saved</span> </span>
	</p>
	<p>
	<span class="verse" data-osis="Isa.64.6"><span class="verse-num">6&nbsp;</span><span class="word" data-lemma="strong:H2931">But we are all as an unclean</span> <span class="word" data-lemma="strong:H6666">and all our righteousnesses</span> <span class="word" data-lemma="strong:H5708">as filthy</span> <span class="word" data-lemma="strong:H0899">rags</span> <span class="word" data-lemma="strong:H1101">and we all do fade</span> <span class="word" data-lemma="strong:H5929">as a leaf</span> <span class="word" data-lemma="strong:H5771">and our iniquities</span> <span class="word" data-lemma="strong:H7307">like the wind</span> <span class="word" data-lemma="strong:H5375">have taken us away</span> </span>
	<span class="verse" data-osis="Isa.64.7"><span class="verse-num">7&nbsp;</span><span class="word" data-lemma="strong:H7121">none that calleth</span> <span class="word" data-lemma="strong:H8034">upon thy name</span> <span class="word" data-lemma="strong:H5782">that stirreth up</span> <span class="word" data-lemma="strong:H2388">himself to take hold</span> <span class="word" data-lemma="strong:H5641">of thee: for thou hast hid</span> <span class="word" data-lemma="strong:H6440">thy face</span> <span class="word" data-lemma="strong:H4127">from us, and hast consumed</span> <span class="word" data-lemma="strong:H3027">us, because</span> <span class="word" data-lemma="strong:H5771">of our iniquities</span> </span>
	<span class="verse" data-osis="Isa.64.8"><span class="verse-num">8&nbsp;</span><span class="word" data-lemma="strong:H0001">our father</span> <span class="word" data-lemma="strong:H2563">the clay</span> <span class="word" data-lemma="strong:H3335">and thou our potter</span> <span class="word" data-lemma="strong:H4639">the work</span> <span class="word" data-lemma="strong:H3027">of thy hand</span> </span>
	</p>
	<p>	
	<span class="verse" data-osis="Isa.64.9"><span class="verse-num">9&nbsp;</span><span class="word" data-lemma="strong:H7107">Be not wroth</span> <span class="word" data-lemma="strong:H3966">very sore</span> <span class="word" data-lemma="strong:H2142">neither remember</span> <span class="word" data-lemma="strong:H5771">iniquity</span> <span class="word" data-lemma="strong:H5703">for ever</span> <span class="word" data-lemma="strong:H5027">behold, see</span> <span class="word" data-lemma="strong:H5971">all thy people</span> </span>
	<span class="verse" data-osis="Isa.64.10"><span class="verse-num">10&nbsp;</span><span class="word" data-lemma="strong:H6944">Thy holy</span> <span class="word" data-lemma="strong:H5892">cities</span> <span class="word" data-lemma="strong:H4057">are a wilderness</span> <span class="word" data-lemma="strong:H6726">Zion</span> <span class="word" data-lemma="strong:H4057">is a wilderness</span> <span class="word" data-lemma="strong:H3389">Jerusalem</span> <span class="word" data-lemma="strong:H8077">a desolation</span> </span>
	<span class="verse" data-osis="Isa.64.11"><span class="verse-num">11&nbsp;</span><span class="word" data-lemma="strong:H6944">Our holy</span> <span class="word" data-lemma="strong:H8597">and our beautiful</span> <span class="word" data-lemma="strong:H1004">house</span> <span class="word" data-lemma="strong:H0001">where our fathers</span> <span class="word" data-lemma="strong:H1984">praised</span> <span class="word" data-lemma="strong:H8316">thee, is burned up</span> <span class="word" data-lemma="strong:H0784">with fire</span> <span class="word" data-lemma="strong:H4261">and all our pleasant things</span> <span class="word" data-lemma="strong:H2723">are laid waste</span> </span>
	<span class="verse" data-osis="Isa.64.12"><span class="verse-num">12&nbsp;</span><span class="word" data-lemma="strong:H0662">Wilt thou refrain</span> <span class="word" data-lemma="strong:H2814">wilt thou hold thy peace</span> <span class="word" data-lemma="strong:H6031">and afflict</span> <span class="word" data-lemma="strong:H3966">us very sore</span> </span>
	</p>
</div>
```

### Footer

The document closes with links a second set of navigation basic navigation in the `<body>`

```html
	</div>
	<div data-role="footer">	
		<div data-role="navbar">
			<ul>
				<li><a href="Isa.63.html" data-icon="arrow-l">Isa 63</a></li>
				<li><a href="index.html" data-icon="home">Books</a></li>
				<li><a href="Isa.65.html" data-icon="arrow-r">Isa 65</a></li>
			</ul>
		</div>
	</div>

</div>
</body>
</html>
```

## v0.1 Todo List

* index.html, about.html for all languages/versions

## 0.2 Todo List

* Store user preferences
* Chapter/verse Navigation Dropdown
* Add/delete columns
* Put version info into version.json within folder, then load dynamically
* handle missing books (e.g. Psalms and NT)
* handle apocrypha
* Allow version to switch if a book is missing (WLC -> tisch is hardcoded)
* Build NASB importer

## 0.3 Todo List

* Add Audio player
* Add video launcher
* Add maps/images links
* Add original language tools (highlighting tense/voice/freq)
* Change theme colors
* Change font size within the reader

## Done

* Footnotes now display in the footer
* about.html page for each version (loads with 'i' button)
* Switched from `v001001001` to OSIS style `Gen.1.1`
* Rebuilt exporters for OSIS/XML, USMF, Unbound.
* Build search into application
* Build WLC, Tischendorf importers

## Known Issues

* Notes and CF needs work
* OSIS quotes span over verses
* USMF doesn't handle quote lines (OEB, WEB)