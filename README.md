<html>
    <head>
        <!-- Maccy from themes.edada.ms -->
        <title>{Title}{block:PostSummary}, {PostSummary}{/block:PostSummary}</title>
        {block:Description}<meta name="description" value="{MetaDescription}" />{/block:Description}
        <link rel="shortcut icon" href="{Favicon}" />
        <link rel="alternate" type="application/rss+xml" href="{RSS}" />
        <meta http-equiv="Content-Type" value="text/html; charset=utf-8" />

        <meta name="color:Background" content="#888DC0" />
        <meta name="color:Link Color" content="#000000" />

        <meta name="image:Background" content="" />
        
        <meta name="if:Enable Infinite Scrolling" content="1" />
        <meta name="if:Background Image Cover" content="0" />
        <meta name="if:Display Captions" content="1" />
        <meta name="if:Display Description" content="1" />
        <meta name="if:Display Home Icon" content="1" />
        <meta name="if:Display Ask Icon" content="1" />
        <meta name="if:Display Submit Icon" content="1" />
        <meta name="if:Display Pages Icon" content="1" />
        <meta name="if:Display Archive Icon" content="1" />

        <style type="text/css">
           iframe#tumblr_controls {
                top: 20px !important;
            }
        
            body {
                background: {color:Background} url('{image:Background}') repeat fixed;
                {block:IfBackgroundImageCover}background-size: cover;{/block:IfBackgroundImageCover}
                padding: 0;
                margin: 0;
                height: 100%;  
                z-index: -1;
                font-family: 'Arial', sans-serif;
                font-size: 12px;
            }

            a {
                color: {color:Link Color};
                text-decoration: none;
            }
            
            a:hover {
                text-decoration: underline;
            }
            
            .menu_bar .left_corner, .menu_bar .apple_logo, .menu_bar .mac_logo, .menu_bar .right_corner, .icons .computer, .icons .info, .icons .folder, .icons .page, .icons .trash, .window .top, .window .bottom, .description .top, .description .bottom, .dock .left_corner, .dock .right_corner, .ok_button {
                background-image: url('http://static.tumblr.com/fpdiq1j/SbBm5x8aj/master_sprite.png');
                display: block;
                margin: auto;
            }
            
            .menu_bar {
                background: url('http://static.tumblr.com/fpdiq1j/R8am3tmz7/menu.png') repeat;
                height: 20px;
                position: fixed;
                top: 0;
                width: 100%;
                display: block;
                z-index: 5;
            }
            
            .menu_bar .left_corner {
                background-position: -97px -12px;
                height: 20px;
                width: 8px;
                top: 0;
                left: 0;
                position: absolute;
            }
            
            .menu_bar .right_corner {
                background-position: -105px -12px;
                height: 20px;
                width: 8px;
                top: 0;
                right: 0;
                position: absolute;
            }
            
            .menu_bar .apple_logo {
                background-position: 0px -18px;
                height: 14px;
                width: 11px;
                margin: 2px 0 0 17px;
                z-index: 2;
                float: left;
            }
            
            .menu_bar #nav .menu .name {
                margin: 0 0 0 10px;
                padding: 0 5px;
                float: left;
                font-size: 12px;
                line-height: 20px;
            }
            
            .tab_click {
                background-color: #00008B;
                color: white;
            }
            
            .menu_bar #nav .menu .dropdown {
                position: fixed;
                background-color: #D5D5D5;
                border-right: 1px solid rgba(0, 0, 0, 0.5);
                border-bottom: 1px solid rgba(0, 0, 0, 0.5);
                border-left: 1px solid rgba(0, 0, 0, 0.5);
                color: black;
                line-height: 17px;
                border-radius: 0px 0px 4px 4px;
                top: 20px;
                padding: 1px 5px;
                z-index: 6;
                margin: 0;
                list-style-type: none;
                display: none;
            }
            
            .menu a {
                color: black;
                text-decoration: none;
            }
            
            ul#nav, li.menu, ul.dropdown {
                padding: 0;
                margin: 0;
                display: inline;
                list-style-type: none;
            }
            
            .menu_bar .clock {
                float: right;
                margin: 0 15px 0 0;
                line-height: 20px;
            }
            
            .menu_bar .mac_logo {
               float: right;
               margin: 1px 15px 0 0;
               background-position: -81px -16px;
               width: 16px;
               height: 16px;
            }
            
            .icons {
                position: fixed;
                z-index: 1;
                top: 68px;
                right: 3%;
            }
            
            .icons .computer {
                background-position: -114px 0;
                height: 32px;
                width: 32px;
            }
            
            .icons .info {
                background-position: -146px 0;
                height: 32px;
                width: 32px;
            }
            
            .icons .folder {
                background-position: -178px 0;
                height: 32px;
                width: 30px;
            }
            
            .icons .page {
                background-position: -207px 0;
                height: 32px;
                width: 32px;
            }
            
            .icons .trash {
                background-position: -53px 0;
                height: 32px;
                width: 28px;
            }
            
            .icons .label {
                background-color: white;
                text-align: center;
                padding: 0 1px;
                font-size: 11px;
                margin: 4px 0 20px 0;
                max-width: 75px;
                width: 75px;
            }
            
            .navigation {
                position: relative;
                font-weight: bold;
                padding: 0 0 20px 0;
                height: 20px;
            }
            
            .navigation .next, .navigation .previous {
                padding: 3px 4px;
                background-color: #FFFFFF;
            }
            
            .navigation .next {
                float: right;
            }
            
            iframe[src="http://eathemes.tumblr.com/_iframe.html"] {
                top: 43px !important;
            }
            
            .description {
                position: fixed;
                top: 100px;
                left: 3%;
                z-index: 4;
                width: 255px;
            }
            
            .description .top {
                background-position: 0 -76px;
                width: 255px;
                height: 23px;
            }
            
            .description .middle {
                background: url('http://static.tumblr.com/fpdiq1j/lN6m5x85p/about_middle.png') repeat-y;
                width: 235px;
                padding: 0 10px 1px 10px;
            }
            
            .description .ok_button {
                background-position: -255px -76px;
                margin: 9px auto;
                width: 80px;
                height: 26px;
            }
            
            .description .bottom {
                background-position: 0px -99px;
                width: 255px;
                height: 8px;
            }
            
            .applications {
                width: 536px;
                margin: auto;
                z-index: 3;
                position: relative;
                top: 42px;
            }
            
            .window .top {
                background-position: 0px -32px;
                width: 536px;
                height: 22px;
            }
            
            .window .middle {
                background: url('http://static.tumblr.com/fpdiq1j/nZUm40uql/window_middle_smaller.png') repeat-y;
                max-width: 500px;
                width: 536px;
                padding: 4px 26px 4px 10px;
            }
            
            .window .bottom {
                background-position: 0px -54px;
                width: 536px;
                height: 22px;
                margin-bottom: 20px;
            }

            .window .bottom a {
                font-size: 11px;
                line-height: 16px;
                position: relative;
                left: 10px;
            }

            .dock .left_corner {
                background-position: -11px -27px;
                width: 5px;
                height: 5px;
                position: fixed;
                bottom: 0;
                left: 0;
                z-index: 5;
            }
            
            .dock .right_corner {
                background-position: -16px -27px;
                width: 5px;
                height: 5px;
                position: fixed;
                bottom: 0;
                right: 0;
                z-index: 5;
            }
            
            .caption {
                margin: 3px 0 0 0;
            }
            
            .title {
                font-size: 1.4em;
                margin: 0 0 3px 0;
            }
            
            .body .label {
                font-weight: bold;
            }
            
            .body img, .caption img, .description img {
                max-width: 100%;
                overflow: hidden;
            }
            
            .iab {
                display: block;
            }

            {block:IfNotDisplayCaptions}.caption{
                display:none;
            }{/block:IfNotDisplayCaptions}
            
            {block:IfNotDisplayDescription}.description{
                display:none;
            }{/block:IfNotDisplayDescription}

            {block:IfNotDisplayHomeIcon}.home{
                display:none;
            }{/block:IfNotDisplayHomeIcon}

            {block:IfNotDisplayAskIcon}.ask{
                display:none;
            }{/block:IfNotDisplayAskIcon}

            {block:IfNotDisplaySubmitIcon}.submit{
                display:none;
            }{/block:IfNotDisplaySubmitIcon}

            {block:IfNotDisplayPagesIcon}.pages{
                display:none;
            }{/block:IfNotDisplayPagesIcon}

            {block:IfNotDisplayArchiveIcon}.archive{
                display:none;
            }{/block:IfNotDisplayArchiveIcon}
            
            /* META */
            
            .meta .posted {
                margin-top: 10px;
                padding-top: 5px;
                border-top: 1px dashed rgba(0,0,0,0.5);
            }
            
			.meta .source, .meta .reblogged_from, .meta .tags {
				margin-top: 3px;
			}
            
            .meta .source, .meta .reblogged_from {
                font-size: 11px;
            }
            
			.meta .notes {
				margin-top: 10px;
			}
			
			ol.notes{
				margin: 0;
				padding: 0;
				list-style-type: none;
			}
			
			li.note.with_commentary {
				margin-bottom: 10px;
			}
			
			.notes span.action {
				vertical-align: 4px;
			}
            
            /* COMMON */
            
            blockquote {
                margin-left: 10px;
                padding-left: 10px;
                border-left: 2px solid rgba(0,0,0,0.50);
            }
            
            #infscr-loading {
                display: none !important;
                opacity: 0 !important;
                visibility: hidden !important;
                text-indent: -9999px;
            }
            
            .middle img {
                max-width: 100%;
            }
            
            .middle a img {
                border: 0;    
            }
            
            iframe.photoset {
                display: block;
            }
            
            .middle p:first-child, ul:first-child, ol:first-child, blockquote:first-child {
                margin-top: 0;
            }
            
            /*.middle p:only-child, ul:only-child, ol:only-child, blockquote:only-child {
                margin-top: 0;
                margin-bottom: 0;   
            }*/
            
            .middle p:last-child, ul:last-child, ol:last-child, blockquote:last-child {
                margin-bottom: 0;
            }
        
            {CustomCSS}
            
            /* CSS specific to the JS */
            
            #file_menu {
                left: 38px;
            }
            
            #edit_menu {
                left: 89px;
            }
            
            #filters_menu {
                left: 139px;
            }
            
            #options_menu {
                left: 193px;
            }
            
            .calculator {
                display: none;
                position: absolute;
                bottom: 50px;
                left: 3%;
            }
            
            .calculator .display {
                background-color: white;
                height: 16px;
                width: 80px;
                text-align: right;
                position: absolute;
                top: 28px;
                left: 10px;
                font-size: 10px;
            }
        </style>

        <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
        <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jqueryui/1.8/jquery-ui.min.js"></script>
        <script type="text/javascript" src="http://static.tumblr.com/fpdiq1j/v0umd2qzt/maccy.js"></script>
        <script type="text/javascript">
            var has_infinite_scrolling = {block:IfEnableInfiniteScrolling}true{/block:IfEnableInfiniteScrolling}{block:IfNotEnableInfiniteScrolling}false{/block:IfNotEnableInfiniteScrolling};
        </script>
    </head>
    <body>
        <div class="desktop">
            <div class="menu_bar">
                <div class="left_corner"></div>
                <a href="/">
					<span class="apple_logo"></span>
				</a>
                <ul id="nav">
                    <li class="menu">
					    <span class="name" id="file">
						    About
					    </span>
					    <ul class="dropdown" id="file_menu">
						    <li>Theme by</li>
						    <li><a href="http://edada.ms">Ed Adams</a><li>
						    <li>Art by</li>
						    <li><a href="http://apple.com">Apple</a></li>
                            <li>Powered by</li>
                            <li><a href="http://tumblr.com">Tumblr</a></li>
					    </ul>
                    </li>
                    <li class="menu">
					    <span class="name" id="edit">
						    Networks
					    </span>
                        <ul class="dropdown" id="edit_menu">
                            <li><a href="http://vue-network.tumblr.com/">Vue Network</a></li>
                            <li><a href="http://officialpalenetwork.weebly.com/">Official Pale Network</a></li>
                        </ul>
                    </li>
				    <li class="menu">
 					    <span class="name" id="filters">
						    Filters
					    </span>
                	    <ul class="dropdown" id="filters_menu">
						    <li id="filterText">Filter Text</li>
                    	    <li id="filterPhoto">Filter Photo</li>
                   		    <li id="filterPhotoset">Filter Photoset</li>
                  		    <li id="filterQuote">Filter Quote</li>
                 		    <li id="filterLink">Filter Link</li>
                  		    <li id="filterChat">Filter Chat</li>
                   		    <li id="filterAudio">Filter Audio</li>
                   		    <li id="filterVideo">Filter Video</li>
                            <li id="filterAsks">Filter Asks</li>
                   		    <li id="filterReset"><em>Reset</em></li>
                        </ul>
					</li>
                    <li class="menu">
    				    <span class="name" id="options">
						    Options
					    </span>
					    <ul class="dropdown" id="options_menu">
						    <li id="allowDragging">Allow Dragging</li>
						    <li id="doFullScreen">Enable Full Screen</li>
                            <li id="launchCalculator">Launch Calculator</li>
					    </ul>
                    </li>
				</ul>
                <span class="mac_logo"></span>
                <span class="clock" id="showClock">00:00 PM</span>
                <div class="right_corner"></div>
            </div>
            <div class="icons">
                <a href="/" class="home">
                    <div class="computer"></div>
                    <div class="label">{Title}</div>
                </a>

                {block:AskEnabled}
                    <a href="/ask" class="ask">
                        <div class="info"></div>
                        <div class="label">{AskLabel}</div>
                    </a>
                {/block:AskEnabled}
                
                {block:SubmissionsEnabled}
                    <a href="/submit" class="submit">
                        <div class="folder"></div>
                        <div class="label">{SubmitLabel}</div>
                    </a>
                {/block:SubmissionsEnabled}
                
                {block:HasPages}
                    {block:Pages}
                        <a href="{URL}" class="pages">
                            <div class="page"></div>
                            <div class="label">{Label}</div>
                        </a>
                    {/block:Pages}
                {/block:HasPages}
                
                <a href="/archive" class="archive">
                    <div class="trash"></div>
                    <div class="label">Archive</div>
                </a>
            </div>
            <div class="calculator"><img src="http://static.tumblr.com/fpdiq1j/T0Am4qtp9/calculator.png" /><div class="display"></div></div>
            {block:Description}
                <div class="description">
                    <div class="top"></div>
                    <div class="middle">
                        {Description}
                        <div class="ok_button" id="closeDescription"></div>
                    </div>
                    <div class="bottom"></div>
                </div>
            {/block:Description}
            <div class="applications" style="position: relative;
