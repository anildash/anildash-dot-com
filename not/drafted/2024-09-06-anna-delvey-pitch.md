---
title: "How I got pitched by Anna Delvey"
slug: anna-delvey-pitch
date_published: 2024-09-06T12:00:05.000Z
heroimage:
tags: [absurdity]
---

Many people will be familiar with Anna Sorokin, also known as Anna Delvey, who was one of the most high-profile of the wave of hipster grifters during the 2010s. Today, she's beginning to pivot into some kind of reality TV/competition game show participant, playing on her celebrity, but back in 2016, she was just a person pitching strangers for her big idea that she was trying to get funded.

The basic pitch is especially amusing these days because Anna was trying to get everyone excited about... a big, vague AI startup with no proven business model or use cases. Maybe she was just ahead of her time!

A lot of people have told me they were curious about what, exactly, Anna's pitch looked like, so I thought I'd share what I saw.

First, on February 22, 2016, there was this original email, under the subject line, "Artificial Intelligence X Art project":

<blockquote>
  Hello Anil,

  My team and I are working on a new project that will explore Al creativity in art context by enabling direct collaboration between artist and Al, which will produce data that could be applied to problem solving on a higher level. I am a 25 year old art collector based in New York, and together with professors from the largest Al research institute in the world DFKI we are developing soft- and hardware that will be assigned to selected high-profile contemporary artists and will create a show exhibiting the results. See more details in dropbox links below.

  The project is a part of a bigger initiative and is planned to launch simultaneously with the opening of my new art foundation designed by Calatrava and located in Aby Rosen's building in Gramercy NYC. In the future we are looking to experiment further and integrate Artificial Intelligence in different areas involving art and creativity.

  We are currently raising our first $1mm round of financing.

  Let me know your thoughts.

  Best,

  Anna Delvey
  
</blockquote>

First of all, how _quaint_ is it that an AI startup would be raising only one million dollars in funding? Also, I love the signifiers of mentioning the designer of her art foundation — who can argue with the taste of a art collector who likes Calatrava? I'm assuming at least part of the reason she reached out to me at the time was that I had been <a href="https://www.anildash.com/2021/11/14/i-didnt-invent-nfts-but-we-dont-really-have-any-other-way-to-talk-about-tech/">orbiting around the code-and-art scene in NYC</a> for a while at that point, and was probably one of the few folks who was visible both with the museum crowd and as a VC-backed startup founder.

But really, I don't know exactly how she found me. Staying true to my character, I never replied to the email. So, she had a follow-up pitch a few weeks later, on March 27, 2016:

<blockquote>
  Hello Anil,
  
  My team and I are working on the first Al-powered creative assistant in the world, and its reverse reaction-predicting counterpart. We are based in NYC, and together with professors from the largest Al research institute in the world DFKI and MIT in Boston we are developing soft- and hardware that will facilitate creative collaboration between an individual and Al.

  Our deck: https://www.dropbox.com/s/w8ldihpt1wxkkz3/DECK%20COAl.pdf?dI=0
  
  We are currently in the middle of assembling a board of advisors and raising our seed round.
  
  Let me know your thoughts.
  
  Anna Delvey
  
</blockquote>

This message is the source of the <a href="https://cdn.glitch.global/034ff067-8128-4744-8807-d19cee4142e7/DECK%20COAI.pdf?v=1725635335907">original PDF of her pitch deck</a> that you can use to follow along with her story. (Side note: she signed her emails below her name with her initials, which are the same as mine, and it still throws me off because it felt like I had somehow sent these messages to myself.)


<script type="module">
 import pdfjs-dist from https://cdn.jsdelivr.net/npm/pdfjs-dist@4.6.82/+esm 
// If absolute URL from the remote server is provided, configure the CORS
// header on that server.
var url = 'https://cdn.glitch.global/034ff067-8128-4744-8807-d19cee4142e7/DECK%20COAI.pdf?v=1725635335907';

// Loaded via <script> tag, create shortcut to access PDF.js exports.
var { pdfjsLib } = globalThis;

// The workerSrc property shall be specified.
pdfjsLib.GlobalWorkerOptions.workerSrc = '//mozilla.github.io/pdf.js/build/pdf.worker.mjs';

// Asynchronous download of PDF
var loadingTask = pdfjsLib.getDocument(url);
loadingTask.promise.then(function(pdf) {
  console.log('PDF loaded');

  // Fetch the first page
  var pageNumber = 1;
  pdf.getPage(pageNumber).then(function(page) {
    console.log('Page loaded');

    var scale = 1.5;
    var viewport = page.getViewport({scale: scale});

    // Prepare canvas using PDF page dimensions
    var canvas = document.getElementById('the-canvas');
    var context = canvas.getContext('2d');
    canvas.height = viewport.height;
    canvas.width = viewport.width;

    // Render PDF page into canvas context
    var renderContext = {
      canvasContext: context,
      viewport: viewport
    };
    var renderTask = page.render(renderContext);
    renderTask.promise.then(function () {
      console.log('Page rendered');
    });
  });
}, function (reason) {
  // PDF loading error
  console.error(reason);
});
</script>


<canvas id="the-canvas"></canvas>