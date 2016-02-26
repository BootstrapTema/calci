# CalcI
##Responsive Calc Iframe
###Ratio 16/9
###Ratio 3/2
###Ratio 4/3
####Bootstrap 3+
##CSS
<pre><code>
.calci {position:relative;width:100%;height:0;overflow:hidden}
.c-16-9 {padding-top:calc(100%/(16/9))}
.c-16-9 iframe {width:100%;height:100%;position:absolute;top:0;left:0}
.c-3-2 {padding-top:calc(100%/(3/2))}
.c-3-2 iframe {width:calc((100%/(3/2)) * (16/9));height:100%;position:absolute;top:0;left:calc((100% - ((100%/(3/2)) * (16/9))) / 2)}
.c-4-3 {padding-top:calc(100%/(4/3))}
.c-4-3 iframe {width:calc((100%/(4/3)) * (16/9));height:100%;position:absolute;top:0;left:calc((100% - ((100%/(4/3)) * (16/9))) / 2)}
</code></pre>
##SCSS
<pre><code>
.calci {
  position: relative;
  width: 100%;
  height: 0;
  overflow: hidden;
}
.c-16-9 {
  padding-top: calc(100%/(16/9));
  iframe {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
  }
}
.c-3-2 {
  padding-top: calc(100%/(3/2));
  iframe {
    width: calc((100%/(3/2)) * (16/9));
    height: 100%;
    position: absolute;
    top: 0;
    left: calc((100% - ((100%/(3/2)) * (16/9))) / 2);
  }
}
.c-4-3 {
  padding-top: calc(100%/(4/3));
  iframe {
    width: calc((100%/(4/3)) * (16/9));
    height: 100%;
    position: absolute;
    top: 0;
    left: calc((100% - ((100%/(4/3)) * (16/9))) / 2);
  }
}
</code></pre>
##Code
<pre><code>
&lt;div class="calci c-3-2"&gt;
&lt;iframe src="http://url.swf" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen&gt;&lt;/iframe&gt;
&lt;/div&gt;
</code></pre>
