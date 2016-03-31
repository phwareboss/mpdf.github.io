---
layout: page
title: SetDisplayPreferences()
parent_title: mPDF functions
permalink: /reference/mpdf-functions/setdisplaypreferences.html
---

<div id="bpmbook" class="bpmbook" style="direction:ltr;">
<div class="topic_user_field">
<div id="U0">
<p>(mPDF &gt;= 3.0)</p>
<p>SetDisplayPreferences – Defines the way the document shall be presented on the screen</p>
<h2>Description</h2>

<div class="alert alert-info" role="alert">void <b>SetDisplayPreferences</b> ( string <span class="parameter">$prefs</span> )</div>
<p>Specify the way the document shall be presented on the screen when the PDF file is opened in Adobe Reader. When the user opens the finished file in Adobe Reader, these values will determine the initial appearance and layout.</p>
<h2>Parameters</h2>
<p class="manual_param_dt"><span class="parameter">prefs</span></p>
<p class="manual_param_dd">This parameter takes a string containing any one or more of the possible values separated by any characters (e.g. comma, forward slash or space). All the options start as <span class="smallblock">FALSE</span>, and can only be set <span class="smallblock">TRUE</span> by this command. Each setting is added to those previously set.</p>
<p class="manual_param_dd"><b>Values</b> (case-sensitive)

FullScreen: Full-screen mode, with no menu bar, window controls, or any other window visible

HideMenubar: whether to hide the conforming reader’s menu bar when the document is active

HideToolbar: whether to hide the conforming reader’s tool bars when the document is active

HideWindowUI: whether to hide user interface elements in the document’s window (such as scroll bars and navigation controls), leaving only the document’s contents displayed

DisplayDocTitle: whether the window’s title bar should display the document title taken from the Title entry of the document information dictionary. If false, the title bar will instead display the name of the PDF file containing the document

CenterWindow: whether to position the document’s window in the center of the screen

FitWindow: whether to resize the document’s window to fit the size of the first displayed page

NoPrintScaling: overrides the user's default setting to scale the printing size (mPDF &gt;= 5.1)</p>
<h2>Examples</h2>

{% highlight php %}
Example #1
{% endhighlight %}

{% highlight php %}
<?php

<?php

$mpdf=new mPDF();

$mpdf->SetDisplayPreferences('/HideMenubar/HideToolbar/DisplayDocTitle');

$mpdf->WriteHTML('<p>Hallo World</p>');

$mpdf->Output('filename.pdf');

?>
{% endhighlight %}

<h2>See Also

</h2>
<ul>
<li class="manual_boxlist"><a href="/reference/mpdf-functions/setdisplaymode.html">SetDisplayMode()</a> - Specify the initial Display Mode when the PDF file is opened in Adobe Reader</li>
</ul>
<p>&nbsp;</p>
</div>
</div>