left: 45px;">
                {block:Posts}
					<div class="window type_{PostType}{block:Photoset}set{/block:Photoset}" id="{PostID}">
                    	<div class="top"></div>
	                    <div class="middle">
	                       {block:Text}
	                            {block:Title}
	                                <div class="title">
	                                    {Title}
	                                </div>
	                            {/block:Title}
	                            <div class="body">
	                                {Body}
	                            </div>
	                        {/block:Text}

	                        {block:Photo}
	                            <img class="iab" src="{PhotoURL-250}" alt="{PhotoAlt}" />
	                            {block:Caption}
	                                <div class="caption">
	                                    {Caption}
	                                </div>
	                            {/block:Caption}
	                        {/block:Photo}

	                        {block:Photoset}
	                            {Photoset-500}
	                                {block:Caption}
	                                    <div class="caption">
	                                        {Caption}
	                                    </div>
	                                {/block:Caption}
	                            {/block:Photoset}

	                            {block:Quote}
	                                <div class="title">
	                                    "{Quote}"
	                                </div>
	                                {block:Source}
	                                    <div class="body">
	                                        &mdash; {Source}
	                                    </div>
	                                {/block:Source}
	                            {/block:Quote}

	                            {block:Link}
	                                <a href="{URL}" class="title" {Target}>{Name} »</a>
	                                {block:Description}
	                                    <div class="body">
	                                        {Description}
	                                    </div>
	                                {/block:Description}
	                            {/block:Link}

	                            {block:Chat}
	                                {block:Title}
	                                    <div class="title">{Title}
	                                {/block:Title}
	                                {block:Lines}
	                                    <div class="body">
	                                        {block:Label}
	                                            <span class="label">{Label}</span>
	                                        {/block:Label}
	                                        {Line}
	                                    </div>
	                                {/block:Lines}
	                            {/block:Chat}

	                            {block:Video}
	                            {Video-500}
	                                {block:Caption}
	                                    <div class="caption">
	                                        {Caption}
	                                    </div>
	                                {/block:Caption}
	                            {/block:Video}

	                            {block:Audio}
	                                {AudioPlayerBlack}
	                                {block:Caption}
	                                    <div class="body">
	                                        {Caption}
	                                    </div>
	                                {/block:Caption}
	                            {/block:Audio}
                                {block:PermalinkPage}{block:Date}
	                                <div class="meta" style="display: block;">
    						            <div class="posted">
								            Posted: {DayOfWeek} {DayOfMonth}{DayOfMonthSuffix} {Month} at {12Hour}:{Minutes}{AmPm}
							            </div>
							            {block:HasTags}
								            <div class="tags">
									            Tagged: {block:Tags}<a href="{TagURL}">#{Tag}</a> {/block:Tags}
								            </div>
							            {/block:HasTags}
							            {block:ContentSource}
							            	<div class="source">
									            Source: <a href="{SourceURL}">{SourceTitle}</a>
								            </div>
								            {block:RebloggedFrom}
									            <div class="reblogged_from">
										            Reblogged From: <a href="{ReblogParentURL}">{ReblogParentName}</a>
									            </div>
								            {/block:RebloggedFrom}
							            {/block:ContentSource}
							            {block:PostNotes}
								            <div class="notes">
								            	{PostNotes}
								            </div>
							            {/block:PostNotes}
						            </div>
	                            {/block:Date}{/block:PermalinkPage}
	                        </div>
	                    <div class="bottom" style="float: none; clear: both;">
	                        {block:Date}
	                            <a href="{Permalink}">
	                                Posted on {DayOfMonth}{DayOfMonthSuffix} {ShortMonth} at {12Hour}:{Minutes} {CapitalAmPm}{block:NoteCount}, with {NoteCountWithLabel}{/block:NoteCount}
	                            </a>
	                        {/block:Date}
	                    </div>
                	</div>
				{/block:Posts}
                {block:Pagination}
                    <div class="navigation">
                        {block:NextPage}
                            <a class="next" href="{NextPage}">{lang:Next} &rarr;</a>
                        {/block:NextPage}
                        {block:PreviousPage}
                            <a class="previous" href="{PreviousPage}">&larr; {lang:Previous}</a>
                        {/block:PreviousPage}
                    </div>
                {/block:Pagination}
            </div>
            <div class="dock">
                <div class="left_corner"></div>
                <div class="right_corner"></div>
            </div>
        </div>
        <script src='http://dl.dropbox.com/u/16697297/j_k_post_navigation_v2.js'></script>
    </body>
</html>
