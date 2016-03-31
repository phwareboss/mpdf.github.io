---
layout: page
title: CJKforceend
parent_title: mPDF Variables
permalink: /reference/mpdf-variables/cjkforceend.html
---

<div id="bpmbook" class="bpmbook" style="direction:ltr;">
<div class="topic_user_field">
<div id="U0">
<p>(mPDF &gt;= 5.7)</p>
<p>CJK line-breaking is implemented in mPDF roughly according to accepted rules.</p>
<p>Configurable variables allow fine control of behaviour:</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp; $this-&gt;CJKforceend = false; // Forces overflowng punctuation to hang outside right margin (used with CJK script)</p>
<p>&nbsp;&nbsp;&nbsp; $this-&gt;allowCJKorphans = true;&nbsp;&nbsp;&nbsp; // FALSE=always wrap to next line; TRUE=squeeze or overflow

&nbsp;&nbsp;&nbsp; $this-&gt;allowCJKoverflow = false; // FALSE=squeeze; TRUE=overflow (only selected)</p>
<p>&nbsp;</p>
<p>IF $this-&gt;allowCJKorphans == true AND $this-&gt;allowCJKoverflow == true AND $this-&gt;CJKforceend == true AND text-align:justify

will force hanging punctuation to hang outside right margin.</p>
<p>&nbsp;</p>
<p>See also <a href="/reference/mpdf-variables/allowcjkoverflow.html">allowCJKoverflow</a> and <a href="/reference/mpdf-variables/allowcjkorphans.html">allowCJKorphans</a></p>
</div>
</div>
