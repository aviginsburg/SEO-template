# An SEO Template for Facebook (Twitter, Schema, AMP, and debugging coming soon)

You can go straight to the SEO template by clicking <a href="./seo.html">here</a>, for more of an explanation keep reading.

So you've setup your website and you want to get noticed. You want to be the top hit when people hit up a search term on Google. To do this, you need to start thinking properly about SEO or Search Engine Optimisation. Many people think SEO is not important, but in 2019 with a world of paid avertisements SEO has a more crucial place in your marketing strategy than ever.

In the past, SEO has just involved using some <code>meta</code> tags in your <code>title</code> section of your HTML page. Today, o for keywords to describe your site. This worked for a while but soon this was being spammed, now <code>meta</code> tags have fallen out of favour and are practically obselete.


## Contents
<ul>
  <li><a href="https://github.com/aviginsburg/SEO-template#what-is-seo">What is SEO?</a></li>
  <li><a href="https://github.com/aviginsburg/SEO-template#traditional-seo">Traditional SEO</a></li>
  <li><a href="https://github.com/aviginsburg/SEO-template#modern-seo">Modern SEO</a></li>
  <li><a href="https://github.com/aviginsburg/SEO-template#facebook-opengraph">Facebook OpenGraph</a></li>
<!--   <li>Twitter</li> -->
<!--   <li>Schema.org</li>  -->
<!--   <li>robot.txt</li> -->
<!--   <li>AMP</li> -->
<!--   <li>Crucial Links</li> -->
</ul>

### What is SEO?
SEO stands for Search Engine Optimisation and is a practice of growing the visibility of links and webpages on search sites. It is the practice of moving your page from the tenth Google <b>o</b> to the top of the first page. 

Search Engines like Google would deploy bots or crawlers on new sites, assessing them for keywords, content, phrases, structure and links. These bots will then return a summary to Google which will rank the sites when a user searches.

### Traditional SEO 
Previously SEO was a more simple endeavour. There were a couple of major points you had to cover:
<ul>
  <li><b>Keywords</b> - these were the way to highlight unique words or phrases on your site. This was soon corrupted with keyword stuffing and other pratices to the point where Google will now penalised your site for having too many keywords</li>
  <li><b>Page Ranking</b> - another principle in SEO where a page is ranked by the number of <i>other</i> sites that link to it. Furthermore, the rank of the website dictates how value that is given to the websites <b>it links to</b>. The more websites you link to, the lower the impact of weight of your websites. This was done to prevent websites from cramming thousands of links, inflating their position</li>
</ul>

This can be seen in the code below. The layout here is called <b>metadata</b>, which is defined as providing data about other kinds of data.

```
    <title>How to SEO!</title>
    <meta name="keywords" content="SEO, templates, modern SEO, Search Engines" >
    <meta name="description" content="An easy way to understand and implement the newest practices in SEO" >
```

### Modern SEO
Modern SEO has moved further toewards providing functionality outside a website as well as inside. For example, type <i>easy spaghetti recipe</i> into Google, and Google will provide ten or twenty recipes without you clicking on a single site. These are all examples of sites moving outside their borders. Facebook, Twitter and others also show higher engagement rates for links where the author,a picture, and a small description are provided. Sites need to be able to be immediately inviting to users. 

Facebook has led this, with its <a href="ogp.me/">Open Graph Protocol</a> slowly becoming an industry standard. Twitter also has its own standard, as does Google. These will all be covered here, with accompanying code.

### Facebook OpenGraph
The OpenGraph Protocol is a series <code>meta property</code> tags for declaring the nature of a site, as well as information about the author, aithor's sits, pictures and dimensions. We have also seen Facebook links done badly, an image blown up 10x. It doesn't look inviting.

Facebook demands images of certain dimensions. Images are not allowed to be larger than <b>1200 x 630</b> or Facebook will take a chunk and remove the rest. Images can be as small as <b>600 x 315</b>. Here is a typical example of Facebook OpenGraph metadata.

```
    <meta property="og:url" content="www.example.com" />
    <meta property="og:type" content="website" />
    <meta property="og:title" content="Welcome to Example!" />
    <meta property="og:description" content="This is what your page does!" />
    <meta property="og:image" content="https://www.example.com/public/images/fb_img_1200_630.jpg" />
    <meta property="og:image:secure_url" content="https://www.example.com/public/images/fb_img_1200_630.jpg" />
    <meta property="og:image:width" content="1200" />
    <meta property="og:image:height" content="630" />
    <meta property="og:site_name" content="Example" />
    <meta property="”og:see_also”" content="www.example.com/cool-thing-1" />
    <meta property="”og:see_also”" content="www.example.com/cool-thing-2" />
```
   
Many of the tags above are self explanatory, but there are some which bear mentioning. 

#### <a href="http://ogp.me/#types">og:type</a>
To increase engagement, allowing Facebook to know what type of site you have means it will be able to change the interactions available to users. For example, if you are posting about a music video then the music:video tag would be the best one. There are tens of possible variants like books, music, restarants, videos, news, and products.

#### og:see_also
See_also allows additional items of content to be diplayed below the link to allow users to easily move between content. This one is a bit more up in the air though. All reference to it has been removed from Facebook, Pinterest and OpenGraph's sites, so one could assume it is no longer in use. I include it just in case though.

It is crucial to point out that <b>all the data above must be correct for when Facebook first crawls your site</b>. You can be stuck with old metadata for <b>years!!</b>
