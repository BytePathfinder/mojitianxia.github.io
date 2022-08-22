<!doctype html>
<html>

<head>
    <meta charset='UTF-8'>
    <meta name='viewport' content='width=device-width initial-scale=1'>

    <link href='https://fonts.loli.net/css?family=Open+Sans:400italic,700italic,700,400&subset=latin,latin-ext'
        rel='stylesheet' type='text/css' />
    <style type='text/css'>
        html {
            overflow-x: initial !important;
        }

        :root {
            --bg-color: #ffffff;
            --text-color: #333333;
            --select-text-bg-color: #B5D6FC;
            --select-text-font-color: auto;
            --monospace: "Lucida Console", Consolas, "Courier", monospace;
            --title-bar-height: 20px;
        }

        .mac-os-11 {
            --title-bar-height: 28px;
        }

        html {
            font-size: 14px;
            background-color: var(--bg-color);
            color: var(--text-color);
            font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
            -webkit-font-smoothing: antialiased;
        }

        body {
            margin: 0px;
            padding: 0px;
            height: auto;
            inset: 0px;
            font-size: 1rem;
            line-height: 1.42857;
            overflow-x: hidden;
            background: inherit;
            tab-size: 4;
        }

        iframe {
            margin: auto;
        }

        a.url {
            word-break: break-all;
        }

        a:active,
        a:hover {
            outline: 0px;
        }

        .in-text-selection,
        ::selection {
            text-shadow: none;
            background: var(--select-text-bg-color);
            color: var(--select-text-font-color);
        }

        #write {
            margin: 0px auto;
            height: auto;
            width: inherit;
            word-break: normal;
            overflow-wrap: break-word;
            position: relative;
            white-space: normal;
            overflow-x: visible;
            padding-top: 36px;
        }

        #write.first-line-indent p {
            text-indent: 2em;
        }

        #write.first-line-indent li p,
        #write.first-line-indent p * {
            text-indent: 0px;
        }

        #write.first-line-indent li {
            margin-left: 2em;
        }

        .for-image #write {
            padding-left: 8px;
            padding-right: 8px;
        }

        body.typora-export {
            padding-left: 30px;
            padding-right: 30px;
        }

        .typora-export .footnote-line,
        .typora-export li,
        .typora-export p {
            white-space: pre-wrap;
        }

        .typora-export .task-list-item input {
            pointer-events: none;
        }

        @media screen and (max-width: 500px) {
            body.typora-export {
                padding-left: 0px;
                padding-right: 0px;
            }

            #write {
                padding-left: 20px;
                padding-right: 20px;
            }

            .CodeMirror-sizer {
                margin-left: 0px !important;
            }

            .CodeMirror-gutters {
                display: none !important;
            }
        }

        #write li>figure:last-child {
            margin-bottom: 0.5rem;
        }

        #write ol,
        #write ul {
            position: relative;
        }

        img {
            max-width: 100%;
            vertical-align: middle;
            image-orientation: from-image;
        }

        button,
        input,
        select,
        textarea {
            color: inherit;
            font: inherit;
        }

        input[type="checkbox"],
        input[type="radio"] {
            line-height: normal;
            padding: 0px;
        }

        *,
        ::after,
        ::before {
            box-sizing: border-box;
        }

        #write h1,
        #write h2,
        #write h3,
        #write h4,
        #write h5,
        #write h6,
        #write p,
        #write pre {
            width: inherit;
        }

        #write h1,
        #write h2,
        #write h3,
        #write h4,
        #write h5,
        #write h6,
        #write p {
            position: relative;
        }

        p {
            line-height: inherit;
        }

        h1,
        h2,
        h3,
        h4,
        h5,
        h6 {
            break-after: avoid-page;
            break-inside: avoid;
            orphans: 4;
        }

        p {
            orphans: 4;
        }

        h1 {
            font-size: 2rem;
        }

        h2 {
            font-size: 1.8rem;
        }

        h3 {
            font-size: 1.6rem;
        }

        h4 {
            font-size: 1.4rem;
        }

        h5 {
            font-size: 1.2rem;
        }

        h6 {
            font-size: 1rem;
        }

        .md-math-block,
        .md-rawblock,
        h1,
        h2,
        h3,
        h4,
        h5,
        h6,
        p {
            margin-top: 1rem;
            margin-bottom: 1rem;
        }

        .hidden {
            display: none;
        }

        .md-blockmeta {
            color: rgb(204, 204, 204);
            font-weight: 700;
            font-style: italic;
        }

        a {
            cursor: pointer;
        }

        sup.md-footnote {
            padding: 2px 4px;
            background-color: rgba(238, 238, 238, 0.7);
            color: rgb(85, 85, 85);
            border-radius: 4px;
            cursor: pointer;
        }

        sup.md-footnote a,
        sup.md-footnote a:hover {
            color: inherit;
            text-transform: inherit;
            text-decoration: inherit;
        }

        #write input[type="checkbox"] {
            cursor: pointer;
            width: inherit;
            height: inherit;
        }

        figure {
            overflow-x: auto;
            margin: 1.2em 0px;
            max-width: calc(100% + 16px);
            padding: 0px;
        }

        figure>table {
            margin: 0px;
        }

        tr {
            break-inside: avoid;
            break-after: auto;
        }

        thead {
            display: table-header-group;
        }

        table {
            border-collapse: collapse;
            border-spacing: 0px;
            width: 100%;
            overflow: auto;
            break-inside: auto;
            text-align: left;
        }

        table.md-table td {
            min-width: 32px;
        }

        .CodeMirror-gutters {
            border-right: 0px;
            background-color: inherit;
        }

        .CodeMirror-linenumber {
            user-select: none;
        }

        .CodeMirror {
            text-align: left;
        }

        .CodeMirror-placeholder {
            opacity: 0.3;
        }

        .CodeMirror pre {
            padding: 0px 4px;
        }

        .CodeMirror-lines {
            padding: 0px;
        }

        div.hr:focus {
            cursor: none;
        }

        #write pre {
            white-space: pre-wrap;
        }

        #write.fences-no-line-wrapping pre {
            white-space: pre;
        }

        #write pre.ty-contain-cm {
            white-space: normal;
        }

        .CodeMirror-gutters {
            margin-right: 4px;
        }

        .md-fences {
            font-size: 0.9rem;
            display: block;
            break-inside: avoid;
            text-align: left;
            overflow: visible;
            white-space: pre;
            background: inherit;
            position: relative !important;
        }

        .md-fences-adv-panel {
            width: 100%;
            margin-top: 10px;
            text-align: center;
            padding-top: 0px;
            padding-bottom: 8px;
            overflow-x: auto;
        }

        #write .md-fences.mock-cm {
            white-space: pre-wrap;
        }

        .md-fences.md-fences-with-lineno {
            padding-left: 0px;
        }

        #write.fences-no-line-wrapping .md-fences.mock-cm {
            white-space: pre;
            overflow-x: auto;
        }

        .md-fences.mock-cm.md-fences-with-lineno {
            padding-left: 8px;
        }

        .CodeMirror-line,
        twitterwidget {
            break-inside: avoid;
        }

        .footnotes {
            opacity: 0.8;
            font-size: 0.9rem;
            margin-top: 1em;
            margin-bottom: 1em;
        }

        .footnotes+.footnotes {
            margin-top: 0px;
        }

        .md-reset {
            margin: 0px;
            padding: 0px;
            border: 0px;
            outline: 0px;
            vertical-align: top;
            background: 0px 0px;
            text-decoration: none;
            text-shadow: none;
            float: none;
            position: static;
            width: auto;
            height: auto;
            white-space: nowrap;
            cursor: inherit;
            -webkit-tap-highlight-color: transparent;
            line-height: normal;
            font-weight: 400;
            text-align: left;
            box-sizing: content-box;
            direction: ltr;
        }

        li div {
            padding-top: 0px;
        }

        blockquote {
            margin: 1rem 0px;
        }

        li .mathjax-block,
        li p {
            margin: 0.5rem 0px;
        }

        li blockquote {
            margin: 1rem 0px;
        }

        li {
            margin: 0px;
            position: relative;
        }

        blockquote> :last-child {
            margin-bottom: 0px;
        }

        blockquote> :first-child,
        li> :first-child {
            margin-top: 0px;
        }

        .footnotes-area {
            color: rgb(136, 136, 136);
            margin-top: 0.714rem;
            padding-bottom: 0.143rem;
            white-space: normal;
        }

        #write .footnote-line {
            white-space: pre-wrap;
        }

        @media print {

            body,
            html {
                border: 1px solid transparent;
                height: 99%;
                break-after: avoid;
                break-before: avoid;
                font-variant-ligatures: no-common-ligatures;
            }

            #write {
                margin-top: 0px;
                padding-top: 0px;
                border-color: transparent !important;
            }

            .typora-export * {
                -webkit-print-color-adjust: exact;
            }

            .typora-export #write {
                break-after: avoid;
            }

            .typora-export #write::after {
                height: 0px;
            }

            .is-mac table {
                break-inside: avoid;
            }

            .typora-export-show-outline .typora-export-sidebar {
                display: none;
            }
        }

        .footnote-line {
            margin-top: 0.714em;
            font-size: 0.7em;
        }

        a img,
        img a {
            cursor: pointer;
        }

        pre.md-meta-block {
            font-size: 0.8rem;
            min-height: 0.8rem;
            white-space: pre-wrap;
            background: rgb(204, 204, 204);
            display: block;
            overflow-x: hidden;
        }

        p>.md-image:only-child:not(.md-img-error) img,
        p>img:only-child {
            display: block;
            margin: auto;
        }

        #write.first-line-indent p>.md-image:only-child:not(.md-img-error) img {
            left: -2em;
            position: relative;
        }

        p>.md-image:only-child {
            display: inline-block;
            width: 100%;
        }

        #write .MathJax_Display {
            margin: 0.8em 0px 0px;
        }

        .md-math-block {
            width: 100%;
        }

        .md-math-block:not(:empty)::after {
            display: none;
        }

        .MathJax_ref {
            fill: currentcolor;
        }

        [contenteditable="true"]:active,
        [contenteditable="true"]:focus,
        [contenteditable="false"]:active,
        [contenteditable="false"]:focus {
            outline: 0px;
            box-shadow: none;
        }

        .md-task-list-item {
            position: relative;
            list-style-type: none;
        }

        .task-list-item.md-task-list-item {
            padding-left: 0px;
        }

        .md-task-list-item>input {
            position: absolute;
            top: 0px;
            left: 0px;
            margin-left: -1.2em;
            margin-top: calc(1em - 10px);
            border: none;
        }

        .math {
            font-size: 1rem;
        }

        .md-toc {
            min-height: 3.58rem;
            position: relative;
            font-size: 0.9rem;
            border-radius: 10px;
        }

        .md-toc-content {
            position: relative;
            margin-left: 0px;
        }

        .md-toc-content::after,
        .md-toc::after {
            display: none;
        }

        .md-toc-item {
            display: block;
            color: rgb(65, 131, 196);
        }

        .md-toc-item a {
            text-decoration: none;
        }

        .md-toc-inner:hover {
            text-decoration: underline;
        }

        .md-toc-inner {
            display: inline-block;
            cursor: pointer;
        }

        .md-toc-h1 .md-toc-inner {
            margin-left: 0px;
            font-weight: 700;
        }

        .md-toc-h2 .md-toc-inner {
            margin-left: 2em;
        }

        .md-toc-h3 .md-toc-inner {
            margin-left: 4em;
        }

        .md-toc-h4 .md-toc-inner {
            margin-left: 6em;
        }

        .md-toc-h5 .md-toc-inner {
            margin-left: 8em;
        }

        .md-toc-h6 .md-toc-inner {
            margin-left: 10em;
        }

        @media screen and (max-width: 48em) {
            .md-toc-h3 .md-toc-inner {
                margin-left: 3.5em;
            }

            .md-toc-h4 .md-toc-inner {
                margin-left: 5em;
            }

            .md-toc-h5 .md-toc-inner {
                margin-left: 6.5em;
            }

            .md-toc-h6 .md-toc-inner {
                margin-left: 8em;
            }
        }

        a.md-toc-inner {
            font-size: inherit;
            font-style: inherit;
            font-weight: inherit;
            line-height: inherit;
        }

        .footnote-line a:not(.reversefootnote) {
            color: inherit;
        }

        .md-attr {
            display: none;
        }

        .md-fn-count::after {
            content: ".";
        }

        code,
        pre,
        samp,
        tt {
            font-family: var(--monospace);
        }

        kbd {
            margin: 0px 0.1em;
            padding: 0.1em 0.6em;
            font-size: 0.8em;
            color: rgb(36, 39, 41);
            background: rgb(255, 255, 255);
            border: 1px solid rgb(173, 179, 185);
            border-radius: 3px;
            box-shadow: rgba(12, 13, 14, 0.2) 0px 1px 0px, rgb(255, 255, 255) 0px 0px 0px 2px inset;
            white-space: nowrap;
            vertical-align: middle;
        }

        .md-comment {
            color: rgb(162, 127, 3);
            opacity: 0.6;
            font-family: var(--monospace);
        }

        code {
            text-align: left;
            vertical-align: initial;
        }

        a.md-print-anchor {
            white-space: pre !important;
            border-width: initial !important;
            border-style: none !important;
            border-color: initial !important;
            display: inline-block !important;
            position: absolute !important;
            width: 1px !important;
            right: 0px !important;
            outline: 0px !important;
            background: 0px 0px !important;
            text-decoration: initial !important;
            text-shadow: initial !important;
        }

        .os-windows.monocolor-emoji .md-emoji {
            font-family: "Segoe UI Symbol", sans-serif;
        }

        .md-diagram-panel>svg {
            max-width: 100%;
        }

        [lang="flow"] svg,
        [lang="mermaid"] svg {
            max-width: 100%;
            height: auto;
        }

        [lang="mermaid"] .node text {
            font-size: 1rem;
        }

        table tr th {
            border-bottom: 0px;
        }

        video {
            max-width: 100%;
            display: block;
            margin: 0px auto;
        }

        iframe {
            max-width: 100%;
            width: 100%;
            border: none;
        }

        .highlight td,
        .highlight tr {
            border: 0px;
        }

        mark {
            background: rgb(255, 255, 0);
            color: rgb(0, 0, 0);
        }

        .md-html-inline .md-plain,
        .md-html-inline strong,
        mark .md-inline-math,
        mark strong {
            color: inherit;
        }

        .md-expand mark .md-meta {
            opacity: 0.3 !important;
        }

        mark .md-meta {
            color: rgb(0, 0, 0);
        }

        @media print {

            .typora-export h1,
            .typora-export h2,
            .typora-export h3,
            .typora-export h4,
            .typora-export h5,
            .typora-export h6 {
                break-inside: avoid;
            }
        }

        .md-diagram-panel .messageText {
            stroke: none !important;
        }

        .md-diagram-panel .start-state {
            fill: var(--node-fill);
        }

        .md-diagram-panel .edgeLabel rect {
            opacity: 1 !important;
        }

        .md-fences.md-fences-math {
            font-size: 1em;
        }

        .md-fences-advanced:not(.md-focus) {
            padding: 0px;
            white-space: nowrap;
            border: 0px;
        }

        .md-fences-advanced:not(.md-focus) {
            background: inherit;
        }

        .typora-export-show-outline .typora-export-content {
            max-width: 1440px;
            margin: auto;
            display: flex;
            flex-direction: row;
        }

        .typora-export-sidebar {
            width: 300px;
            font-size: 0.8rem;
            margin-top: 80px;
            margin-right: 18px;
        }

        .typora-export-show-outline #write {
            --webkit-flex: 2;
            flex: 2 1 0%;
        }

        .typora-export-sidebar .outline-content {
            position: fixed;
            top: 0px;
            max-height: 100%;
            overflow: hidden auto;
            padding-bottom: 30px;
            padding-top: 60px;
            width: 300px;
        }

        @media screen and (max-width: 1024px) {

            .typora-export-sidebar,
            .typora-export-sidebar .outline-content {
                width: 240px;
            }
        }

        @media screen and (max-width: 800px) {
            .typora-export-sidebar {
                display: none;
            }
        }

        .outline-content li,
        .outline-content ul {
            margin-left: 0px;
            margin-right: 0px;
            padding-left: 0px;
            padding-right: 0px;
            list-style: none;
        }

        .outline-content ul {
            margin-top: 0px;
            margin-bottom: 0px;
        }

        .outline-content strong {
            font-weight: 400;
        }

        .outline-expander {
            width: 1rem;
            height: 1.42857rem;
            position: relative;
            display: table-cell;
            vertical-align: middle;
            cursor: pointer;
            padding-left: 4px;
        }

        .outline-expander::before {
            content: "";
            position: relative;
            font-family: Ionicons;
            display: inline-block;
            font-size: 8px;
            vertical-align: middle;
        }

        .outline-item {
            padding-top: 3px;
            padding-bottom: 3px;
            cursor: pointer;
        }

        .outline-expander:hover::before {
            content: "";
        }

        .outline-h1>.outline-item {
            padding-left: 0px;
        }

        .outline-h2>.outline-item {
            padding-left: 1em;
        }

        .outline-h3>.outline-item {
            padding-left: 2em;
        }

        .outline-h4>.outline-item {
            padding-left: 3em;
        }

        .outline-h5>.outline-item {
            padding-left: 4em;
        }

        .outline-h6>.outline-item {
            padding-left: 5em;
        }

        .outline-label {
            cursor: pointer;
            display: table-cell;
            vertical-align: middle;
            text-decoration: none;
            color: inherit;
        }

        .outline-label:hover {
            text-decoration: underline;
        }

        .outline-item:hover {
            border-color: rgb(245, 245, 245);
            background-color: var(--item-hover-bg-color);
        }

        .outline-item:hover {
            margin-left: -28px;
            margin-right: -28px;
            border-left: 28px solid transparent;
            border-right: 28px solid transparent;
        }

        .outline-item-single .outline-expander::before,
        .outline-item-single .outline-expander:hover::before {
            display: none;
        }

        .outline-item-open>.outline-item>.outline-expander::before {
            content: "";
        }

        .outline-children {
            display: none;
        }

        .info-panel-tab-wrapper {
            display: none;
        }

        .outline-item-open>.outline-children {
            display: block;
        }

        .typora-export .outline-item {
            padding-top: 1px;
            padding-bottom: 1px;
        }

        .typora-export .outline-item:hover {
            margin-right: -8px;
            border-right: 8px solid transparent;
        }

        .typora-export .outline-expander::before {
            content: "+";
            font-family: inherit;
            top: -1px;
        }

        .typora-export .outline-expander:hover::before,
        .typora-export .outline-item-open>.outline-item>.outline-expander::before {
            content: "−";
        }

        .typora-export-collapse-outline .outline-children {
            display: none;
        }

        .typora-export-collapse-outline .outline-item-open>.outline-children,
        .typora-export-no-collapse-outline .outline-children {
            display: block;
        }

        .typora-export-no-collapse-outline .outline-expander::before {
            content: "" !important;
        }

        .typora-export-show-outline .outline-item-active>.outline-item .outline-label {
            font-weight: 700;
        }

        .md-inline-math-container mjx-container {
            zoom: 0.95;
        }


        :root {
            --side-bar-bg-color: #fafafa;
            --control-text-color: #777;
        }

        @include-when-export url(https://fonts.loli.net/css?family=Open+Sans:400italic,700italic,700,400&subset=latin,latin-ext);

        /* open-sans-regular - latin-ext_latin */
        /* open-sans-italic - latin-ext_latin */
        /* open-sans-700 - latin-ext_latin */
        /* open-sans-700italic - latin-ext_latin */
        html {
            font-size: 16px;
            -webkit-font-smoothing: antialiased;
        }

        body {
            font-family: "Open Sans", "Clear Sans", "Helvetica Neue", Helvetica, Arial, 'Segoe UI Emoji', sans-serif;
            color: rgb(51, 51, 51);
            line-height: 1.6;
        }

        #write {
            max-width: 860px;
            margin: 0 auto;
            padding: 30px;
            padding-bottom: 100px;
        }

        @media only screen and (min-width: 1400px) {
            #write {
                max-width: 1024px;
            }
        }

        @media only screen and (min-width: 1800px) {
            #write {
                max-width: 1200px;
            }
        }

        #write>ul:first-child,
        #write>ol:first-child {
            margin-top: 30px;
        }

        a {
            color: #4183C4;
        }

        h1,
        h2,
        h3,
        h4,
        h5,
        h6 {
            position: relative;
            margin-top: 1rem;
            margin-bottom: 1rem;
            font-weight: bold;
            line-height: 1.4;
            cursor: text;
        }

        h1:hover a.anchor,
        h2:hover a.anchor,
        h3:hover a.anchor,
        h4:hover a.anchor,
        h5:hover a.anchor,
        h6:hover a.anchor {
            text-decoration: none;
        }

        h1 tt,
        h1 code {
            font-size: inherit;
        }

        h2 tt,
        h2 code {
            font-size: inherit;
        }

        h3 tt,
        h3 code {
            font-size: inherit;
        }

        h4 tt,
        h4 code {
            font-size: inherit;
        }

        h5 tt,
        h5 code {
            font-size: inherit;
        }

        h6 tt,
        h6 code {
            font-size: inherit;
        }

        h1 {
            font-size: 2.25em;
            line-height: 1.2;
            border-bottom: 1px solid #eee;
        }

        h2 {
            font-size: 1.75em;
            line-height: 1.225;
            border-bottom: 1px solid #eee;
        }

        /*@media print {
    .typora-export h1,
    .typora-export h2 {
        border-bottom: none;
        padding-bottom: initial;
    }

    .typora-export h1::after,
    .typora-export h2::after {
        content: "";
        display: block;
        height: 100px;
        margin-top: -96px;
        border-top: 1px solid #eee;
    }
}*/

        h3 {
            font-size: 1.5em;
            line-height: 1.43;
        }

        h4 {
            font-size: 1.25em;
        }

        h5 {
            font-size: 1em;
        }

        h6 {
            font-size: 1em;
            color: #777;
        }

        p,
        blockquote,
        ul,
        ol,
        dl,
        table {
            margin: 0.8em 0;
        }

        li>ol,
        li>ul {
            margin: 0 0;
        }

        hr {
            height: 2px;
            padding: 0;
            margin: 16px 0;
            background-color: #e7e7e7;
            border: 0 none;
            overflow: hidden;
            box-sizing: content-box;
        }

        li p.first {
            display: inline-block;
        }

        ul,
        ol {
            padding-left: 30px;
        }

        ul:first-child,
        ol:first-child {
            margin-top: 0;
        }

        ul:last-child,
        ol:last-child {
            margin-bottom: 0;
        }

        blockquote {
            border-left: 4px solid #dfe2e5;
            padding: 0 15px;
            color: #777777;
        }

        blockquote blockquote {
            padding-right: 0;
        }

        table {
            padding: 0;
            word-break: initial;
        }

        table tr {
            border: 1px solid #dfe2e5;
            margin: 0;
            padding: 0;
        }

        table tr:nth-child(2n),
        thead {
            background-color: #f8f8f8;
        }

        table th {
            font-weight: bold;
            border: 1px solid #dfe2e5;
            border-bottom: 0;
            margin: 0;
            padding: 6px 13px;
        }

        table td {
            border: 1px solid #dfe2e5;
            margin: 0;
            padding: 6px 13px;
        }

        table th:first-child,
        table td:first-child {
            margin-top: 0;
        }

        table th:last-child,
        table td:last-child {
            margin-bottom: 0;
        }

        .CodeMirror-lines {
            padding-left: 4px;
        }

        .code-tooltip {
            box-shadow: 0 1px 1px 0 rgba(0, 28, 36, .3);
            border-top: 1px solid #eef2f2;
        }

        .md-fences,
        code,
        tt {
            border: 1px solid #e7eaed;
            background-color: #f8f8f8;
            border-radius: 3px;
            padding: 0;
            padding: 2px 4px 0px 4px;
            font-size: 0.9em;
        }

        code {
            background-color: #f3f4f4;
            padding: 0 2px 0 2px;
        }

        .md-fences {
            margin-bottom: 15px;
            margin-top: 15px;
            padding-top: 8px;
            padding-bottom: 6px;
        }


        .md-task-list-item>input {
            margin-left: -1.3em;
        }

        @media print {
            html {
                font-size: 13px;
            }

            table,
            pre {
                page-break-inside: avoid;
            }

            pre {
                word-wrap: break-word;
            }
        }

        .md-fences {
            background-color: #f8f8f8;
        }

        #write pre.md-meta-block {
            padding: 1rem;
            font-size: 85%;
            line-height: 1.45;
            background-color: #f7f7f7;
            border: 0;
            border-radius: 3px;
            color: #777777;
            margin-top: 0 !important;
        }

        .mathjax-block>.code-tooltip {
            bottom: .375rem;
        }

        .md-mathjax-midline {
            background: #fafafa;
        }

        #write>h3.md-focus:before {
            left: -1.5625rem;
            top: .375rem;
        }

        #write>h4.md-focus:before {
            left: -1.5625rem;
            top: .285714286rem;
        }

        #write>h5.md-focus:before {
            left: -1.5625rem;
            top: .285714286rem;
        }

        #write>h6.md-focus:before {
            left: -1.5625rem;
            top: .285714286rem;
        }

        .md-image>.md-meta {
            /*border: 1px solid #ddd;*/
            border-radius: 3px;
            padding: 2px 0px 0px 4px;
            font-size: 0.9em;
            color: inherit;
        }

        .md-tag {
            color: #a7a7a7;
            opacity: 1;
        }

        .md-toc {
            margin-top: 20px;
            padding-bottom: 20px;
        }

        .sidebar-tabs {
            border-bottom: none;
        }

        #typora-quick-open {
            border: 1px solid #ddd;
            background-color: #f8f8f8;
        }

        #typora-quick-open-item {
            background-color: #FAFAFA;
            border-color: #FEFEFE #e5e5e5 #e5e5e5 #eee;
            border-style: solid;
            border-width: 1px;
        }

        /** focus mode */
        .on-focus-mode blockquote {
            border-left-color: rgba(85, 85, 85, 0.12);
        }

        header,
        .context-menu,
        .megamenu-content,
        footer {
            font-family: "Segoe UI", "Arial", sans-serif;
        }

        .file-node-content:hover .file-node-icon,
        .file-node-content:hover .file-node-open-state {
            visibility: visible;
        }

        .mac-seamless-mode #typora-sidebar {
            background-color: #fafafa;
            background-color: var(--side-bar-bg-color);
        }

        .md-lang {
            color: #b4654d;
        }

        /*.html-for-mac {
    --item-hover-bg-color: #E6F0FE;
}*/

        #md-notification .btn {
            border: 0;
        }

        .dropdown-menu .divider {
            border-color: #e5e5e5;
            opacity: 0.4;
        }

        .ty-preferences .window-content {
            background-color: #fafafa;
        }

        .ty-preferences .nav-group-item.active {
            color: white;
            background: #999;
        }

        .menu-item-container a.menu-style-btn {
            background-color: #f5f8fa;
            background-image: linear-gradient(180deg, hsla(0, 0%, 100%, 0.8), hsla(0, 0%, 100%, 0));
        }
    </style>
    <title>设计模式</title>
