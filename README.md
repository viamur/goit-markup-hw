<article><div class="theme-doc-markdown markdown"><ul><li>Create a repository <code>goit-markup-hw-05</code>.</li><li>Clone the created repository and copy the previous work files into it.</li><li>Add animated decorative effects to layout pages of
<a href="https://www.figma.com/file/4ne9cjmosUiP9OgIdkkYB1/Web-Studio-Homework-Project?node-id=1%3A836" target="_blank" rel="noopener noreferrer"><strong>homework #5</strong></a>.</li><li>Set up <code>GitHub Pages</code> and add a link to the live page in the header of the
GitHub repository.</li></ul><h2 class="anchor anchorWithHideOnScrollNavbar_WYt5" id="criteria-for-work-acceptance-by-the-tutor">Criteria for work acceptance by the tutor<a class="hash-link" href="#criteria-for-work-acceptance-by-the-tutor" title="Direct link to heading">​</a></h2><h3 class="anchor anchorWithHideOnScrollNavbar_WYt5" id="project">Project<a class="hash-link" href="#project" title="Direct link to heading">​</a></h3><p><strong><code>«A1»</code></strong> All styles are contained in one <code>styles.css</code> file in the <code>css</code>
folder.</p><p><strong><code>«A2»</code></strong> Source code is formatted with <code>Prettier</code>.</p><p><strong><code>«A3»</code></strong> All images and text content are taken from the layout.</p><p><strong><code>«A4»</code></strong> All HTML pages have a style normalizer
<a href="https://github.com/sindresorhus/modern-normalize" target="_blank" rel="noopener noreferrer"><code>modern-normalize</code></a>.</p><p><strong><code>«A5»</code></strong> The code is in line with the <a href="https://codeguide.co/" target="_blank" rel="noopener noreferrer"><strong>guide</strong></a>.</p><p><strong><code>«A6»</code></strong> The modal window script is linked in HTML as a separate file,
<code>modal.js</code>.</p><h3 class="anchor anchorWithHideOnScrollNavbar_WYt5" id="markup">Markup<a class="hash-link" href="#markup" title="Direct link to heading">​</a></h3><p><strong><code>«B1»</code></strong> HTML-markup is done for all layout elements.</p><p><strong><code>«B2»</code></strong> Tags are used according to their semantics.</p><h3 class="anchor anchorWithHideOnScrollNavbar_WYt5" id="styling">Styling<a class="hash-link" href="#styling" title="Direct link to heading">​</a></h3><p><strong><code>«C1»</code></strong> For all hover and focus effects (color, background, shadow),
transitions are made. Time is set to <code>250ms</code>, and the timing function is
<code>cubic-bezier(0.4, 0, 0.2, 1)</code>.</p><p><strong><code>«C2»</code></strong> Transitions and animations explicitly specify the properties to be
animated. There is no <code>all</code> value anywhere.</p><p><strong><code>«C3»</code></strong> In the <code>What We Do</code> section, text with background is positioned over
the image.</p><p><strong><code>«C4»</code></strong> In the main navigation, the current page&#x27;s link (which the user is
currently viewing) is underlined using the <code>::after</code> pseudo-element.</p><p><strong><code>«C5»</code></strong> Blue overlay with text appears on the cards of the <code>Portfolio</code> page
when hovering over any part of the card.</p><p><strong><code>«C6»</code></strong> Blue overlay slides out from the bottom of the cards on the
<code>Portfolio</code> page, as shown in the video.</p><img src="/lms-html-css-homework/v2/en/img/05-preview.gif" alt="card overlay preview" style="display:block;width:100%;margin-left:auto;margin-right:auto;margin-bottom:var(--ifm-leading);max-width:600px"><p><strong><code>«C7»</code></strong> Pseudo-elements have no text content in the <code>content</code> property. They
are used exclusively for decorative purposes.</p><h3 class="anchor anchorWithHideOnScrollNavbar_WYt5" id="modal-window">Modal window<a class="hash-link" href="#modal-window" title="Direct link to heading">​</a></h3><p><strong><code>«D1»</code></strong> The markup and styling of the modal &quot;backdrop&quot; (dark semi-transparent
background) are done.</p><p><strong><code>«D2»</code></strong> &quot;Backdrop&quot; fills 100% of the height and width of the browser viewport
and stays fixed in it.</p><p><strong><code>«D3»</code></strong> The markup and styling of the modal window are done.</p><p><strong><code>«D4»</code></strong> The modal window is vertically and horizontally positioned in the
middle of the backdrop.</p><p><strong><code>«D5»</code></strong> The markup and styling of the button for closing the modal window in
the upper right corner are done.</p><p><strong><code>«D6»</code></strong> By default, the modal and backdrop are hidden using the <code>is-hidden</code>
class in the backdrop, whose selector uses the <code>visibility</code>, <code>opacity</code> and
<code>pointer-events</code> properties.</p><p><strong><code>«D7»</code></strong> If you remove the <code>is-hidden</code> class from the backdrop, the backdrop
and modal window will appear.</p><p><strong><code>«D8»</code></strong> The modal window opening/closing is animated using a transition with
an arbitrary effect such as <code>scale</code> or <code>translate</code>, and <code>opacity</code>.</p><h2 class="anchor anchorWithHideOnScrollNavbar_WYt5" id="modal-window-openingclosing">Modal window opening/closing<a class="hash-link" href="#modal-window-openingclosing" title="Direct link to heading">​</a></h2><p>A modal window with the order form opens by clicking on the &quot;Order a service&quot;
button. In order for the script to work, you need to add special attributes to
the markup, used by the script to search for elements:</p><ul><li><code>data-modal-open</code> to the button for modal window opening;</li><li><code>data-modal-close</code> to the button for modal window closing;</li><li><code>data-modal</code> to the modal window&#x27;s backdrop.</li></ul><p>Then, before the closing <code>body</code> tag, add the <code>script</code> tag with a link to the
script file for the modal window.</p><div class="language-html codeBlockContainer_Ckt0 theme-code-block" style="--prism-color:#393A34;--prism-background-color:#f6f8fa"><div class="codeBlockContent_biex"><pre tabindex="0" class="prism-code language-html codeBlock_bY9V thin-scrollbar"><code class="codeBlockLines_e6Vv"><span class="token-line" style="color:#393A34"><span class="token tag punctuation" style="color:#393A34">&lt;</span><span class="token tag" style="color:#00009f">body</span><span class="token tag punctuation" style="color:#393A34">&gt;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  </span><span class="token comment" style="color:#999988;font-style:italic">&lt;!-- All you markup, including the modal window --&gt;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain" style="display:inline-block"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  </span><span class="token comment" style="color:#999988;font-style:italic">&lt;!-- Place before the body closing tag --&gt;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  </span><span class="token tag punctuation" style="color:#393A34">&lt;</span><span class="token tag" style="color:#00009f">script</span><span class="token tag" style="color:#00009f"> </span><span class="token tag attr-name" style="color:#00a4db">src</span><span class="token tag attr-value punctuation attr-equals" style="color:#393A34">=</span><span class="token tag attr-value punctuation" style="color:#393A34">&quot;</span><span class="token tag attr-value" style="color:#e3116c">./js/modal.js</span><span class="token tag attr-value punctuation" style="color:#393A34">&quot;</span><span class="token tag punctuation" style="color:#393A34">&gt;</span><span class="token script"></span><span class="token tag punctuation" style="color:#393A34">&lt;/</span><span class="token tag" style="color:#00009f">script</span><span class="token tag punctuation" style="color:#393A34">&gt;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain"></span><span class="token tag punctuation" style="color:#393A34">&lt;/</span><span class="token tag" style="color:#00009f">body</span><span class="token tag punctuation" style="color:#393A34">&gt;</span><br></span></code></pre><div class="buttonGroup__atx"><button type="button" aria-label="Copy code to clipboard" title="Copy" class="clean-btn"><span class="copyButtonIcons_eSgA" aria-hidden="true"><svg class="copyButtonIcon_y97N" viewBox="0 0 24 24"><path d="M19,21H8V7H19M19,5H8A2,2 0 0,0 6,7V21A2,2 0 0,0 8,23H19A2,2 0 0,0 21,21V7A2,2 0 0,0 19,5M16,1H4A2,2 0 0,0 2,3V17H4V3H16V1Z"></path></svg><svg class="copyButtonSuccessIcon_LjdS" viewBox="0 0 24 24"><path d="M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"></path></svg></span></button></div></div></div><p>The script to be copied and pasted into the <code>modal.js</code> file.</p><div class="language-js codeBlockContainer_Ckt0 theme-code-block" style="--prism-color:#393A34;--prism-background-color:#f6f8fa"><div class="codeBlockContent_biex"><pre tabindex="0" class="prism-code language-js codeBlock_bY9V thin-scrollbar"><code class="codeBlockLines_e6Vv"><span class="token-line" style="color:#393A34"><span class="token punctuation" style="color:#393A34">(</span><span class="token punctuation" style="color:#393A34">(</span><span class="token punctuation" style="color:#393A34">)</span><span class="token plain"> </span><span class="token arrow operator" style="color:#393A34">=&gt;</span><span class="token plain"> </span><span class="token punctuation" style="color:#393A34">{</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  </span><span class="token keyword" style="color:#00009f">const</span><span class="token plain"> refs </span><span class="token operator" style="color:#393A34">=</span><span class="token plain"> </span><span class="token punctuation" style="color:#393A34">{</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">    </span><span class="token literal-property property" style="color:#36acaa">openModalBtn</span><span class="token operator" style="color:#393A34">:</span><span class="token plain"> </span><span class="token dom variable" style="color:#36acaa">document</span><span class="token punctuation" style="color:#393A34">.</span><span class="token method function property-access" style="color:#d73a49">querySelector</span><span class="token punctuation" style="color:#393A34">(</span><span class="token string" style="color:#e3116c">&quot;[data-modal-open]&quot;</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">,</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">    </span><span class="token literal-property property" style="color:#36acaa">closeModalBtn</span><span class="token operator" style="color:#393A34">:</span><span class="token plain"> </span><span class="token dom variable" style="color:#36acaa">document</span><span class="token punctuation" style="color:#393A34">.</span><span class="token method function property-access" style="color:#d73a49">querySelector</span><span class="token punctuation" style="color:#393A34">(</span><span class="token string" style="color:#e3116c">&quot;[data-modal-close]&quot;</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">,</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">    </span><span class="token literal-property property" style="color:#36acaa">modal</span><span class="token operator" style="color:#393A34">:</span><span class="token plain"> </span><span class="token dom variable" style="color:#36acaa">document</span><span class="token punctuation" style="color:#393A34">.</span><span class="token method function property-access" style="color:#d73a49">querySelector</span><span class="token punctuation" style="color:#393A34">(</span><span class="token string" style="color:#e3116c">&quot;[data-modal]&quot;</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">,</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  </span><span class="token punctuation" style="color:#393A34">}</span><span class="token punctuation" style="color:#393A34">;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain" style="display:inline-block"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  refs</span><span class="token punctuation" style="color:#393A34">.</span><span class="token property-access">openModalBtn</span><span class="token punctuation" style="color:#393A34">.</span><span class="token method function property-access" style="color:#d73a49">addEventListener</span><span class="token punctuation" style="color:#393A34">(</span><span class="token string" style="color:#e3116c">&quot;click&quot;</span><span class="token punctuation" style="color:#393A34">,</span><span class="token plain"> toggleModal</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  refs</span><span class="token punctuation" style="color:#393A34">.</span><span class="token property-access">closeModalBtn</span><span class="token punctuation" style="color:#393A34">.</span><span class="token method function property-access" style="color:#d73a49">addEventListener</span><span class="token punctuation" style="color:#393A34">(</span><span class="token string" style="color:#e3116c">&quot;click&quot;</span><span class="token punctuation" style="color:#393A34">,</span><span class="token plain"> toggleModal</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain" style="display:inline-block"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  </span><span class="token keyword" style="color:#00009f">function</span><span class="token plain"> </span><span class="token function" style="color:#d73a49">toggleModal</span><span class="token punctuation" style="color:#393A34">(</span><span class="token punctuation" style="color:#393A34">)</span><span class="token plain"> </span><span class="token punctuation" style="color:#393A34">{</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">    refs</span><span class="token punctuation" style="color:#393A34">.</span><span class="token property-access">modal</span><span class="token punctuation" style="color:#393A34">.</span><span class="token property-access">classList</span><span class="token punctuation" style="color:#393A34">.</span><span class="token method function property-access" style="color:#d73a49">toggle</span><span class="token punctuation" style="color:#393A34">(</span><span class="token string" style="color:#e3116c">&quot;is-hidden&quot;</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">;</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain">  </span><span class="token punctuation" style="color:#393A34">}</span><span class="token plain"></span><br></span><span class="token-line" style="color:#393A34"><span class="token plain"></span><span class="token punctuation" style="color:#393A34">}</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">(</span><span class="token punctuation" style="color:#393A34">)</span><span class="token punctuation" style="color:#393A34">;</span><br></span></code></pre><div class="buttonGroup__atx"><button type="button" aria-label="Copy code to clipboard" title="Copy" class="clean-btn"><span class="copyButtonIcons_eSgA" aria-hidden="true"><svg class="copyButtonIcon_y97N" viewBox="0 0 24 24"><path d="M19,21H8V7H19M19,5H8A2,2 0 0,0 6,7V21A2,2 0 0,0 8,23H19A2,2 0 0,0 21,21V7A2,2 0 0,0 19,5M16,1H4A2,2 0 0,0 2,3V17H4V3H16V1Z"></path></svg><svg class="copyButtonSuccessIcon_LjdS" viewBox="0 0 24 24"><path d="M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"></path></svg></span></button></div></div></div></div></article>
