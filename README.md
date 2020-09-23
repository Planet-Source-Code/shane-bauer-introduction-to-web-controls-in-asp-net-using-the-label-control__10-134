<div align="center">

## Introduction  to Web Controls in ASP\.NET using the label control


</div>

### Description

This is to give you an introduction to the idea of controls by using the label control.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Shane Bauer](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/shane-bauer.md)
**Level**          |Beginner
**User Rating**    |5.0 (20 globes from 4 users)
**Compatibility**  |VB\.NET, ASP\.NET
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__10-9.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/shane-bauer-introduction-to-web-controls-in-asp-net-using-the-label-control__10-134/archive/master.zip)





### Source Code


<p><br><br>
<p>Web Controls are server-side elements used to create
&quot;smart forms&quot; in ASP.NET.&nbsp; These Web controls actually turn into
html elements when they are processed on the server.&nbsp; In this article, I am
going to explain how to use the label control.&nbsp; My goal is to teach you
step-by-step by keeping it simple.&nbsp; Instead of throwing all web controls together in one
article, I am going to break it down so you don't get too much at one time.&nbsp;
Ready? Let's begin!</p>
<p><b>The &quot;label&quot; Control</b></p>
<p>Adding static content to your page has always been easy.&nbsp;
But what if you want to dynamically change what will be displayed?&nbsp; You
could use the &quot;label&quot; control.&nbsp; Here is the code:</p>
<p><font color="#0000FF">&lt;asp:Label id=&quot;lblexample&quot; runat=&quot;server&quot;
/&gt;</font></p>
<p>This is the minimal amount of code you need to create a
label.&nbsp; If you wanted to set a default text value in the label, you would
do something like this:</p>
<p><font color="#0000FF">&lt;asp:Label id=&quot;lblexample&quot; text=&quot;This is my first label&quot;
runat=&quot;server&quot; /&gt;</font></p>
<p>Lets break some of this down for a minute.&nbsp; The &quot;<font color="#0000FF">asp:Label</font>&quot;
part is the start of the control.&nbsp; The &quot;id&quot; parameter is going to be the
name of your label control.&nbsp; You can name yours whatever you want. In the
text parameter, it set a default text value to &quot;This is my first label.&quot;&nbsp;
Do not forget the &quot;runat=server&quot; part. When you execute your page, it
will display &quot;This is my first label.&quot; </p>
<p>If you wanted to change the text dynamically in a subroutine, you would
call the following:</p>
<p><font color="#0000FF">lblexample.text = &quot;New text would go here!&quot;</font></p>
<p>Remember, if you did not call your label &quot;lblexample&quot; then
you would have to change the tag to the appropriate name. </p>
<p>Are you ready for your first example? Of course you are!&nbsp;
</p>
<p><font color="#0000FF">&lt;script runat=&quot;server&quot;&gt;</font></p>
<p><font color="#0000FF">Sub page_load<br>
lblexample.text = &quot;Welcome to my site!&quot;<br>
End Sub</font></p>
<p><font color="#0000FF">&lt;/script&gt;</font></p>
<p><font color="#0000FF">&lt;html&gt;<br>
&lt;head&gt;<br>
&lt;title&gt;My first label&lt;/title&gt;<br>
&lt;/head&gt;<br>
&lt;body&gt;<br>
&lt;asp:Label id=&quot;lblexample&quot; runat=&quot;server&quot; /&gt;<br>
&lt;/body&gt;<br>
&lt;/html&gt;</font></p>
<p>Let me explain this now.&nbsp; We started off the script
by using &quot;<font color="#0000FF">&lt;script runat=&quot;server&quot;&gt;</font>.&quot; This starts are
server-side scripting section.&nbsp; We will hide our subroutines in there. In
the next line, we declare our first (and only) subroutine.&nbsp; This subroutine
is called &quot;page_load.&quot; This subroutine will always be executed when the page
begins to load.&nbsp; For your own reference, you can always use the &quot;page_load&quot;
sub in any of your pages. It will always execute first. The &quot;page_load&quot;
subroutine is a good place to declare and store variables which you will use
throughout the script.</p>
<p>In the next line, we called &quot;lblexample.text.&quot; This will
change the text value in the control named &quot;lblexample&quot; to &quot;Welcome to my
site!&quot;.</p>
<p>After that, we just clean up by ending the &quot;page_load&quot; sub
and closing the script tag.&nbsp; This allows us to start developing what the
user will see when he/she comes to the page.&nbsp; Notice, the rest is all HTML
tags except for the one label control entitled &quot;lblexample.&quot; This is the spot
where the &quot;Welcome to my site!&quot; text will be placed.&nbsp; Simple isn't it?</p>
<p>I hope you found that somewhat helpful.&nbsp; I tried to
keep it as simple as possible but still not making it boring.&nbsp; Please vote
and leave your comments! If you have any problems or you get stuck, please email
me at <a href="mailto:webmaster@sourcecode-central.com">
webmaster@sourcecode-central.com</a>. I will be glad to help you!</p>
<p>&nbsp;</p>

