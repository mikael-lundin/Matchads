# Matchads - Render template
Basic render template setup

```
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
		numberPerRow : '3',
		amount : '6',
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
| Item 						| Example						| Required		|
|---------------------------|-------------------------------|---------------|
| renderTemplateUrl			| 'http://cdn....Recs.html'		| Mandatory		|
| cxWidgetId				| 'bf8579f41d7feecff4....a0'	| Mandatory		|
| adId						| '0000000000005f5c'			| Mandatory		|
| insertBeforeElementId		| 'cx_demo'						| Mandatory		|
| width						| 980 / '100%'					| Mandatory		|
| height					| 0								| Mandatory		|
| margin					| 40							| Optional		|
| numberPerRow				| '3'							| Mandatory		|
| amount					| '6'							| Mandatory		|
| header					| 'Rekommenderat för dig'		| Optional		|
| headerFont				| 'bold 20px Roboto'			| Optional		|
| headerColor				| '#ff636e'						| Optional		|
| headerPadding				| '10px 0px 5px'				| Optional		|
| adInTextPosition			| 'true'						| Optional		|
| adTextColor				| '#FFF'						| Optional		|
| adBgColor					| '#ff636e'						| Optional		|
| font						| 'Arial'						| Optional		|
| positions					| ['1,3,5']						| Optional		|

