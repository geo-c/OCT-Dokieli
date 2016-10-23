# GEO-C guidelines

One of the most important parts of the GEO-C project is to share outputs in each doctoral thesis. To achieve this, we provide a template to create interactive guidelines in order to share these advances. 

These guides use the Dokieli (https://github.com/linkeddata/dokieli) tool. Dokieli is a decentralized article authoring, annotation, and social notification tool which works from a web browser.

Dokieli is coded using HTML, where a main file defines all content. We define mandatory sections, so all guidelines have to follow. The first part of the guidelines is the title and a short description. Also, the guidelines have to include six sections: Context, Challenges, Actions, Results, Impact and Scaling Up.  Following, we show the fragments to change in order to personalize the guidelines.

*Title
<h1 property="schema:name doap:name">Title Guideline</h1>

*Description general
<p id="introduction" property="schema:description doap:shortdesc">Description ... ... ...</p>

*Sections (Context ex.) content
<section id="context" inlist="" rel="schema:hasPart" resource=" #context">
<h2 property="schema:name">Context</h2>
<div datatype="rdf:HTML" property="schema:description">
     <p>bla bla bla ...</p>
</div>
</section>


To offer an interactive guideline, Dockieli supports the possibility to add some media elements. We show some snippets to add these items.  

*Photo
<img src="URL.jpg" style="width:304px; height:228px;">

*Audio
<audio src="URL.ogg"></audio>

*Video
<video poster="http://www.html5rocks.com/es/tutorials/video/basics/star.png" id="video-canvas-frames" controls="" >
<source src="URL.mp4" type="video/mp4; codecs=&quot;avc1.42E01E,             mp4a.40.2&quot;">
<source src="URL.webm" type="video/webm; codecs=&quot;vp8, vorbis&quot;">
<source src="URL.ogv" type="video/ogg; codecs=&quot;theora, vorbis&quot;">
</video>


Also, Dokieli (HTML5) offer more functions.


*PDF
<figure id="fig_userStudy">
<object data="URL.pdf" type="application/pdf"        
width="100%" height="350" internalinstanceid="3" title="">
      <p>It appears you don't have a PDF plugin for this browser. 
      No biggie... you can <a href="URL.pdf">click here 
      to the PDF file.</a></p>
</object>
<figcaption>Caption.</figcaption>
</figure>  

Reference call
<a href="#fig_userStudy">Figure 1</a>

*SPARQL GUI
<figure id="figure-sparql-editor">
<object type="text/html" data="http://yasgui.org/" width="640" height="480"></object>
<figcaption>SPARQL GUI</figcaption>
</figure>


Also, you can add other components like maps, chats, … using Javascript libraries that you know!


##How deploy your guideline


When you have updated the index.html, you will need a web server, like Apache. An easy option is to use Apache is installing XAMPP. To setup XAMPP, you can follow the next steps:

*Download the latest version for your platform (Linux, Windows, Mac OS X, or Solaris) from apachefriends.
*Run the executable to extract it (you can extract it straight to C:\ if you want; it'll create an XAMPP subfolder and put all the files there) and answer the questions setup will ask you. Rename the folder to XAMPP.
*At the end, setup will give you an option to start the XAMPP control panel; select that option and it should pop up.
*Check the checkboxes for Apache and click on their respective Start button to start.
*Copy all files and folder provided in the Guideline zip (guidelineV_0.zip) and the updated index.html into a subfolder e.g. esrX\ of the htdocs folder, wherever that is e.g. c:\xampp\htdocs\.
*Direct your browser to the appropriate page, e.g. http://localhost/esrX