</head>

<body class='typora-export os-windows typora-export-show-outline typora-export-collapse-outline'>
    <div class='typora-export-content'>
        <div class="typora-export-sidebar">
            <div class="outline-content">
                <li class="outline-item-wrapper outline-h1 outline-item-single">
                    <div class="outline-item"><span class="outline-expander"></span><a class="outline-label"
                            href="#创建型模式">创建型模式</a></div>
                    <ul class="outline-children"></ul>
                </li>
                <li class="outline-item-wrapper outline-h1 outline-item-single">
                    <div class="outline-item"><span class="outline-expander"></span><a class="outline-label"
                            href="#结构型模式">结构型模式</a></div>
                    <ul class="outline-children"></ul>
                </li>
                <li class="outline-item-wrapper outline-h1 outline-item-single">
                    <div class="outline-item"><span class="outline-expander"></span><a class="outline-label"
                            href="#行为型模式">行为型模式</a></div>
                    <ul class="outline-children"></ul>
                </li>
            </div>
        </div>
        <div id='write' class=''>
            <h1 id='创建型模式'><span>创建型模式</span></h1>
            <p>&nbsp;</p>
            <p><span>Singleton模式解决的是实体对象个数的问题。</span></p>
            <p><span>除了Singleton之外，其他创建型模式解决的都是New所带来的耦合关系。</span></p>
            <p><span>Factory Method，Abstract
                    Factory，Builder都需要一个额外的工厂类来负责实例化“易变对象”，而Prototype则是通过原型（一个特殊的工厂类）来克隆“易变对象”。</span></p>
            <p><span>如果遇到“易变类”，起初的设计通常从Factory Method开始，当遇到更多的复杂变化时，再考虑重构为其他三种工厂模式（Abstract
                    Factory，Builder，Prototype）</span></p>
            <p><span> </span></p>
            <p><strong><span>适用性：</span></strong></p>
            <p><strong><span>一、Abstract Factory：</span></strong></p>
            <p><span> 1、一个系统要独立于它的产品的创建、组合和表示时。</span></p>
            <p><span> 2、一个系统要由多个产品系列中的一个配置时。</span></p>
            <p><span> 3、当要强调一系列相关的产品对象的设计以便进行联合使用时。</span></p>
            <p><span> 4、当提供一个产品类库，而只是显示它们的接口而不是实现时。</span></p>
            <p><strong><span>二、Builder：</span></strong></p>
            <p><span> 1、当创建复杂对象的</span><a
                    href='http://lib.csdn.net/base/datastructure'><span>算法</span></a><span>应该独立于该对象的组成部分以及它们的装配方式时。</span>
            </p>
            <p><span> 2、当构造过程必须允许被构造的对象有不同的表示时。</span></p>
            <p><strong><span>三、Factory Method：</span></strong></p>
            <p><span> 1、当一个类不知道它所必须创建的对象的类的时候。</span></p>
            <p><span> 2、当一个类希望由它的子类来指定它所创建的对象的时候</span></p>
            <p><span> 3、当类将创建对象的职责委托给多个帮助子类中的某一个，并且你希望将哪一个帮助子类是代理者这以信息局部化的时候。</span></p>
            <p><strong><span>四、Prototype：</span></strong></p>
            <p><span> 1、当要实例化的类是运行时刻指定时。</span></p>
            <p><span> 2、为了避免创建一个与产品类层次平行的工厂类层次时。</span></p>
            <p><span> 3、当一个类的实例只能有几个不同状态组合中的一种时。建立相应数目的原型并克隆它们可能比每次用何时的状态手工实例化该类更方面一些。</span></p>
            <p><strong><span>五、Singleton：</span></strong></p>
            <p><span> 1、当类只能有一个实例而且客户可以从一个总所周知的访问点访问它时。</span></p>
            <p><span> 2、当这个唯一实例应该是通过子类化可扩展的，并且客户应该无需更改代码就能使用一个扩展的实例时。</span></p>
            <p>&nbsp;</p>
            <h1 id='结构型模式'><span>结构型模式</span></h1>
            <p>&nbsp;</p>
            <p><span>Adapter模式注重转换接口，将不吻合的接口适配对接。</span></p>
            <p><span>Bridge模式注重分离接口与其实现，支持多维度变化。</span></p>
            <p><span>Composite模式注重统一接口，将“一对多”的关系转换为“一对一”的关系。</span></p>
            <p><span>Decorator模式注重稳定接口，在此前提下为对象扩展功能。</span></p>
            <p><span>Facade模式注重简化接口，简化组件系统与外部客户程序的依赖关系。</span></p>
            <p><span>Flyweight模式注重保留接口，在内部使用共享技术对对象存储进行优化。</span></p>
            <p><span>Proxy模式注重假借接口，增加间接层次实现灵活控制。</span></p>
            <p><span> </span></p>
            <p><strong><span>适用性：</span></strong></p>
            <p><strong><span>一、Adapter：</span></strong></p>
            <p><span> 1、想使用一个已经存在的类，而它的接口不符合需求</span></p>
            <p><span> 2、想创建一个可复用的类，该类可以与其他不相关的类或不可预见的类（即那些接口可能不兼容的类）协同工作</span></p>
            <p><span> 3、（仅适用于对象Adapter）想使用一些已经存在的子类，但是不可能对每一个都进行子类化以匹配它们的接口。对象适配器可以适配它的父类接口。</span></p>
            <p><strong><span>二、Bridge：</span></strong></p>
            <p><span> 1、你不希望在抽象和它的实现部分之间有一个固定的绑定关系。</span></p>
            <p><span> 例如这种情况可能是因为，在程序运行时刻实现部分应可以被选择或者切换。</span></p>
            <p><span> 2、类的抽象以及它的实现都应该可以通过生成子类的方法加以扩充。这时Bridge模式使你可以对不同的抽象接口和实现部分进行组合，并分别对它们进行扩充。</span></p>
            <p><span> 3、对一个抽象的实现部分的修改应对客户不产生影响，即客户的代码不必重新编译。</span></p>
            <p><strong><span>三、Composite：</span></strong></p>
            <p><span> 1、表示对象的部分-整体层次结构。</span></p>
            <p><span> 2、希望用户忽略组合对象与单个对象的不同，用户将统一地使用组合结构中的所有对象。</span></p>
            <p><strong><span>四、Decorator：</span></strong></p>
            <p><span> 1、在不影响其他对象的情况下，以动态、透明的方式给单个对象添加职责。</span></p>
            <p><span> 2、处理那些可以撤销的职责。</span></p>
            <p><span> 3、当不能采用生成子类的方法进行扩充时。</span></p>
            <p><span> 一种情况是，可能有大量独立的扩展，为支持每一种组合将产生大量的子类，使得子类数目呈爆炸性增长。</span></p>
            <p><span> 另一种情况可能是因为类定义被隐藏，或类定义不能用于生成子类。</span></p>
            <p><strong><span>五、Facade：</span></strong></p>
            <p><span>
                    1、当你要为一个复杂子系统提供一个简单接口时。子系统往往因为不断演化而变得越来越复杂。大多数模式使时都会产生更多更小的类。这使得子系统更具可重用性，也更容易对子系统进行定制，但这也给那些不需要定制子系统的用户带来一些使用上的困难。Facade可以提供一个简单的缺省视图，这一视图对大多数用户来说已经足够，而那些需要更多的可定制性的用户可以越过Facade层。</span>
            </p>
            <p><span> 2、客户程序与抽象类的实现部分之间存在着很大的依赖性，引入facade将这个子系统与客户以及其他的子系统分离，可以提高子系统独立性和可移植性。</span></p>
            <p><span>
                    3、当你需要构建一个层次结构的子系统时，使用Facade模式定义子系统中每层的入口点。如果子系统之间是相互依赖的，你可以让它们仅通过Facade进行通讯，从而简化了它们之间的依赖关系。</span>
            </p>
            <p><strong><span>六、Flyweight：</span></strong></p>
            <p><span> 1、一个应用程序使用了大量的对象，造成很大的存储开销</span></p>
            <p><span> 2、完全由于使用大量的对象，造成很大的存储开销</span></p>
            <p><span> 3、对象的大多数状态都可变为外部状态</span></p>
            <p><span> 4、如果删除对象的外部状态，那么可以相对较少的共享对象取代很多组对象</span></p>
            <p><span> 5、应用程序不依赖于对象标识。由于Flyweight对象可以被共享，对于概念上明显有别的对象，标识</span><a
                    href='http://lib.csdn.net/base/softwaretest'><span>测试</span></a><span>将返回真值</span></p>
            <p><strong><span>七、Proxy</span></strong></p>
            <p><span> 1、远程代理（Remote Peoxy）为一个对象在不同的地址空间提供局部代表。这样可以隐藏一个对象存在于不同地址空间的事实。</span></p>
            <p><span> 2、虚拟代理（Virtual Proxy）根据需要创建开销很大的对象。通过它来存放实例化需要很长时间的真实对象。</span></p>
            <p><span> 3、安全代理（Protection Proxy）控制真实对象访问时的权限。</span></p>
            <p><span> 4、智能指引（Smart Reference）当调用真实的对象时，代理处理另外一些事。</span></p>
            <p>&nbsp;</p>
            <h1 id='行为型模式'><span>行为型模式</span></h1>
            <p>&nbsp;</p>
            <p><span>Chain Of Responsibility模式注重封装对象责任，支持责任的变化。</span></p>
            <p><span>Command模式注重将请求封装为对象，支持请求的变化。</span></p>
            <p><span>Interpreter模式注重封装特定领域变化，支持领域问题的频繁变化。</span></p>
            <p><span>Iterator模式注重封装集合对象内部结构，支持集合的变化。</span></p>
            <p><span>Mediator模式注重封装对象间的交互，支持对象交互的变化。</span></p>
            <p><span>Memento模式注重封装对象状态变化，支持状态保存/恢复。</span></p>
            <p><span>Observer模式注重封装对象通知，支持通信对象的变化。</span></p>
            <p><span>State模式注重封装与状态相关的行为，支持状态的变化。</span></p>
            <p><span>Strategy模式注重封装苏阿伐，支持</span><a
                    href='http://lib.csdn.net/base/datastructure'><span>算法</span></a><span>的变化。</span></p>
            <p><span>Template Method模式封装算法结构，支持算法子步骤变化。</span></p>
            <p><span>Visitor模式注重封装对象操作变化，支持在运行时为类层次结构动态添加新的操作。</span></p>
            <p><span> </span></p>
            <p><strong><span>适用性：</span></strong></p>
            <p><strong><span>一、Chain of Responsibility</span></strong></p>
            <p><span>1、有多个的对象可以处理一个请求，哪个对象处理该请求运行时刻自动确定。</span></p>
            <p><span>2、你想在不明确指定接受者的情况下，向多个对象中的一个提交一个请求。</span></p>
            <p><span>3、可处理一个请求的对象集合应被动态指定。</span></p>
            <p><strong><span>二、Command</span></strong></p>
            <p><span>1、回调。（回调函数是指函数先在某处注册，而它将在稍后某个需要的时候被调用。Command是回调机制的一个面向对象的替代品。）</span></p>
            <p><span>2、在不同的时刻指定、排列和执行请求。</span></p>
            <p><span>3、支持取消操作。</span></p>
            <p><span>4、支持修改日志。</span></p>
            <p><span>5、用构建在原语操作上的高层操作构造一个系统。</span></p>
            <p><strong><span>三、Interpreter</span></strong></p>
            <p><span>1、该文法简单对于复杂的文法，文法的类层次变得庞大而无法管理。</span></p>
            <p><span>2、效率不是一个关键最高效的解释器不是通过直接解释语法分析树实现的，而是首先将它们转化成另一种形式。</span></p>
            <p><strong><span>四、Iterator</span></strong></p>
            <p><span>1、访问一个聚合对象的内容而无需暴露它的内部表示。</span></p>
            <p><span>2、支持对聚合对象的多种遍历。</span></p>
            <p><span>3、为遍历不同的聚合结构提供一个统一的接口（即，支持多态迭代）</span></p>
            <p><strong><span>五、Mediator</span></strong></p>
            <p><span>1、一组对象以定义良好但是复杂的方式进行通信。产生的相互依赖关系结构混乱且难以理解</span></p>
            <p><span>2、一个对象引用其他很多对象并且直接与这些对象通信，导致难以复用该对象</span></p>
            <p><span>3、像定制一个分布在多个类中的行为，而又不想生成太多的子类</span></p>
            <p><strong><span>六、Memento</span></strong></p>
            <p><span>1、必须保存一个对象在某一时刻的（部分）状态，这样以后需要时它才能恢复到先前的状态</span></p>
            <p><span>2、如果一个用接口来让其它对象直接得到这些状态，将会暴露对象的实现细节并破坏对象的封装性。</span></p>
            <p><strong><span>七、Observer</span></strong></p>
            <p><span>1、当一个抽象模型有两个方面，其中一个方面依赖于另一方面。将这二者封装在独立的对象中以使它们可以各自独立地改变和复用。</span></p>
            <p><span>2、当对一个对象的改变需要同时改变其它对象，而不知道具体有多少对象有待改变。</span></p>
            <p><span>3、当一个对象必须通知其他对象，而它又不能假定其它对象是谁。换言之，你不希望这些对象是紧耦合的。</span></p>
            <p><strong><span>八、State</span></strong></p>
            <p><span>1、一个对象的行为取决于它的状态，并且它必须在运行时刻根据状态改变它的行为。</span></p>
            <p><span>2、一个操作中含有庞大的多分支条件语句，且这些分支依赖于该对象的状态。这个状态通常用一个或多个枚举常量表示。（如大话设计模式里介绍的：无尽加班何时休。每个时间段的都干什么。枚举每个时间段）</span>
            </p>
            <p><strong><span>九、Strategy</span></strong></p>
            <p><span>1、许多相关的类仅仅是行为有异。“策略”提供了一种用多个行为中的一个行为来配置一个类的方法。</span></p>
            <p><span>2、需要使用一个算法的不同变体。</span></p>
            <p><span>3、算法使用客户不应该知道的数据。</span></p>
            <p><span>4、一个类定义了多种行为，并且这些行为在这个类的操作中以多个条件语句的形式出现。将相关的条件分支移入它们各自的Strategy类中以代替这些条件语句。</span></p>
            <p><span>（《大话设计模式》商场促销，收银的算法）</span></p>
            <p><strong><span>十、Template Method</span></strong></p>
            <p><span>1、一次性实现一个算法的不变的部分，并将可变的行为留给子类来实现。</span></p>
            <p><span>2、各子类中公共的行为应被提取出来并集中到一个公共的父类中以避免代码重复。</span></p>
            <p><span>3、控制子类扩展。</span></p>
            <p><strong><span>十一、Visitor</span></strong></p>
            <p><span>1、一个对象结构包含很多类对象，它们有不同的接口，而你想对这些对象实施一些依赖于其具体类的操作。</span></p>
            <p><span>2、需要对一个对象结构中的对象进行很多不同的并且不相关的操作，而你想避免让这些操作“污染”这些对象的类。</span></p>
            <p><span>3、定义对象结构的类很少改变，但经常需要在此结构上定义新的操作。改变对象结构类需要重定义对所有访问者的接口，这可能需要很大的代价。如果对象结构类经常改变，那么可能还是在这些类中定义这些操作较好</span>
            </p>
        </div>
    </div>

    <script>(function () { var e = document.body.parentElement, t = [], n = null, i = document.body.classList.contains("typora-export-collapse-outline"), r = function (e, t, n) { document.addEventListener(e, function (e) { if (!e.defaultPrevented) for (var i = e.target; i && i != this; i = i.parentNode)if (i.matches(t)) { !1 === n.call(i, e) && (e.preventDefault(), e.stopPropagation()); break } }, !1) }; function o() { return e.scrollTop } r("click", ".outline-expander", function (e) { var t = this.closest(".outline-item-wrapper").classList; return t.contains("outline-item-open") ? t.remove("outline-item-open") : t.add("outline-item-open"), d(), !1 }), r("click", ".outline-item", function (e) { var t = this.querySelector(".outline-label"); if (location.hash = "#" + t.getAttribute("href"), i) { var n = this.closest(".outline-item-wrapper").classList; n.contains("outline-item-open") || n.add("outline-item-open"), c(), n.add("outline-item-active") } }); var a, s, l = function () { var e = o(); n = null; for (var i = 0; i < t.length && t[i][1] - e < 60; i++)n = t[i] }, c = function () { document.querySelectorAll(".outline-item-active").forEach(e => e.classList.remove("outline-item-active")), document.querySelectorAll(".outline-item-single.outline-item-open").forEach(e => e.classList.remove("outline-item-open")) }, d = function () { if (n) { c(); var e = document.querySelector('.outline-label[href="#' + (CSS.escape ? CSS.escape(n[0]) : n[0]) + '"]'); if (e) if (i) { var t = e.closest(".outline-item-open>ul>.outline-item-wrapper"); if (t) t.classList.add("outline-item-active"); else { for (var r = (e = e.closest(".outline-item-wrapper")).parentElement.closest(".outline-item-wrapper"); r;)r = (e = r).parentElement.closest(".outline-item-wrapper"); e.classList.add("outline-item-active") } } else e.closest(".outline-item-wrapper").classList.add("outline-item-active") } }; window.addEventListener("scroll", function (e) { a && clearTimeout(a), a = setTimeout(function () { l(), d() }, 300) }); var u = function () { s = setTimeout(function () { !function () { t = []; var e = o(); document.querySelector("#write").querySelectorAll("h1, h2, h3, h4, h5, h6").forEach(n => { var i = n.getAttribute("id"); t.push([i, e + n.getBoundingClientRect().y]) }) }(), l(), d() }, 300) }; window.addEventListener("resize", function (e) { s && clearTimeout(s), u() }), u() })();</script>
</body>

</html>
