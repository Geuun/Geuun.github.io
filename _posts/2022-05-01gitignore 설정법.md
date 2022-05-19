<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>.gitignore 설정법</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	text-indent: -1.7em;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

.simple-table {
	margin-top: 1em;
	font-size: 0.875rem;
	empty-cells: show;
}
.simple-table td {
	height: 29px;
	min-width: 120px;
}

.simple-table th {
	height: 29px;
	min-width: 120px;
}

.simple-table-header-color {
	background: rgb(247, 246, 243);
	color: black;
}
.simple-table-header {
	font-weight: 500;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	max-height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, ui-serif, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK JP'; }
.pdf:lang(zh-CN) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC'; }
.pdf:lang(zh-TW) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK TC'; }
.pdf:lang(ko-KR) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK KR'; }
.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK JP'; }
.pdf:lang(zh-CN) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK SC'; }
.pdf:lang(zh-TW) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK TC'; }
.pdf:lang(ko-KR) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK KR'; }
.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.highlight-default {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.highlight-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.highlight-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.highlight-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.highlight-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.highlight-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.highlight-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.highlight-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.highlight-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.highlight-gray_background {
	background: rgba(241, 241, 239, 1);
}
.highlight-brown_background {
	background: rgba(244, 238, 238, 1);
}
.highlight-orange_background {
	background: rgba(251, 236, 221, 1);
}
.highlight-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.highlight-teal_background {
	background: rgba(237, 243, 236, 1);
}
.highlight-blue_background {
	background: rgba(231, 243, 248, 1);
}
.highlight-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.highlight-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.highlight-red_background {
	background: rgba(253, 235, 236, 1);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.block-color-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.block-color-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.block-color-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.block-color-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.block-color-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.block-color-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.block-color-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.block-color-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.block-color-gray_background {
	background: rgba(241, 241, 239, 1);
}
.block-color-brown_background {
	background: rgba(244, 238, 238, 1);
}
.block-color-orange_background {
	background: rgba(251, 236, 221, 1);
}
.block-color-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.block-color-teal_background {
	background: rgba(237, 243, 236, 1);
}
.block-color-blue_background {
	background: rgba(231, 243, 248, 1);
}
.block-color-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.block-color-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.block-color-red_background {
	background: rgba(253, 235, 236, 1);
}
.select-value-color-pink { background-color: rgba(245, 224, 233, 1); }
.select-value-color-purple { background-color: rgba(232, 222, 238, 1); }
.select-value-color-green { background-color: rgba(219, 237, 219, 1); }
.select-value-color-gray { background-color: rgba(227, 226, 224, 1); }
.select-value-color-opaquegray { background-color: rgba(255, 255, 255, 0.0375); }
.select-value-color-orange { background-color: rgba(250, 222, 201, 1); }
.select-value-color-brown { background-color: rgba(238, 224, 218, 1); }
.select-value-color-red { background-color: rgba(255, 226, 221, 1); }
.select-value-color-yellow { background-color: rgba(253, 236, 200, 1); }
.select-value-color-blue { background-color: rgba(211, 229, 239, 1); }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="7f5970ce-ad2d-4d51-a544-35de29bd4b1e" class="page sans"><header><div class="page-header-icon undefined"><span class="icon">😜</span></div><h1 class="page-title">.gitignore 설정법</h1><table class="properties"><tbody><tr class="property-row property-row-created_time"><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesCreatedAt"><path d="M7.01356 14.0001C8.8042 14.0001 10.5958 13.3107 11.9575 11.9324C14.681 9.21201 14.6808 4.7603 11.9571 2.04013C9.23336 -0.680043 4.77573 -0.680043 2.05199 2.04013C0.727519 3.36277 0 5.13301 0 6.99553C0 8.8764 0.727811 10.6285 2.05199 11.9509C3.43207 13.3106 5.22243 14.0001 7.01356 14.0001ZM3.72947 7.00914V8.461V8.65543H3.92382H5.34563H8.2794H8.4738V8.461V5.52541V3.37947V3.18502H8.2794H6.82747H6.63307V3.37947V6.81467H3.92382H3.72947V7.00914ZM1.83985 6.99553C1.83985 5.61698 2.38099 4.32597 3.36061 3.3477C5.36746 1.34337 8.64803 1.34062 10.6585 3.33944C10.6613 3.34219 10.6639 3.34494 10.6668 3.3477C12.676 5.3546 12.6763 8.63642 10.6668 10.6434C8.65705 12.6504 5.37031 12.6504 3.36061 10.6434C2.38099 9.66506 1.83985 8.37408 1.83985 6.99553Z"></path></svg></span>작성일시</th><td><time>@May 18, 2022 3:28 PM</time></td></tr><tr class="property-row property-row-last_edited_time"><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesCreatedAt"><path d="M7.01356 14.0001C8.8042 14.0001 10.5958 13.3107 11.9575 11.9324C14.681 9.21201 14.6808 4.7603 11.9571 2.04013C9.23336 -0.680043 4.77573 -0.680043 2.05199 2.04013C0.727519 3.36277 0 5.13301 0 6.99553C0 8.8764 0.727811 10.6285 2.05199 11.9509C3.43207 13.3106 5.22243 14.0001 7.01356 14.0001ZM3.72947 7.00914V8.461V8.65543H3.92382H5.34563H8.2794H8.4738V8.461V5.52541V3.37947V3.18502H8.2794H6.82747H6.63307V3.37947V6.81467H3.92382H3.72947V7.00914ZM1.83985 6.99553C1.83985 5.61698 2.38099 4.32597 3.36061 3.3477C5.36746 1.34337 8.64803 1.34062 10.6585 3.33944C10.6613 3.34219 10.6639 3.34494 10.6668 3.3477C12.676 5.3546 12.6763 8.63642 10.6668 10.6434C8.65705 12.6504 5.37031 12.6504 3.36061 10.6434C2.38099 9.66506 1.83985 8.37408 1.83985 6.99553Z"></path></svg></span>속성</th><td><time>@May 19, 2022 9:08 AM</time></td></tr><tr class="property-row property-row-select"><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesSelect"><path d="M7,13 C10.31348,13 13,10.31371 13,7 C13,3.68629 10.31348,1 7,1 C3.68652,1 1,3.68629 1,7 C1,10.31371 3.68652,13 7,13 Z M3.75098,5.32278 C3.64893,5.19142 3.74268,5 3.90869,5 L10.09131,5 C10.25732,5 10.35107,5.19142 10.24902,5.32278 L7.15771,9.29703 C7.07764,9.39998 6.92236,9.39998 6.84229,9.29703 L3.75098,5.32278 Z"></path></svg></span>For</th><td><span class="selected-value select-value-color-green">완료 🙌</span></td></tr><tr class="property-row property-row-url"><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesUrl"><path d="M3.73333,3.86667 L7.46667,3.86667 C8.49613,3.86667 9.33333,4.70387 9.33333,5.73333 C9.33333,6.7628 8.49613,7.6 7.46667,7.6 L6.53333,7.6 C6.01813,7.6 5.6,8.0186 5.6,8.53333 C5.6,9.04807 6.01813,9.46667 6.53333,9.46667 L7.46667,9.46667 C9.5284,9.46667 11.2,7.79507 11.2,5.73333 C11.2,3.6716 9.5284,2 7.46667,2 L3.73333,2 C1.6716,2 0,3.6716 0,5.73333 C0,7.124 0.762067,8.33453 1.88953,8.97713 C1.87553,8.83107 1.86667,8.6836 1.86667,8.53333 C1.86667,7.92013 1.98753,7.33447 2.2036,6.7978 C1.99267,6.4954 1.86667,6.12953 1.86667,5.73333 C1.86667,4.70387 2.70387,3.86667 3.73333,3.86667 Z M12.1095,5.28907 C12.1231,5.4356 12.1333,5.58307 12.1333,5.73333 C12.1333,6.34607 12.0101,6.9294 11.7931,7.46513 C12.0059,7.768 12.1333,8.13573 12.1333,8.53333 C12.1333,9.5628 11.2961,10.4 10.2667,10.4 L6.53333,10.4 C5.50387,10.4 4.66667,9.5628 4.66667,8.53333 C4.66667,7.50387 5.50387,6.66667 6.53333,6.66667 L7.46667,6.66667 C7.98187,6.66667 8.4,6.24807 8.4,5.73333 C8.4,5.2186 7.98187,4.8 7.46667,4.8 L6.53333,4.8 C4.4716,4.8 2.8,6.4716 2.8,8.53333 C2.8,10.59507 4.4716,12.2667 6.53333,12.2667 L10.2667,12.2667 C12.3284,12.2667 14,10.59507 14,8.53333 C14,7.14267 13.2375,5.93167 12.1095,5.28907 Z"></path></svg></span>참고자료_1</th><td></td></tr><tr class="property-row property-row-url"><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesUrl"><path d="M3.73333,3.86667 L7.46667,3.86667 C8.49613,3.86667 9.33333,4.70387 9.33333,5.73333 C9.33333,6.7628 8.49613,7.6 7.46667,7.6 L6.53333,7.6 C6.01813,7.6 5.6,8.0186 5.6,8.53333 C5.6,9.04807 6.01813,9.46667 6.53333,9.46667 L7.46667,9.46667 C9.5284,9.46667 11.2,7.79507 11.2,5.73333 C11.2,3.6716 9.5284,2 7.46667,2 L3.73333,2 C1.6716,2 0,3.6716 0,5.73333 C0,7.124 0.762067,8.33453 1.88953,8.97713 C1.87553,8.83107 1.86667,8.6836 1.86667,8.53333 C1.86667,7.92013 1.98753,7.33447 2.2036,6.7978 C1.99267,6.4954 1.86667,6.12953 1.86667,5.73333 C1.86667,4.70387 2.70387,3.86667 3.73333,3.86667 Z M12.1095,5.28907 C12.1231,5.4356 12.1333,5.58307 12.1333,5.73333 C12.1333,6.34607 12.0101,6.9294 11.7931,7.46513 C12.0059,7.768 12.1333,8.13573 12.1333,8.53333 C12.1333,9.5628 11.2961,10.4 10.2667,10.4 L6.53333,10.4 C5.50387,10.4 4.66667,9.5628 4.66667,8.53333 C4.66667,7.50387 5.50387,6.66667 6.53333,6.66667 L7.46667,6.66667 C7.98187,6.66667 8.4,6.24807 8.4,5.73333 C8.4,5.2186 7.98187,4.8 7.46667,4.8 L6.53333,4.8 C4.4716,4.8 2.8,6.4716 2.8,8.53333 C2.8,10.59507 4.4716,12.2667 6.53333,12.2667 L10.2667,12.2667 C12.3284,12.2667 14,10.59507 14,8.53333 C14,7.14267 13.2375,5.93167 12.1095,5.28907 Z"></path></svg></span>참고자료_2</th><td></td></tr><tr class="property-row property-row-select"><th><span class="icon property-icon"><svg viewBox="0 0 14 14" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0;-webkit-backface-visibility:hidden" class="typesSelect"><path d="M7,13 C10.31348,13 13,10.31371 13,7 C13,3.68629 10.31348,1 7,1 C3.68652,1 1,3.68629 1,7 C1,10.31371 3.68652,13 7,13 Z M3.75098,5.32278 C3.64893,5.19142 3.74268,5 3.90869,5 L10.09131,5 C10.25732,5 10.35107,5.19142 10.24902,5.32278 L7.15771,9.29703 C7.07764,9.39998 6.92236,9.39998 6.84229,9.29703 L3.75098,5.32278 Z"></path></svg></span>Tag</th><td><span class="selected-value select-value-color-orange">Blog</span></td></tr></tbody></table></header><div class="page-body"><h1 id="3c23f4de-445f-4f62-8fcb-149f1e600bb8" class="">목차</h1><ol type="1" id="373729ce-9c2b-4c23-980e-78023825852c" class="numbered-list" start="1"><li>.gitignore 이란?</li></ol><ol type="1" id="bbd4c234-8b71-499d-a20a-9446334ff1ee" class="numbered-list" start="2"><li>.gitignore 를 사용해야하는 이유는 무엇일까?</li></ol><ol type="1" id="29063bc6-3ead-44a4-848e-bc2cd6cccc76" class="numbered-list" start="3"><li>.gitignore File 생성 / 적용</li></ol><ol type="1" id="8f6b07c9-c275-49b0-8c37-ee75db19a3eb" class="numbered-list" start="4"><li>간단하게 .gitignore File 생성하는 방법<p id="16f086a8-36e5-4dc8-9437-ce15d63437fc" class="">
</p></li></ol><h3 id="44c68e35-88b7-4bec-ab03-c2769b7354ba" class="">1. .gitignore이란?</h3><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="473da42a-09b0-4821-9c08-c079abe603ff"><div style="font-size:1.5em"><span class="icon">📝</span></div><div style="width:100%"><code>.gitignore</code> 의 개념<ul id="6467eb62-bc33-4379-9412-298451964afc" class="bulleted-list"><li style="list-style-type:disc">프로젝트 작업시 로컬 환경의 정보나 빌드 정보등 원격 저장소에서 추적(Tracking) 하지 말아야되는 파일에 대해서 미리 List를 작성하고, Git이 List를 참고해서 추적하지 않도록 관리하는 파일</li></ul><ul id="890f05a3-3faa-454e-8691-53b8351c9829" class="bulleted-list"><li style="list-style-type:disc">git이 파일을 추적할 때, 어떤 파일이나 폴더 등을 추적하지 않도록 명시하기위해 작성하며, 해당 문서에 작성된 List는 수정사항이 발생해도 git이 무시하게된다.</li></ul><ul id="44633225-c7e3-4ec6-b828-a1303d10630a" class="bulleted-list"><li style="list-style-type:disc">특정 파일 확장자를 무시하거나 이름에 패턴이 존재하는 경우, 또는 특정 디렉토리 아래의 모든 파일을 무시할 수 있다.</li></ul></div></figure><h3 id="299221ec-f791-43a1-bd70-e957fdf293e2" class="">2. .gitignore 를 사용해야하는 이유는 무엇일까?</h3><ul id="1758e407-9501-4cd8-b769-a0d0dce62e2e" class="bulleted-list"><li style="list-style-type:disc">git을 활용해 여러사람과 협업을 진행하게되면 원격저장소에 관리하지 않아도 될 파일들이 올라가는 경우
(예로들면 jupyter notebook을 사용하면 자동으로 생성되는 .ipycheckpoint_checkpoints 등)</li></ul><ul id="0adade02-d97e-4eae-9f78-e7f8262b8e60" class="bulleted-list"><li style="list-style-type:disc">git을 활용해 여러사람과 협업을 진행 중 원격저장소에 올라가면 충돌이 일어날 수 있는 여지가 있는 파일들이 있는 경우</li></ul><ul id="d193d8b4-cec3-45e2-ae26-7767b3a3e6a4" class="bulleted-list"><li style="list-style-type:disc">원격저장소에 업로드하면 안되는 파일이 있을 때
(예로들면 django의 SECRETKEY가 포함된 settings.py File)</li></ul><p id="cbfe92f7-6b06-4a68-8c7d-d43214d95257" class="">즉, 간단하게 말하면 원격저장소에 올라가는 안되는 파일을 선택적으로 미리 List를 만들어 놓는것이다.</p><p id="45fd7112-f508-4e20-83f9-2dfa45afc587" class="">
</p><h3 id="99f6d5af-b7e1-4d6d-838b-2a297fbc76ef" class="">3. .gitignore File 생성</h3><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="d2541f06-f1a8-4dc4-8ca6-e519d6532e28"><div style="font-size:1.5em"><span class="icon">📝</span></div><div style="width:100%">작성방법<ul id="e92b572e-96b7-4e16-940b-b5849aaade0f" class="bulleted-list"><li style="list-style-type:disc">&#x27;#&#x27;로 시작하는 라인은 무시한다.</li></ul><ul id="2c2cb0c8-a0a2-4130-ac91-1090d83ec144" class="bulleted-list"><li style="list-style-type:disc">표준 Glob 패턴을 사용한다.</li></ul><ul id="16fff1bb-2405-4adf-8e6e-ec71e099dedf" class="bulleted-list"><li style="list-style-type:disc">슬래시(/)로 시작하면 하위 디렉터리에 적용되지(recursivity) 않는다.</li></ul><ul id="e34e0a64-4ad9-44ac-862b-46bde6e1e9c4" class="bulleted-list"><li style="list-style-type:disc">디렉터리는 슬래시(/)를 끝에 사용하는 것으로 표현한다.</li></ul><ul id="b663baf5-a56c-4d29-9e9d-672922aff0df" class="bulleted-list"><li style="list-style-type:disc">느낌표(!)로 시작하는 패턴의 파일은 무시하지 않는다.</li></ul><p id="7aab60e6-ee1f-4004-bc21-77cc426bf120" class="">참고문헌 : <a href="https://github.com/github/gitignore">Git 공식 github </a></p></div></figure><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="853be296-1b2f-451f-9877-b7273c13a2d2"><div style="font-size:1.5em"><span class="icon">✏️</span></div><div style="width:100%">Example<pre id="942d5da2-21fd-4c5f-8687-640656885310" class="code code-wrap"><code># ignore all .class files
*.class

# exclude lib.class from &quot;*.class&quot;, meaning all lib.class are still tracked
!lib.class

# ignore all json files whose name begin with &#x27;temp-&#x27;
temp-*.json

# only ignore the build.log file in current directory, not those in its subdirectories
/build.log

# specify a folder with slash in the end
# ignore all files in any directory named temp
temp/

# ignore doc/notes.txt, but not doc/server/arch.txt
bin/*.txt

# ignore all .pdf files in the doc/ directory and any of its subdirectories
# /** matches 0 or more directories
doc/**/*.pdf</code></pre></div></figure><p id="321bf13a-a23a-4007-9d4a-0de4f44850ed" class="">기본적인 .gitignore 파일을 작성했다면 Github 원격저장소에 적용해보도록하자.</p><h3 id="06c4253e-d64c-40ce-b348-6e57ecda7e40" class="">3-1. .gitignore 파일 적용</h3><p id="f5234f37-fac9-47da-b1bb-995b33af5bc0" class="">이미 원격저장소에 올라가있는 파일은 git 시스템에 의해 추적(Tracking) 당하고(🤔?) 있는 중이다.
이때는 아래의 코드를 입력해서 추적을 끊고 앞으로 추적 되지않도록 하자.</p><pre id="709d22c2-4828-4c16-9fd2-297bdbae9fbd" class="code"><code>$git rm -r --cached .
$git add. 
$git commit -m &quot;커밋메세지&quot;
$git push origin {브랜치명}</code></pre><p id="aa7104a8-ba17-464f-93e6-4cdc042890c3" class="">위 코드를 적용하면 원격저장소에서 .gitignore File List에 등록해둔 파일 또는 디렉토리가 사라진 것을 확인할 수 있을것이다.</p><p id="1475135a-d29f-43ad-922a-c49a430c702e" class="">
</p><h3 id="016f4a51-93a7-41c0-889f-373574f6692a" class="">4. 간단하게 .gitignore File 생성하는 방법</h3><p id="607d1a8f-0315-4ac6-a25f-1ef3779f4962" class="">일일히 .gitignore 파일을 작성하는 방법도 있겠지만 개발자들은 귀찮은걸 싫어한다.
따라서 당연히 자신의 개발환경을 입력하면 거기에 알맞는 .gitignore 파일을 생성해주는 사이트가 있다.</p><p id="86afc316-437d-4f9b-907b-8ac06cb480ec" class=""><a href="https://www.gitignore.io/">https://www.gitignore.io/</a> 에 접속해보자!
접속했다면 자신의 현재 개발환경에 알맞는 키워드를 입력하고 생성버튼을 눌러주면 알맞는 .gitignore 파일을 생성해준다!
</p><p id="97520d3a-a706-4823-bcf8-2cb3d8ba5e6e" class="">
</p><hr id="c9569b70-e723-4b71-b1c6-7f0c9a99197b"/><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="5efe83bf-f88b-4ba4-ac76-1ae35be107bd"><div style="font-size:1.5em"><span class="icon">✏️</span></div><div style="width:100%"><span style="border-bottom:0.05em solid"><strong>마무리하며</strong></span>
원격저장소를 혼자 사용한다면 .gitignore 파일을 사용하지 않아도 되지만,
자신이 여러사람과 협업하는 상황이라면 프로젝트 초반단계에 간단하게라도
.gitignore 파일을 생성해두면 불필요한 충돌상황을 피할 수 있을것 같다.  </div></figure></div></article></body></html>