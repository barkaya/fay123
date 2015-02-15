<head><center><script type=”text/javascript” src=”http://proto.jp/js/tumblrAutoPager.js”></script><center><!-- DEFAULT VARIABLES -->
<meta name="color:background" content="#FAFAFA" />
<meta name="color:text" content="#C7C7C7" />
<meta name="color:link" content="#aaaaaa" />
<meta name="font:blog title" content="arial black" />
<meta name="font:body" content="arial" />
<meta name="if:Show Notes" content="0"/>
<title>{Title}</title>
<link rel="shortcut icon" href="{Favicon}">
<link rel="alternate" type="application/rss+xml" href="{RSS}">
{block:Description}<meta name="description" content="{MetaDescription}" />{/block:Description}

<style type="text/css">
small{font-size:100%;}
body{
text-align:justify;
color:{color:text}; 
font-size: 9px; font-family: {font:body};
line-height:100%; 
background:{color:background}; 
}
a:link, a:visited, a:active{color:{color:link}; text-decoration:none; outline: none; -moz-outline-style: none;}
a:hover{color:{color:text}; outline: none;-moz-outline-style: none;}
.label {font-weight:bold;}
ul.chat, .chat ol, .chat li {list-style:none; margin:0px; padding:0px;}
blockquote{padding:0px; padding-left:5px; margin:5px; border-left:1px dotted {color:text};}
blockquote img{display:block;}
blockquote p{padding:0px; margin:0px;}
blockquote blockquote{position:relative; left:-5px; margin-top:0px; margin-right:0px; padding-right:0px;}
a img{border;none;}
img{border:none; -webkit-transition: opacity 0.5s linear; opacity: 0.70;}
img:hover{-webkit-transition: opacity 0.5s linear; opacity: 1;}
#center{width:500px; padding-bottom:5px; margin:auto;}
#entry{width:500px; padding-top:5px; padding-bottom:5px; border-bottom:1px dotted {color:text};}
#perma{width:500px; padding-top:5px; padding-bottom:5px; padding-left:5px; padding-right:5px; margin-bottom:10px;}
.title{font-size:11px; letter-spacing:1px; text-transform:uppercase; text-align:left;}
.src{text-align:right; margin-top:3px;}
.cap{margin-bottom:-5px;}
.date{margin-bottom:5px; font-size:10px;}
.blog{margin-top:5px; margin-bottom:2px; font-family:{font:blog title}; font-size:20px; letter-spacing:1px; text-transform:uppercase; text-align:left;}
#footer{margin-top:5px; width:500px; padding-top:5px; padding-bottom:5px;}

{CustomCSS}
</style>
</center>
<script type=”text/javascript” src=”http://proto.jp/js/tumblrAutoPager.js”></script>
<script type="text/javascript" src="http://codysherman.com/tools/infinite-scrolling/code"></script>
</center>
</head>
<body>
<center>
<div id="center">

<div> 
<div id="entry"><a href="/"><div class="blog"><center>{Title}</center></div></a>{Description}</div> 
</div>

<Div class = "autopagerize_page_element"> <!-- infinitescroll BINGO! THE PART YOU NEED!-->
{block:Posts}
<div>

<div id="entry">

{block:Date}<div class="date"><a href="{Permalink}">{TimeAgo} {block:IfShowNotes}{block:NoteCount}with {NoteCount} notes {/block:NoteCount}{/block:IfShowNotes} </a></div>{/block:Date}

<center>
<div> 

{block:Text} 
{block:Title}<center><div class="title">{Title}</div></center>{/block:Title}{Body}
{/block:Text} 
</div>
</center>

<div>

{block:Photo} 
{LinkOpenTag}<img src="{PhotoURL-500}">{LinkCloseTag}{block:Caption}<div class="cap"></div>{/block:Caption}
{/block:Photo} 
</div>

<div>

{block:Photoset}
{Photoset-500}{block:Caption}<div class="cap">{Caption}</div>{/block:Caption}
{/block:Photoset}
</div>

<div>

{block:Quote} 
<div class="title">{Quote}</div>{block:Source}<div class="src">{Source}</div>{/block:Source}
{/block:Quote} 
</div>

<div>

{block:Link} 
<div class="title"><a href="{URL}" {Target}>{Name}</a></div>{block:Description}{Description}{/block:Description} 
{/block:Link} 
</div>

<div>

{block:Chat} 
{block:Title}<div class="title">{Title}</div>{/block:Title}
<ul class="chat">{block:Lines}<li class="{Alt} user_{UserNumber}">{block:Label}<span class="label">{Label}</span>{/block:Label}{Line}</li>{/block:Lines}</ul>
{/block:Chat}
</div>

<div>

{block:Audio} 
{AudioPlayerWhite}{block:Caption}{Caption}{/block:Caption}
{/block:Audio} 
</div>

<div>

{block:Video} 
{Video-500}{block:Caption}<div class="cap">{Caption}</div>{/block:Caption}
{/block:Video} 
</div>

<div>

{block:Answer} 
<i>{Asker}: {Question}</i><br>{Answer}
{/block:Answer} 
</div>
</div>

{/block:Posts}
</div> <!-- infinitescroll THE /DIV YOU NEED TO ADD TO FINISH THE "autopagerize_page_element" PART-->
</div>

<div class="pre_footer">
<right>
	 {block:PermalinkPagination} 
		{block:PreviousPost}<a href="{PreviousPost}">Previous Post</a>    
		{/block:PreviousPost} 
		{block:NextPost}<a href="{NextPost}">Next Post</a>
		{/block:NextPost}
	 {/block:PermalinkPagination}
	 {block:DayPagination}
		 {block:PreviousDayPage}<a href="{PreviousDayPage}">< {ShortDayOfWeek}, {ShortMonth} {DayOfMonth}{DayOfMonthSuffix}</a>
		 {/block:PreviousDayPage}    
		 {block:NextDayPage}<a href="{NextDayPage}">{ShortDayOfWeek}, {ShortMonth} {DayOfMonth}{DayOfMonthSuffix} ></a>
		 {/block:NextDayPage}
	 {/block:DayPagination}<br />
	</right>
	</div>  

</div>
</center>
</body>
</html>

? THIS THEME FOR TUMBLR MADE BY ? ILYABARKAYA ? http://barkaya.tumblr.com/ ?
