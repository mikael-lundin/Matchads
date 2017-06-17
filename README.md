# Matchads - Content 
## Basic template setup for content
In order to create new placements for Matchads you should place below ad-tag into the publishers website. Do note that some of these values are optional as seen below.

```html
<div id="cx_demo" style="display: none"></div>
<script type="text/javascript">

	var cX = cX || {};
	cX.callQueue = cX.callQueue || [];
	cX.callQueue.push(['insertWidget',{
		renderTemplateUrl : 'http://cdn.cxpublic.com/Matchads_Adnuntius_Recs.html',
		cxWidgetId : 'bf8579f41d7feecff4dd67c05e28ddb9d15e0ea0',
		adId : '0000000000005f5c',
		insertBeforeElementId : 'cx_demo',
		width: 980,
		height : 0,
		margin: 40,
		numberPerRow : 3,
		amount : 6,
		header : 'Rekommenderat för dig',
		headerFont : 'bold 20px Roboto',
		headerColor : '#ff636e',
		headerPadding : '10px 0px 5px',
		adInTextPosition: 'true',
		adTextColor: '#FFF',
		adBgColor: '#ff636e',
		font: 'Arial',
		positions : ['1,3,5'],
	}]);

</script>

<script type="text/javascript">
	(function(d,s,e,t){e=d.createElement(s);e.type="text/java"+s;e.async="async";
	e.src="http"+("https:"===location.protocol?"s://s":"://")+"cdn.cxense.com/cx.js";
	t=d.getElementsByTagName(s)[0];t.parentNode.insertBefore(e,t);})(document,"script");
</script>
```

The items in 'insertWidget' are bound to these values.

| Item 						| Example						| Required		| Type 			| Descrition
|:--------------------------|:------------------------------|:--------------|:--------------|:-------------
| renderTemplateUrl			| 'http://cdn....Recs.html'		| Mandatory		| String		| Url to Rendertemplate in Cxense. Do not change.
| cxWidgetId				| 'bf8579f41d7feecff4....a0'	| Mandatory		| String		| Id to Cxense Widget ID, change to the one you are referring to.
| adId						| '0000000000005f5c'			| Mandatory		| String		| Ad unit ID in Adnuntius
| insertBeforeElementId		| 'cx_demo'						| Mandatory		| String		| ID of div to place the ad at.
| width						| 980 / '100%'					| Mandatory		| Number/String	| Width of ad unit, if set to '100%' it will be responsive. Number will correlate to pixel value.
| height					| 0								| Mandatory		| Number 		| Should be set to 0
| margin					| 40							| Optional		| Number 		| Margin between items, will not work in responsive mode.
| numberPerRow				| 3								| Mandatory		| Number 		| Number of items within a row.
| amount					| 6								| Mandatory		| Number 		| Total amount of items in the widget. (Cannot be greater than set in Cxense Admin)
| header					| 'Rekommenderat för dig'		| Optional		| String		| Optional header text
| headerFont				| 'bold 20px Roboto'			| Optional		| String		| One line CSS for font styling.
| headerColor				| '#ff636e'						| Optional		| String		| Change color of header.
| headerPadding				| '10px 0px 5px'				| Optional		| String		| Padding for header
| adInTextPosition			| 'true'						| Optional		| String		| Moves ad marking below the image
| adTextColor				| '#FFF'						| Optional		| String		| Change color of ad marking text
| adBgColor					| '#ff636e'						| Optional		| String		| Change color of ad marking background
| font						| 'Arial'						| Optional		| String		| Change font for entire widget
| positions					| ['1,3,5']						| Optional		| Array			| Array to tell where to put the ads in widget. (one based index)


#Good to know
Programmatic
Responsive mode do not render programmatic ads well, move to pixel sized widget for that. When pixel dimensions are selected item size will be defaulted to 300x250 (Medium sized rectangle)

