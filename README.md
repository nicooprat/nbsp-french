<h1>JSM&#039;s Non-Breaking Space for French Content</h1>

<table>
<tr><th align="right" valign="top" nowrap>Plugin Name</th><td>JSM&#039;s Non-Breaking Space for French Content</td></tr>
<tr><th align="right" valign="top" nowrap>Summary</th><td>Adds a non-breaking space between words and punctuation marks to avoid inappropriate line-breaks in French.</td></tr>
<tr><th align="right" valign="top" nowrap>Stable Version</th><td>1.10.0</td></tr>
<tr><th align="right" valign="top" nowrap>Requires PHP</th><td>5.6 or newer</td></tr>
<tr><th align="right" valign="top" nowrap>Requires WordPress</th><td>4.2 or newer</td></tr>
<tr><th align="right" valign="top" nowrap>Tested Up To WordPress</th><td>5.4.1</td></tr>
<tr><th align="right" valign="top" nowrap>Contributors</th><td>jsmoriss</td></tr>
<tr><th align="right" valign="top" nowrap>License</th><td><a href="https://www.gnu.org/licenses/gpl.txt">GPLv3</a></td></tr>
<tr><th align="right" valign="top" nowrap>Tags / Keywords</th><td>non-breaking, french, content, line-break, punctuation, space, new line, line break</td></tr>
</table>

<h2>Description</h2>

<p>This plugin adds non-breaking spaces required by the French language in the content, excerpt, comments, text widget, and WooCommerce short description &mdash; skipping over pre-formatted code blocks, styles and scripts.</p>

<p>If the <code>&lt;!--:fr--&gt;</code> HTML  tag is found (used by some multilingual plugins), non-breaking spaces are added only between the <code>&lt;!--:fr--&gt;</code> and <code>&lt;!--:--&gt;</code> HTML tags.</p>

<p>There are no plugin settings &mdash; simply <em>install</em> and <em>activate</em> the plugin.</p>

<h4>Filters for Developers</h4>

<p><strong>'nbsp_french_add_filters' ( array $filter_names )</strong></p>

<p>An associative array of filter names (and priority) for the plugin to hook.</p>

<pre>
array(
    'the_title'                     => 10,
    'the_content'                   => 10,
    'the_excerpt'                   => 10,
    'comment_text'                  => 10,
    'widget_title'                  => 10,
    'widget_text'                   => 10,
    'woocommerce_short_description' => 10,
)
</pre>

<p>To hook additional filters, include their names (and priority) in the 'nbsp_french_add_filters' array, or hook them individually in your functions.php:</p>

<pre>
add_filter( 'another_text_filter_name',
    array( 'NbspFrench', 'filter' ), 10, 1 );
</pre>

<p><strong>'nbsp_french_currencies' ( $regex )</strong></p>

<p>A regular expression of recognized currency symbols.</p>


<h2>Installation</h2>

<h4>Automated Install</h4>

<ol>
<li>Go to the wp-admin/ section of your website.</li>
<li>Select the <em>Plugins</em> menu item.</li>
<li>Select the <em>Add New</em> sub-menu item.</li>
<li>In the <em>Search</em> box, enter the plugin name.</li>
<li>Click the <em>Search Plugins</em> button.</li>
<li>Click the <em>Install Now</em> link for the plugin.</li>
<li>Click the <em>Activate Plugin</em> link.</li>
</ol>

<h4>Semi-Automated Install</h4>

<ol>
<li>Download the plugin ZIP file.</li>
<li>Go to the wp-admin/ section of your website.</li>
<li>Select the <em>Plugins</em> menu item.</li>
<li>Select the <em>Add New</em> sub-menu item.</li>
<li>Click on <em>Upload</em> link (just under the Install Plugins page title).</li>
<li>Click the <em>Browse...</em> button.</li>
<li>Navigate your local folders / directories and choose the ZIP file you downloaded previously.</li>
<li>Click on the <em>Install Now</em> button.</li>
<li>Click the <em>Activate Plugin</em> link.</li>
</ol>


<h2>Frequently Asked Questions</h2>




