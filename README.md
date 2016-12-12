<h1>JSM&#039;s Non-Breaking Space for French Content</h1>

<table>
<tr><th align="right" valign="top" nowrap>Plugin Name</th><td>JSM&#039;s Non-Breaking Space for French Content</td></tr>
<tr><th align="right" valign="top" nowrap>Summary</th><td>Adds a non-breaking space between words and punctuation marks to avoid inappropriate line-breaks in French.</td></tr>
<tr><th align="right" valign="top" nowrap>Stable Version</th><td>1.7.2-1</td></tr>
<tr><th align="right" valign="top" nowrap>Requires At Least</th><td>WordPress 3.7</td></tr>
<tr><th align="right" valign="top" nowrap>Tested Up To</th><td>WordPress 4.7</td></tr>
<tr><th align="right" valign="top" nowrap>Contributors</th><td>jsmoriss</td></tr>
<tr><th align="right" valign="top" nowrap>License</th><td><a href="https://www.gnu.org/licenses/gpl.txt">GPLv3</a></td></tr>
<tr><th align="right" valign="top" nowrap>Tags / Keywords</th><td>nbsp, french, exclamation, question, interrogation, line-break</td></tr>
</table>

<h2>Description</h2>

<p>This plugin will add non-breaking spaces where appropriate in the content, excerpt, comments, and text widget &mdash; skipping over pre-formatted code blocks and scripts &mdash; and if the <code>&lt;!--:fr--&gt;</code> HTML  tag is found, non-breaking spaces will be added only between the <code>&lt;!--:fr--&gt;</code> and <code>&lt;!--:--&gt;</code> HTML tags.</p>

<h4>Recognized Punctuation</h4>

<ul>
<li>?</li>
<li>!</li>
<li>%</li>
<li>:</li>
<li>;</li>
<li>&laquo;</li>
<li>&raquo;</li>
<li>Currency symbols and numeric thousands (example: 1 000,10 $).</li>
</ul>

<h4>Developer Filters</h4>

<p><em>'nbsp_french_filter_priority' ( $priority )</em> &mdash; The default filter priority (default: 10).</p>

<p><em>'nbsp_french_add_filters' ( array $names )</em> &mdash; The default filter list to hook (default: 'the_title', 'the_content', 'the_excerpt', 'comment_text', 'widget_title', 'widget_text' ).</p>

<p><em>'nbsp_french_filter_'.$name ( $bool )</em> &mdash; Hook the filter name (default: true).</p>

<p><em>'nbsp_french_currencies' ( $pcre )</em> &mdash; A list of recognized currencies.</p>

<p><em>'nbsp_french_preg_first_second_last' ( array $pattern )</em> &mdash; An array of patterns to match. Spaces are replaced in the second set of parenthesis, and the returned string corresponds to the first, second, and last set of parenthesis.</p>

<p>To hook additional text filters, include their names in the 'nbsp_french_add_filters' array, or hook them individually in your functions.php file:</p>

<pre>
add_filter( $filter_name, array( 'NbspFrench', 'filter' ) );
</pre>


<h2>Installation</h2>

<h4>Automated Install</h4>

<ol>
<li>Go to the wp-admin/ section of your website</li>
<li>Select the <em>Plugins</em> menu item</li>
<li>Select the <em>Add New</em> sub-menu item</li>
<li>In the <em>Search</em> box, enter the plugin name</li>
<li>Click the <em>Search Plugins</em> button</li>
<li>Click the <em>Install Now</em> link for the plugin</li>
<li>Click the <em>Activate Plugin</em> link</li>
</ol>

<h4>Semi-Automated Install</h4>

<ol>
<li>Download the plugin archive file</li>
<li>Go to the wp-admin/ section of your website</li>
<li>Select the <em>Plugins</em> menu item</li>
<li>Select the <em>Add New</em> sub-menu item</li>
<li>Click on <em>Upload</em> link (just under the Install Plugins page title)</li>
<li>Click the <em>Browse...</em> button</li>
<li>Navigate your local folders / directories and choose the zip file you downloaded previously</li>
<li>Click on the <em>Install Now</em> button</li>
<li>Click the <em>Activate Plugin</em> link</li>
</ol>


<h2>Frequently Asked Questions</h2>

<h4>Frequently Asked Questions</h4>

<ul>
<li>None</li>
</ul>


<h2>Other Notes</h2>

<h3>Other Notes</h3>
<h4>Additional Documentation</h4>

<ul>
<li>None</li>
</ul>

